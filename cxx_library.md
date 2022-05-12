::: {#fb-root}
:::

::: topbar
[](http://buck.build/)

# Buck

-   
-   [Docs](/setup/getting_started.html)
-   [Issues](https://github.com/facebook/buck/issues)
-   [GitHub](https://github.com/facebook/buck)
:::

::: socialBanner
Support Ukraine. [Help Provide Humanitarian Aid to
Ukraine](https://opensource.fb.com/support-ukraine).
:::

::: {.section .content}
::: width
# cxx_library()

::: overview
[This is liable to change in the future.]{.small}

A `cxx_library()` rule specifies a set of C/C++ source files and also
provides flags that specify how those files should be built.

### Building requires a specified top-level target

Whether a Buck command builds the `cxx_library` is determined by the
inclusion of a top-level target, such as a
[`cxx_binary`](/rule/cxx_binary.html) or
[`android_binary`](/rule/android_binary.html), that transitively depends
on the `cxx_library`. The set of targets specified to the Buck command
(`buck build`, `buck run`, etc) must include one of these top-level
targets in order for Buck to build the `cxx_library`. Note that you
could specify the top-level target implicitly using a [build target
pattern](/concept/build_target_pattern.html) or you could also specify
the top-level target using an
[`[alias]`](/files-and-dirs/buckconfig.html#alias) defined in
`.buckconfig`.

*How* Buck builds the library also depends on the specified top-level
target. For example, a C/C++ binary (`cxx_binary`) would require a
static non-PIC build of the library, whereas an Android APK
(`android_binary`) would require a shared PIC-enabled build. (PIC stands
for position-independent code.)

#### Dependencies of the cxx_library also require a top-level target

Similarly, in order for Buck to build a target that the `cxx_library`
depends on, such as a [`cxx_genrule`](/rule/cxx_genrule.html), you must
specify in the Buck command a top-level target that depends on the
`cxx_library`. For example, you could specify to
[`buck build`](/command/build.html) a `cxx_binary` that depends on the
`cxx_library`. If you specify as your build target the `cxx_library`
itself, the build targets that the `cxx_library` depends on *might not
be built*.

## Arguments

-   ::: {#name}
    ### `name`{.argName} [(required)]{.argDefault} [\#](#name){.inline-link}

    The *short name* for this [build
    target](/concept/build_target.html).
    :::

-   ::: {#srcs}
    ### `srcs`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#srcs){.inline-link}

    The set of C, C++, Objective-C, Objective-C++, or assembly source
    files to be preprocessed, compiled, and assembled by this rule. We
    determine which stages to run on each input source based on its file
    extension. See the [GCC
    documentation](https://gcc.gnu.org/onlinedocs/gcc/Overall-Options.html)
    for more detail on how file extensions are interpreted. Each element
    can be either a string specifying a source file (e.g. `'foo/bar.c'`)
    or a tuple of a string specifying a source file and a list of
    compilation flags (e.g. `('foo/bar.c', ['-Wall', '-Werror'])`). In
    the latter case the specified flags will be used in addition to the
    rule\'s other flags when preprocessing and compiling that file (if
    applicable).
    :::

-   ::: {#platform_srcs}
    ### `platform_srcs`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#platform_srcs){.inline-link}

    Platform specific source files. These should be specified as a list
    of pairs where the first element is an un-anchored regex (in
    java.util.regex.Pattern syntax) against which the platform name is
    matched, and the second element is either a list of source files or
    a list of tuples of source files and a list of compilation flags to
    be preprocessed, compiled and assembled if the platform matches the
    regex. See `srcs` for more information.
    :::

-   ::: {#headers}
    ### `headers`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#headers){.inline-link}

    The set of header files that are made available for inclusion to the
    source files in this target. These should be specified as either a
    list of header files or a dictionary of header names to header
    files. The header name can contain forward slashes (`/`). The
    headers can be included with
    `#include "$HEADER_NAMESPACE/$HEADER_NAME"` or
    `#include <$HEADER_NAMESPACE/$HEADER_NAME>`, where
    `$HEADER_NAMESPACE` is the value of the target\'s `header_namespace`
    attribute, and `$HEADER_NAME` is the header name if specified, and
    the filename of the header file otherwise. See `header_namespace`
    for more information.
    :::

-   ::: {#platform_headers}
    ### `platform_headers`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#platform_headers){.inline-link}

    Platform specific header files. These should be specified as a list
    of pairs where the first element is an un-anchored regex (in
    java.util.regex.Pattern syntax) against which the platform name is
    matched, and the second element is either a list of header files or
    a dictionary of header names to header files that will be made
    available for inclusion to the source files in the target if the
    platform matches the regex. See `headers` for more information.
    :::

-   ::: {#exported_headers}
    ### `exported_headers`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#exported_headers){.inline-link}

    The set of header files that are made available for inclusion to the
    source files in the target and all targets that transitively depend
    on it. These should be specified as either a list of header files or
    a dictionary of header names to header files. The headers can be
    included with `#include "$HEADER_NAMESPACE/$HEADER_NAME"` or
    `#include <$HEADER_NAMESPACE/$HEADER_NAME>`, where
    `$HEADER_NAMESPACE` is the value of the target\'s `header_namespace`
    attribute, and `$HEADER_NAME` is the header name if specified, and
    the filename of the header file otherwise. Note that the header name
    can contain forward slashes (`/`). See `header_namespace` for more
    information.
    :::

-   ::: {#exported_header_style}
    ### `exported_header_style`{.argName} [(defaults to `local`)]{.argDefault} [\#](#exported_header_style){.inline-link}

    How dependents should include exported headers from this rule. Can
    be either `local`(e.g. `-I`) or `system` (e.g. `-isystem`).
    :::

-   ::: {#exported_platform_headers}
    ### `exported_platform_headers`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#exported_platform_headers){.inline-link}

    Platform specific header files. These should be specified as a list
    of pairs where the first element is an un-anchored regex (in
    java.util.regex.Pattern syntax) against which the platform name is
    matched, and the second element is either a list of header files or
    a dictionary of header names to header files that will be made
    available for inclusion to the source files in the target and all
    targets that transitively depend on it if the platform matches the
    regex. See `headers` for more information.
    :::

-   ::: {#header_namespace}
    ### `header_namespace`{.argName} [(defaults to `name`)]{.argDefault} [\#](#header_namespace){.inline-link}

    A path prefix when including headers of this target. Defaults to the
    path from the root of the repository to the directory where this
    target is defined. Can contain forward slashes (`/`), but cannot
    start with one. See `headers` for more information.
    :::

-   ::: {#preprocessor_flags}
    ### `preprocessor_flags`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#preprocessor_flags){.inline-link}

    Flags to use when preprocessing any of the above sources (which
    require preprocessing).
    :::

-   ::: {#lang_preprocessor_flags}
    ### `lang_preprocessor_flags`{.argName} [(defaults to `{}`)]{.argDefault} [\#](#lang_preprocessor_flags){.inline-link}

    Language-specific preprocessor flags. These should be specified as a
    map of C-family language short names to lists of flags and is used
    to target flags to sources files for a specific language in the
    C-family (C, C++, assembler, etc.). The keys in the map can be:

    -   `c` for C
    -   `c++` for C++
    -   `objective-c` for Objective-C
    -   `objective-c++` for Objective-C++
    -   `cuda` for Cuda
    -   `assembler-with-cpp` for Assembly
    -   `asm-with-cpp` for ASM
    :::

-   ::: {#platform_preprocessor_flags}
    ### `platform_preprocessor_flags`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#platform_preprocessor_flags){.inline-link}

    Platform specific preprocessor flags. These should be specified as a
    list of pairs where the first element is an un-anchored regex (in
    java.util.regex.Pattern syntax) against which the platform name is
    matched, and the second element is a list of flags to use when
    preprocessing the target\'s sources. See `preprocessor_flags` for
    more information.
    :::

-   ::: {#lang_platform_preprocessor_flags}
    ### `lang_platform_preprocessor_flags`{.argName} [(defaults to `{}`)]{.argDefault} [\#](#lang_platform_preprocessor_flags){.inline-link}

    Language- and platform-specific preprocessor flags. These should be
    specified as a map of C-family language short names, as described in
    `lang_preprocessor_flags`, to lists of pairs, as described in
    `platform_preprocessor_flags`.
    :::

-   ::: {#exported_preprocessor_flags}
    ### `exported_preprocessor_flags`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#exported_preprocessor_flags){.inline-link}

    Just as `preprocessor_flags`, flags to use when preprocessing any of
    the above sources (which require preprocessing). However, unlike
    `preprocessor_flags`, these preprocessor flags are also used by
    rules that transitively depend on this rule when preprocessing their
    own sources.
    :::

-   ::: {#exported_lang_preprocessor_flags}
    ### `exported_lang_preprocessor_flags`{.argName} [(defaults to `{}`)]{.argDefault} [\#](#exported_lang_preprocessor_flags){.inline-link}

    Just as `lang_preprocessor_flags`, but these flags also apply to
    rules that transitively depend on this rule.
    :::

-   ::: {#exported_platform_preprocessor_flags}
    ### `exported_platform_preprocessor_flags`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#exported_platform_preprocessor_flags){.inline-link}

    Platform specific exported preprocessor flags. These should be
    specified as a list of pairs where the first element is an
    un-anchored regex (in java.util.regex.Pattern syntax) against which
    the platform name is matched, and the second element is a list of
    flags to use when preprocessing the source files in the target and
    all targets that transitively depend on it if the platform matches
    the regex. See `exported_preprocessor_flags` for more information.
    :::

-   ::: {#exported_lang_platform_preprocessor_flags}
    ### `exported_lang_platform_preprocessor_flags`{.argName} [(defaults to `{}`)]{.argDefault} [\#](#exported_lang_platform_preprocessor_flags){.inline-link}

    Just as `lang_platform_preprocessor_flags`, but these flags also
    apply to rules that transitively depend on this rule.
    :::

-   ::: {#compiler_flags}
    ### `compiler_flags`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#compiler_flags){.inline-link}

    Flags to use when compiling any of the above sources (which require
    compilation).
    :::

-   ::: {#lang_compiler_flags}
    ### `lang_compiler_flags`{.argName} [(defaults to `{}`)]{.argDefault} [\#](#lang_compiler_flags){.inline-link}

    Language-specific compiler flags. These should be specified as a map
    of C-family language short names to lists of flags and is used to
    target flags to sources files for a specific language in the
    C-family (C, C++, assembler, etc.). The keys in the map can be:

    -   `cpp-output` for C
    -   `c++-cpp-output` for C++
    -   `objective-c-cpp-output` for Objective-C
    -   `objective-c++-cpp-output` for Objective-C++
    -   `cuda-cpp-output` for Cuda
    -   `assembler` for Assembly
    -   `asm` for ASM
    :::

-   ::: {#platform_compiler_flags}
    ### `platform_compiler_flags`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#platform_compiler_flags){.inline-link}

    Platform specific compiler flags. These should be specified as a
    list of pairs where the first element is an un-anchored regex (in
    java.util.regex.Pattern syntax) against which the platform name is
    matched, and the second element is a list of flags to use when
    compiling the target\'s sources. See `compiler_flags` for more
    information.
    :::

-   ::: {#lang_platform_compiler_flags}
    ### `lang_platform_compiler_flags`{.argName} [(defaults to `{}`)]{.argDefault} [\#](#lang_platform_compiler_flags){.inline-link}

    Language- and platform-specific compiler flags. These should be
    specified as a map of C-family language short names, as described in
    `lang_compiler_flags`, to lists of pairs, as described in
    `platform_compiler_flags`.
    :::

-   ::: {#linker_extra_outputs}
    ### `linker_extra_outputs`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#linker_extra_outputs){.inline-link}

    Declares extra outputs that the linker emits. These identifiers can
    be used in `$(output ...)` macros in `linker_flags` to interpolate
    the output path into the linker command line. Useful for custom
    linkers that emit extra output files.
    :::

-   ::: {#linker_flags}
    ### `linker_flags`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#linker_flags){.inline-link}

    Flags to add to the linker command line whenever the output from
    this rule is used in a link operation, such as linked into an
    executable or a shared library.
    :::

-   ::: {#platform_linker_flags}
    ### `platform_linker_flags`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#platform_linker_flags){.inline-link}

    Platform-specific linker flags. This argument is specified as a list
    of pairs where the first element in each pair is an un-anchored
    regex against which the platform name is matched. The regex should
    use `java.util.regex.Pattern` syntax. The second element in each
    pair is a list of linker flags. If the regex matches the platform,
    these flags are added to the linker command line when the output
    from this rule is used in a link operation.
    :::

-   ::: {#exported_linker_flags}
    ### `exported_linker_flags`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#exported_linker_flags){.inline-link}

    Flags to add to the linker command line when the output from this
    rule, or the output from any rule that transitively depends on this
    rule, is used in a link operation.
    :::

-   ::: {#exported_post_linker_flags}
    ### `exported_post_linker_flags`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#exported_post_linker_flags){.inline-link}

    Flags to add to the linker command line when the output from this
    rule, or the output from any rule that transitively depends on this
    rule, is used in a link operation---with the additional feature that
    these flags are guaranteed to be placed *after* the compiled object
    (`.o`) files on the linker command line.
    :::

-   ::: {#exported_platform_linker_flags}
    ### `exported_platform_linker_flags`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#exported_platform_linker_flags){.inline-link}

    Platform-specific linker flags for this rule and for all rules that
    transitively depend on this rule. This argument is specified as a
    list of pairs where the first element in each pair is an un-anchored
    regex against which the platform name is matched. The regex should
    use `java.util.regex.Pattern` syntax. The second element in each
    pair is a list of linker flags. If the regex matches the platform,
    these flags are added to the linker command line when the output
    from this rule, or the output from any rule that transitively
    depends on this rule, is used in a link operation.
    :::

-   ::: {#exported_post_platform_linker_flags}
    ### `exported_post_platform_linker_flags`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#exported_post_platform_linker_flags){.inline-link}

    Platform-specific linker flags for this rule and for all rules that
    transitively depend on this rule---and that are guaranteed to be
    placed *after* the compiled object (`.o`) files on the linker
    command line. In other respects, the syntax and semantics of this
    argument are the same as for the `exported_platform_linker_flags`
    argument.
    :::

-   ::: {#link_style}
    ### `link_style`{.argName} [(defaults to `static`)]{.argDefault} [\#](#link_style){.inline-link}

    Determines whether to build and link this rule\'s dependencies
    statically or dynamically. Can be either `static`, `static_pic` or
    `shared`.
    :::

-   ::: {#link_whole}
    ### `link_whole`{.argName} [(defaults to `False`)]{.argDefault} [\#](#link_whole){.inline-link}

    On some platforms, the linker may choose to drop objects from
    libraries if it determines they may be unused. This parameter causes
    the linker to always include the entire library in top-level
    executables or shared libraries.
    :::

-   ::: {#raw_headers}
    ### `raw_headers`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#raw_headers){.inline-link}

    The set of header files that can be used for inclusion to the source
    files in the target and all targets that transitively depend on it.
    Buck doesn\'t add raw headers to the search path of a
    compiler/preprocessor automatically.`include_directories` and
    `public_include_directories` are the recommended way to add raw
    headers to the search path (they will be added via
    `-I`).`compiler_flags`, `preprocessor_flags` and
    `exported_preprocessor_flags`can also be used to add such raw
    headers to the search path if inclusion via `-isystem` or`-iquote`
    is needed.`raw_headers` cannot be used together with `headers` or
    `exported_headers` in the same target.
    :::

-   ::: {#include_directories}
    ### `include_directories`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#include_directories){.inline-link}

    A list of include directories (with `raw_headers`) to be added to
    the compile command for compiling this target (via `-I`). An include
    directory is relative to the current package.
    :::

-   ::: {#public_include_directories}
    ### `public_include_directories`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#public_include_directories){.inline-link}

    A list of include directories (with `raw_headers`) to be added to
    the compile command for compiling this target and every target that
    depends on it (via `-I`). An include directory is relative to the
    current package.
    :::

-   ::: {#public_system_include_directories}
    ### `public_system_include_directories`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#public_system_include_directories){.inline-link}

    A list of include directories (with `raw_headers`) to be added to
    the compile command for compiling this target and every target that
    depends on it (via `-isystem` if the compiler supports it of via
    `-I` otherwise). An include directory is relative to the current
    package.
    :::

-   ::: {#soname}
    ### `soname`{.argName} [(defaults to `None`)]{.argDefault} [\#](#soname){.inline-link}

    Sets the soname (\"shared object name\") of any shared library
    produced from this rule. The default value is based on the full rule
    name. The macro `$(ext)` will be replaced with a
    platform-appropriate extension. An argument can be provided, which
    is a library version. For example `soname = 'libfoo.$(ext 2.3)'`
    will be `libfoo.2.3.dylib` on Mac and `libfoo.so.2.3` on Linux.
    :::

-   ::: {#supported_platforms_regex}
    ### `supported_platforms_regex`{.argName} [(defaults to `None`)]{.argDefault} [\#](#supported_platforms_regex){.inline-link}

    If present, an un-anchored regex (in java.util.regex.Pattern syntax)
    that matches all platforms that this library supports. It will not
    be built for other platforms.
    :::

-   ::: {#force_static}
    ### `force_static`{.argName} [(defaults to `False`)]{.argDefault} [\#](#force_static){.inline-link}

    DEPRECATED: `See preferred_linkage`. If `true`, the library will
    always be linked statically, even if the target that depends on it
    specifies `link_style` to be something other than `static`. Note
    that this may still cause the library to be linked into its own
    shared library, if it happens to be the root of the linkable
    dependency tree (e.g. if a Python library directly depends on the
    library with `force_static=True`). Also note this will cause
    duplicate symbols if multiple targets that depend on the library are
    linked together.
    :::

-   ::: {#preferred_linkage}
    ### `preferred_linkage`{.argName} [(defaults to `any`)]{.argDefault} [\#](#preferred_linkage){.inline-link}

    Controls how a library should be linked.

    `any`
    :   The library will be linked based on its dependents `link_style`.

    `shared`
    :   The library will be always be linked as a shared library.

    `static`
    :   The library will be linked as a static library.

    Note: since shared libraries re-export its dependencies, depending
    on multiple shared libraries which themselves have overlapping
    static dependencies will cause duplicate symbols.
    :::

-   ::: {#reexport_all_header_dependencies}
    ### `reexport_all_header_dependencies`{.argName} [(defaults to `True`)]{.argDefault} [\#](#reexport_all_header_dependencies){.inline-link}

    Whether to automatically re-export the exported headers of all
    dependencies.

    When this is set to false, only exported headers from
    `exported_deps` are re-exported.
    :::

-   ::: {#exported_deps}
    ### `exported_deps`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#exported_deps){.inline-link}

    Dependencies that will also appear to belong to any rules that
    depend on this one. This has two effects:

    -   Exported dependencies will also be included in the link line of
        dependents of this rules, but normal dependencies will not.
    -   When `reexport_all_header_dependencies = False`, only exported
        headers of the rules specified here are re-exported.
    :::

-   ::: {#exported_platform_deps}
    ### `exported_platform_deps`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#exported_platform_deps){.inline-link}

    Platform specific dependencies that will also appear to belong to
    any rules that depend on this one. These should be specified as a
    list of pairs where the first element is an un-anchored regex (in
    java.util.regex.Pattern syntax) against which the platform name is
    matched, and the second element is a list of external dependencies
    (same format as `exported_deps`) that are exported if the platform
    matches the regex. See `exported_deps` for more information.
    :::

-   ::: {#precompiled_header}
    ### `precompiled_header`{.argName} [(defaults to `None`)]{.argDefault} [\#](#precompiled_header){.inline-link}

    Path to a
    [`cxx_precompiled_header`](/rule/cxx_precompiled_header.html) to use
    when compiling this rule\'s sources. The precompiled header (PCH) is
    built on-demand, using compiler flags matching those used in this
    rule\'s compile jobs. This is to ensure compatibility between this
    rule and the PCH. Also, this rule will inherit additional `deps`
    from the PCH rule, and as a result, additional include paths as well
    (e.g. `-I`, `-isystem`, `-iquote` path lists, and framework paths
    specified with `-F`).
    :::

-   ::: {#tests}
    ### `tests`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#tests){.inline-link}

    List of [build targets](/concept/build_target.html) that identify
    tests that exercise this target.
    :::

-   ::: {#extra_xcode_sources}
    ### `extra_xcode_sources`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#extra_xcode_sources){.inline-link}

    When the project is generated, this is the list of files that will
    added to the build phase \"Compile Sources\" of the given target.
    :::

-   ::: {#extra_xcode_files}
    ### `extra_xcode_files`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#extra_xcode_files){.inline-link}

    When the project is generated, this is the list of files that will
    added to the project. Those files won\'t be added to the build phase
    \"Compile Sources\".
    :::

-   ::: {#visibility}
    ### `visibility`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#visibility){.inline-link}

    List of [build target patterns](/concept/build_target_pattern.html)
    that identify the build rules that can include this rule as a
    dependency, for example, by listing it in their `deps` or
    `exported_deps` attributes. For more information, see
    [visibility](/concept/visibility.html).
    :::

-   ::: {#licenses}
    ### `licenses`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#licenses){.inline-link}

    Set of license files for this library. To get the list of license
    files for a given [build rule](/concept/build_rule.html) and all of
    its dependencies, you can use [`buck query`](/command/query.html).
    :::

-   ::: {#labels}
    ### `labels`{.argName} [(defaults to `[]`)]{.argDefault} [\#](#labels){.inline-link}

    Set of arbitrary strings which allow you to annotate a [build
    rule](/concept/build_rule.html) with tags that can be searched for
    over an entire dependency tree using
    [`buck query attrfilter()`](/command/query.html#attrfilter).
    :::

## Examples

``` {.prettyprint .lang-py}
# A rule that includes a single .cpp file and its corresponding header and
# also supplies an additional flag for compilation.
cxx_library(
  name = 'fileutil',
  srcs = [
    'fileutil.cpp',
  ],
  exported_headers = [
    'fileutil.h',
  ],
  compiler_flags = [
    '-fno-omit-frame-pointer',
  ],
)

# A rule that defines explicit names for its headers
cxx_library(
  name = 'mathutils',
  header_namespace = 'math',
  srcs = [
    'trig/src/cos.cpp',
    'trig/src/tan.cpp',
  ],
  exported_headers = {
    # These are included as <math/trig/cos.h> and <math/trig/tan.h>
    'trig/cos.h': 'trig/include/cos.h',
    'trig/tan.h': 'trig/include/tan.h',
  },
  compiler_flags = [
    '-fno-omit-frame-pointer',
  ],
)

# A rule that uses different headers and sources per platform
cxx_library(
  name = 'vector',
  # Because of platform_headers, this file can include "config.h"
  # and get the architecture specific header
  srcs = ['vector.cpp'],
  platform_srcs = [
    ('.*armv7$', 'armv7.S'),
    ('.*x86_64$', 'x86_64.S'),
  ],
  exported_headers = [
    'vector.h',
  ],
  platform_headers = [
    (
      '.*armv7$',
      {
        'config.h': 'config-armv7.h',
      }
    ),
    (
      '.*x86_64$',
      {
        'config.h': 'config-x86_64.h',
      }
    ),
  ],
)
```
:::

### The Basics

-   [Getting Started](/setup/getting_started.html)
-   [Key Concepts](/about/overview.html)
-   [Tutorial](/learning/tutorial.html)
-   [Installing the IntelliJ
    Plugin](/setup/intellij_plugin_install.html)
-   [Exopackage](/article/exopackage.html)
-   [Buck Cheat Sheet](/article/query_cheat_sheet.html)

### About

-   [What Makes Buck so Fast?](/concept/what_makes_buck_so_fast.html)
-   [Showcase](/about/showcase.html)
-   [Troubleshooting](/concept/troubleshooting.html)
-   [Performance Tuning](/about/performance_tuning.html)
-   [FAQ](/concept/faq.html)
-   [Learn More (Buck Presentations)](/presentations/index.html)

### Concepts

-   [Build Rule](/concept/build_rule.html)
-   [Build File](/concept/build_file.html)
-   [Build Target](/concept/build_target.html)
-   [Build Target Pattern](/concept/build_target_pattern.html)
-   [Buck Daemon (buckd)](/concept/buckd.html)
-   [Visibility](/concept/visibility.html)
-   [Flavors](/concept/flavors.html)
-   [HTTP Cache API](/concept/http_cache_api.html)
-   [Rule Keys](/concept/rule_keys.html)
-   [Java ABIs](/concept/java_abis.html)
-   [Skylark](/concept/skylark.html)

### Files and Directories

-   [.buckconfig](/files-and-dirs/buckconfig.html)
-   [.buckjavaargs](/files-and-dirs/buckjavaargs.html)
-   [buck-out](/files-and-dirs/buck-out.html)

### Commands

-   [Common Parameters](/command/common_parameters.html)
-   [buck audit](/command/audit.html)
-   [buck build](/command/build.html)
-   [buck clean](/command/clean.html)
-   [buck doctor](/command/doctor.html)
-   [buck fetch](/command/fetch.html)
-   [buck fix](/command/fix.html)
-   [buck install](/command/install.html)
-   [buck kill](/command/kill.html)
-   [buck killall](/command/killall.html)
-   [buck project](/command/project.html)
-   [buck publish](/command/publish.html)
-   [buck query](/command/query.html)
-   [buck run](/command/run.html)
-   [buck root](/command/root.html)
-   [buck server](/command/server.html)
-   [buck targets](/command/targets.html)
-   [buck test](/command/test.html)
-   [buck uninstall](/command/uninstall.html)
-   [Exit Codes](/command/exit_codes.html)

### Build Rules

-   **Core**
-   [command_alias()](/rule/command_alias.html)
-   [export_file()](/rule/export_file.html)
-   [filegroup()](/rule/filegroup.html)
-   [genrule()](/rule/genrule.html)
-   [http_archive()](/rule/http_archive.html)
-   [http_file()](/rule/http_file.html)
-   [remote_file()](/rule/remote_file.html)
-   [test_suite()](/rule/test_suite.html)
-   [worker_tool()](/rule/worker_tool.html)
-   [zip_file()](/rule/zip_file.html)
-   **Android**
-   [android_aar()](/rule/android_aar.html)
-   [android_binary()](/rule/android_binary.html)
-   [android_build_config()](/rule/android_build_config.html)
-   [android_instrumentation_apk()](/rule/android_instrumentation_apk.html)
-   [android_instrumentation_test()](/rule/android_instrumentation_test.html)
-   [android_library()](/rule/android_library.html)
-   [android_manifest()](/rule/android_manifest.html)
-   [android_prebuilt_aar()](/rule/android_prebuilt_aar.html)
-   [android_resource()](/rule/android_resource.html)
-   [apk_genrule()](/rule/apk_genrule.html)
-   [gen_aidl()](/rule/gen_aidl.html)
-   [keystore()](/rule/keystore.html)
-   [ndk_library()](/rule/ndk_library.html)
-   [prebuilt_jar()](/rule/prebuilt_jar.html)
-   [prebuilt_native_library()](/rule/prebuilt_native_library.html)
-   [robolectric_test()](/rule/robolectric_test.html)
-   **CXX**
-   [cxx_binary()](/rule/cxx_binary.html)
-   [cxx_library()](/rule/cxx_library.html)
-   [cxx_genrule()](/rule/cxx_genrule.html)
-   [cxx_precompiled_header()](/rule/cxx_precompiled_header.html)
-   [cxx_test()](/rule/cxx_test.html)
-   [prebuilt_cxx_library()](/rule/prebuilt_cxx_library.html)
-   [prebuilt_cxx_library_group()](/rule/prebuilt_cxx_library_group.html)
-   **D**
-   [d_binary()](/rule/d_binary.html)
-   [d_library()](/rule/d_library.html)
-   [d_test()](/rule/d_test.html)
-   **Go**
-   [go_binary()](/rule/go_binary.html)
-   [go_library()](/rule/go_library.html)
-   [go_test()](/rule/go_test.html)
-   [cgo_library()](/rule/cgo_library.html)
-   **Groovy**
-   [groovy_library()](/rule/groovy_library.html)
-   **Halide**
-   [halide_library()](/rule/halide_library.html)
-   **Haskell**
-   [haskell_binary()](/rule/haskell_binary.html)
-   [haskell_library()](/rule/haskell_library.html)
-   [prebuilt_haskell_library()](/rule/prebuilt_haskell_library.html)
-   **iOS**
-   [apple_asset_catalog()](/rule/apple_asset_catalog.html)
-   [apple_binary()](/rule/apple_binary.html)
-   [apple_bundle()](/rule/apple_bundle.html)
-   [apple_library()](/rule/apple_library.html)
-   [apple_package()](/rule/apple_package.html)
-   [apple_resource()](/rule/apple_resource.html)
-   [apple_test()](/rule/apple_test.html)
-   [core_data_model()](/rule/core_data_model.html)
-   [prebuilt_apple_framework()](/rule/prebuilt_apple_framework.html)
-   **Java**
-   [java_binary()](/rule/java_binary.html)
-   [java_library()](/rule/java_library.html)
-   [java_test()](/rule/java_test.html)
-   [prebuilt_jar()](/rule/prebuilt_jar.html)
-   [prebuilt_native_library()](/rule/prebuilt_native_library.html)
-   **Kotlin**
-   [kotlin_library()](/rule/kotlin_library.html)
-   [kotlin_test()](/rule/kotlin_test.html)
-   **Lua**
-   [cxx_lua_extension()](/rule/cxx_lua_extension.html)
-   [lua_binary()](/rule/lua_binary.html)
-   [lua_library()](/rule/lua_library.html)
-   **OCaml**
-   [ocaml_binary()](/rule/ocaml_binary.html)
-   [ocaml_library()](/rule/ocaml_library.html)
-   **Python**
-   [prebuilt_python_library()](/rule/prebuilt_python_library.html)
-   [python_binary()](/rule/python_binary.html)
-   [python_library()](/rule/python_library.html)
-   [python_test()](/rule/python_test.html)
-   **Rust**
-   [rust_binary()](/rule/rust_binary.html)
-   [rust_library()](/rule/rust_library.html)
-   [rust_test()](/rule/rust_test.html)
-   [prebuilt_rust_library()](/rule/prebuilt_rust_library.html)
-   **Shell**
-   [sh_binary()](/rule/sh_binary.html)
-   [sh_test()](/rule/sh_test.html)
-   **.NET**
-   [csharp_library()](/rule/csharp_library.html)
-   [prebuilt_dotnet_library()](/rule/prebuilt_dotnet_library.html)

### Functions

-   **Python DSL**
-   [add_build_file_dep()](/function/add_build_file_dep.html)
-   [allow_unsafe_import()](/function/allow_unsafe_import.html)
-   [flatten_dicts()](/function/flatten_dicts.html)
-   [glob()](/function/glob.html)
-   [get_base_path()](/function/get_base_path.html)
-   [get_cell_name()](/function/get_cell_name.html)
-   [host_info()](/function/host_info.html)
-   [include_defs()](/function/include_defs.html)
-   [load()](/function/load.html)
-   [read_config()](/function/read_config.html)
-   [subdir_glob()](/function/subdir_glob.html)
-   [String Parameter Macros](/function/string_parameter_macros.html)

```{=html}
<!-- -->
```
-   **Skylark**
-   [glob()](/skylark/generated/glob.html)
-   [host_info()](/skylark/generated/host_info.html)
-   [package_name()](/skylark/generated/package_name.html)
-   [provider()](/skylark/generated/provider.html)
-   [read_config()](/skylark/generated/read_config.html)
-   [repository_name()](/skylark/generated/repository_name.html)
-   [rule_exists()](/skylark/generated/rule_exists.html)

### Extending Buck

-   [Custom Macros](/extending/macros.html)
-   [Custom Rules](/extending/rules.html)
-   [Building E2E Tests for Buck](/extending/e2e_tests.html)
:::
:::

::: width
© Copyright Facebook, 2013 - 2020
:::

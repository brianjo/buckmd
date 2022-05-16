/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.flavors} /\*\*\*/ {template .soyweb} {call buck.page} {param title:
\'Flavors\' /} {param navid: \'concept_flavors\' /} {param prettify:
true /} {param description} Flavors in Buck are a way to specify
different variations of a build that otherwise share most configuration
specifications. {/param} {param content}

Flavors in Buck are a way to specify different variations of a build
that otherwise share most configuration specifications.

Flavors can also be used to simultaneously build for two different
platforms, such as iOS and watchOS. Being able to build for both of
these at the same time is important because iOS application can have a
dependency on the Watch application.

Flavors fall into a number of different categories:

-   [Platform](#platform_http)
-   [Linker](#linker_http)
-   [Symbol](#symbol_http)
-   [Analysis](#analysis_http)
-   [Header](#header_http)
-   [Apple debug](#apple_debug_http)
-   [Apple bundles](#apple_bundles_http)

## Syntax for flavors

A flavor is specified as a suffix to a build target, with the hash mark
(#) used as a separator between the target and flavor. Examples:

{literal}

    buck build :cxx_gr_name#default
    buck build :cxx_gr_name#iphonesimulator-x86_64

{/literal}

You can specify multiple flavors for a single target by separating the
flavors with commas:

{literal}

    buck build Libraries/3rdParty/openssl:ssl#android-armv7,static-pic
    buck build Libraries/3rdParty/openssl:ssl#android-x86,static-pic
    buck build :bundle#iphoneos-x86_64,strip-all,dwarf-and-dsym

{/literal}

**NOTE:** Buck supports a {call buck.concept_link}{param page:
\'build_target_pattern\' /}{param name: \'build target pattern\'
/}{/call}, `...`, as in, `//apps/...`, that specifies that Buck should
recurse through build files in subdirectories, building all build
targets in any build files it finds. *This build target pattern does not
support specifying flavors.*

### Default flavors

The `cxx_library` and `apple_library` rules support specifying *default
flavors*, which pertain if a build target is specified 1)
explicitly-that is, not using a {call buck.concept_link}{param page:
\'build_target_pattern\' /}{param name: \'build target pattern\'
/}{/call} -and 2) without a flavor.

### Syntax for Flagfile Flavors

A flavor may also be specified as a suffix to an \@file or \--flagfile
argument. These flavors are used within the flagfile only and do not
directly change the target flavor. The separator is \'#\' as above, and
if the separator and flavor are present, the \@file (aka flagfile) must
end in \".py\" and be a Python script. The script will be called as
follows:

{literal}

    python /path/to/flagfile.py --flavors 

{/literal}

## Platform flavors [\#](#platform_http){.inline-link} {#platform_http}

These flavors denote a toolchain to use for compiling. You can also use
them to control conditional fields in the Buck target\'s rule.

  Flavor                   Meaning
  ------------------------ -------------------------------
  android-armv7            32-bit Android device
  android-x86              32-bit Android emulator
  iphoneos                 
  iphoneos-armv7           32-bit iPhone device
  iphoneos-arm64           64-bit iPhone device
  iphoneos-i386            
  iphoneos-x86_64          
  iphonesimulator          
  iphonesimulator-i386     Simulator on 32-bit Mac
  iphonesimulator-x86_64   Simulator on 64-bit Mac
  macosx-x86_64            Native x86_64 OSX application
  macosx-arm64             Native arm64 OSX application
  windows-x86_64           Native Windows application

Sighted in the wild:

{literal}

    buck build :main#android-arm64,shared

{/literal}

## Linker flavors [\#](#linker_http){.inline-link} {#linker_http}

### Static

{literal}

    static

{/literal}

Static library (.a)

### Position-independent code (PIC)

{literal}

    static-pic

{/literal}

Static library that generates position-independent code (PIC). Note that
on the Apple platforms, everything is PIC.

### Shared

A shared library (so) or dynamically-loaded module (.dylib on Mac, .dll
on Windows).

### Shared interface

{literal}

    shared-interface

{/literal}

A stub library that only lists the imports and exports of a shared
library. You can link against this library, but it doesn\'t have any
executable code.

### Linker Map

{literal}

    no-linkermap

{/literal}

Specifying this flavor suppresses the generation of a LinkMap.txt file,
which is normally generated by the Apple linker (ld).

## Analysis flavors [\#](#analysis_http){.inline-link} {#analysis_http}

### Rust language

{literal}

    check

{/literal}

The Rust compiler has a build mode which quickly checks syntax and type
correctness, but avoids codegen (which is the slowest phase of Rust
compilation). This flavor invokes check on the suffixed build target.

{literal}

    save-analysis

{/literal}

The `#save-analysis` flavor is an extension of #check. It performs the
same actions as a #check build, but also emits a .json file containing
full type/symbol cross-reference information, for consumption by tools
like RLS (Rust Language Services).

{literal}

    doc

{/literal}

The `#doc` flavor is the equivalent of the cargo doc command. It uses
the rustdoc tool to generate documentation for a target and its
dependencies.

### Compilation database

If you specify one of these flavors, Buck generates analysis information
about your build.

{literal}

    compilation-database

{/literal}

Produces a JSON file that contains (an approximation of) the compiler
commands for compiling each file. The output is in the [clang
compilation
database](https://eli.thegreenplace.net/2014/05/21/compilation-databases-for-clang-based-tools)
format.

### Infer

{literal}

    infer-analyze
    infer-capture-all

{/literal}

These flavors run [Facebook\'s Infer tool](https://fbinfer.com) and
generate intermediate Infer output.

## Symbol stripping flavors[\#](#symbol_http){.inline-link} {#symbol_http}

These flavor control how symbols are stripped from an output binary.

### Strip debug

{literal}

    strip-debug

{/literal}

Strip debug symbols; equivalent to `strip -S`.

### Strip debug and non-external

{literal}

    strip-non-global

{/literal}

Strip debug and non-external symbols; equivalent to `strip -x`.

### Strip all

{literal}

    strip-all

{/literal}

Strip all the things; equivalent to strip with no arguments.

## Header Flavors[\#](#header_http){.inline-link} {#header_http}

These flavors are used with C++ header files, in the deps or
exported_deps attributes of a Buck target.

### Headers used to compile a libraries own files

{literal}

    private-headers

{/literal}

Symlink tree, or header map, of headers used for compiling a library\'s
own files.

### Headers used to compile files that depend on this library

{literal}

    headers

{/literal}

Symlink tree, or header map, of headers used to compile files for other
libraries that depend on this library.

## Apple debug flavors[\#](#apple_debug_http){.inline-link} {#apple_debug_http}

Selects the actual binary used to represent a {call buck.cxx_binary /}.

### Stripped binary

{literal}

    no-debug

{/literal}

Selects the stripped binary

### Unstripped binary

{literal}

    dwarf

{/literal}

Selects the unstripped binary

### Unstripped + dsym

{literal}

    dwarf-and-dsym

{/literal}

Selects the unstripped binary, and the dsym file.

### Other

{literal}

    apple-debuggable-binary

{/literal}

Could be stripped and unstripped, depending on requirements.

## Apple bundles flavors[\#](#apple_bundles_http){.inline-link} {#apple_bundles_http}

These flavors are legacy methods of creating app and framework bundles.

*You should not use these.*

Instead of these flavors, we now use the Buck rule, {call
buck.apple_bundle /}

### App

{literal}

    app
    binary#app

{/literal}

Generates an app bundle.

### Framework

{literal}

    framework
    library#framework

{/literal}

Generates a framework.

{/param} {/call} {/template}

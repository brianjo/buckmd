<div>

JavaScript is disabled on your browser.

</div>

::: {role="banner"}
::: fixedNav
::: topNav
[]{#navbar.top}

::: skipNav
[Skip navigation links](#skip.navbar.top "Skip navigation links")
:::

[]{#navbar.top.firstrow}

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

```{=html}
<!-- -->
```
-   SEARCH:

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

<div>

-   Summary: 
-   Nested \| 
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
::: subTitle
[Package]{.packageLabelInType} [com.facebook.buck.swift](package-summary.html)
:::

## Class SwiftBuckConfig {#class-swiftbuckconfig .title title="Class SwiftBuckConfig"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.swift.SwiftBuckConfig

::: description
-   

    All Implemented Interfaces:
    :   `ConfigView<BuckConfig>`

    ------------------------------------------------------------------------

        public class SwiftBuckConfig
        extends Object
        implements ConfigView<BuckConfig>

    ::: block
    A Swift-specific \"view\" of BuckConfig.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                         Description
          ------------------- ----------------------------- -------------
          `static String`     `COMPILE_FORCE_CACHE`          
          `static String`     `COMPILER_FLAGS_NAME`          
          `static String`     `COPY_STDLIB_TO_FRAMEWORKS`    
          `static String`     `EMIT_SWIFTDOCS`               
          `static String`     `PROJECT_ADD_AST_PATHS`        
          `static String`     `PROJECT_EMBED_RUNTIME`        
          `static String`     `PROJECT_WMO`                  
          `static String`     `USE_FILELIST`                 
          `static String`     `USE_LIPO_THIN`                
          `static String`     `USE_MODULEWRAP`               
          `static String`     `VERSION_NAME`                 

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                              Description
          ---------------------------------------- -------------
          `SwiftBuckConfig​(BuckConfig delegate)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `boolean`             | `ge                   |                       |
        |                       | tCompileForceCache()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Option               | `getCompilerFlags()`  |                       |
        | al<Iterable<String>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getCopy              | ::: block             |
        |                       | StdlibToFrameworks()` | If enabled,           |
        |                       |                       | swift-stdlib-tool     |
        |                       |                       | will be run on        |
        |                       |                       | .framework bundles,   |
        |                       |                       | copying the Swift     |
        |                       |                       | standard library into |
        |                       |                       | them.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `BuckConfig`          | `getDelegate()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getEmitSwiftdocs()`  | ::: block             |
        |                       |                       | If enabled, a         |
        |                       |                       | .swiftdoc file will   |
        |                       |                       | be generated along    |
        |                       |                       | with the .swiftmodule |
        |                       |                       | file.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `get                  | ::: block             |
        |                       | ProjectAddASTPaths()` | If enabled, AST paths |
        |                       |                       | to the .swiftmodules  |
        |                       |                       | will be added as part |
        |                       |                       | of the linker         |
        |                       |                       | invocation.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getP                 | ::: block             |
        |                       | rojectEmbedRuntime()` | If enabled,           |
        |                       |                       | automatically emebds  |
        |                       |                       | the Swift runtime if  |
        |                       |                       | a relevant target     |
        |                       |                       | depends on any        |
        |                       |                       | libraries that use    |
        |                       |                       | Swift.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getProjectWMO()`     | ::: block             |
        |                       |                       | If enabled, turns on  |
        |                       |                       | Whole Module          |
        |                       |                       | Optimization for any  |
        |                       |                       | targets that contain  |
        |                       |                       | Swift.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getUseFileList()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getUseLipoThin()`    | ::: block             |
        |                       |                       | Uses \`lipo -thin\`   |
        |                       |                       | instead of \`lipo     |
        |                       |                       | -extract\` when       |
        |                       |                       | copying the Swift     |
        |                       |                       | standard libraries.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getUseModulewrap()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getVersion()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `of​(                  |                       |
        | atic SwiftBuckConfig` | BuckConfig delegate)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#COMPILER_FLAGS_NAME}

        -   #### COMPILER_FLAGS_NAME

                public static final String COMPILER_FLAGS_NAME

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.swift.SwiftBuckConfig.COMPILER_FLAGS_NAME)

        []{#VERSION_NAME}

        -   #### VERSION_NAME

                public static final String VERSION_NAME

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.swift.SwiftBuckConfig.VERSION_NAME)

        []{#COMPILE_FORCE_CACHE}

        -   #### COMPILE_FORCE_CACHE

                public static final String COMPILE_FORCE_CACHE

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.swift.SwiftBuckConfig.COMPILE_FORCE_CACHE)

        []{#USE_FILELIST}

        -   #### USE_FILELIST

                public static final String USE_FILELIST

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.swift.SwiftBuckConfig.USE_FILELIST)

        []{#USE_MODULEWRAP}

        -   #### USE_MODULEWRAP

                public static final String USE_MODULEWRAP

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.swift.SwiftBuckConfig.USE_MODULEWRAP)

        []{#PROJECT_WMO}

        -   #### PROJECT_WMO

                public static final String PROJECT_WMO

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.swift.SwiftBuckConfig.PROJECT_WMO)

        []{#PROJECT_EMBED_RUNTIME}

        -   #### PROJECT_EMBED_RUNTIME

                public static final String PROJECT_EMBED_RUNTIME

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.swift.SwiftBuckConfig.PROJECT_EMBED_RUNTIME)

        []{#PROJECT_ADD_AST_PATHS}

        -   #### PROJECT_ADD_AST_PATHS

                public static final String PROJECT_ADD_AST_PATHS

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.swift.SwiftBuckConfig.PROJECT_ADD_AST_PATHS)

        []{#COPY_STDLIB_TO_FRAMEWORKS}

        -   #### COPY_STDLIB_TO_FRAMEWORKS

                public static final String COPY_STDLIB_TO_FRAMEWORKS

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.swift.SwiftBuckConfig.COPY_STDLIB_TO_FRAMEWORKS)

        []{#USE_LIPO_THIN}

        -   #### USE_LIPO_THIN

                public static final String USE_LIPO_THIN

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.swift.SwiftBuckConfig.USE_LIPO_THIN)

        []{#EMIT_SWIFTDOCS}

        -   #### EMIT_SWIFTDOCS

                public static final String EMIT_SWIFTDOCS

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.swift.SwiftBuckConfig.EMIT_SWIFTDOCS)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.config.BuckConfig)}

        -   #### SwiftBuckConfig

                public SwiftBuckConfig​(BuckConfig delegate)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getDelegate()}

        -   #### getDelegate

            ``` methodSignature
            public BuckConfig getDelegate()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDelegate` in interface `ConfigView<BuckConfig>`

        []{#of(com.facebook.buck.core.config.BuckConfig)}

        -   #### of

            ``` methodSignature
            public static SwiftBuckConfig of​(BuckConfig delegate)
            ```

        []{#getCompilerFlags()}

        -   #### getCompilerFlags

            ``` methodSignature
            public Optional<Iterable<String>> getCompilerFlags()
            ```

        []{#getVersion()}

        -   #### getVersion

            ``` methodSignature
            public Optional<String> getVersion()
            ```

        []{#getCompileForceCache()}

        -   #### getCompileForceCache

            ``` methodSignature
            public boolean getCompileForceCache()
            ```

        []{#getUseFileList()}

        -   #### getUseFileList

            ``` methodSignature
            public boolean getUseFileList()
            ```

        []{#getUseModulewrap()}

        -   #### getUseModulewrap

            ``` methodSignature
            public boolean getUseModulewrap()
            ```

        []{#getProjectEmbedRuntime()}

        -   #### getProjectEmbedRuntime

            ``` methodSignature
            public boolean getProjectEmbedRuntime()
            ```

            ::: block
            If enabled, automatically emebds the Swift runtime if a
            relevant target depends on any libraries that use Swift.
            :::

        []{#getProjectWMO()}

        -   #### getProjectWMO

            ``` methodSignature
            public boolean getProjectWMO()
            ```

            ::: block
            If enabled, turns on Whole Module Optimization for any
            targets that contain Swift.
            :::

        []{#getProjectAddASTPaths()}

        -   #### getProjectAddASTPaths

            ``` methodSignature
            public boolean getProjectAddASTPaths()
            ```

            ::: block
            If enabled, AST paths to the .swiftmodules will be added as
            part of the linker invocation. This is necessary for lldb to
            be able to debug statically linked Swift libraries.
            :::

        []{#getCopyStdlibToFrameworks()}

        -   #### getCopyStdlibToFrameworks

            ``` methodSignature
            public boolean getCopyStdlibToFrameworks()
            ```

            ::: block
            If enabled, swift-stdlib-tool will be run on .framework
            bundles, copying the Swift standard library into them. This
            is usually not what you want - it will lead to multiple
            redundant copies of the libraries being embedded in both the
            app bundle and any descendant framework bundles. Even if
            Swift is only used in a framework, and not in the app
            binary, Buck and swift-stdlib-tool will handle that
            correctly and embed the libraries.
            :::

        []{#getUseLipoThin()}

        -   #### getUseLipoThin

            ``` methodSignature
            public boolean getUseLipoThin()
            ```

            ::: block
            Uses \`lipo -thin\` instead of \`lipo -extract\` when
            copying the Swift standard libraries.
            Regardless of the value of this config flag, the resulting
            libraries are then passed to \`lipo -create\`.
            :::

        []{#getEmitSwiftdocs()}

        -   #### getEmitSwiftdocs

            ``` methodSignature
            public boolean getEmitSwiftdocs()
            ```

            ::: block
            If enabled, a .swiftdoc file will be generated along with
            the .swiftmodule file. This is necessary for Xcode to
            display the documentation for the libraries prebuilt with
            buck.
            :::
    :::
:::
:::
:::

::: bottomNav
[]{#navbar.bottom}

::: skipNav
[Skip navigation links](#skip.navbar.bottom "Skip navigation links")
:::

[]{#navbar.bottom.firstrow}

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

<div>

-   Summary: 
-   Nested \| 
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

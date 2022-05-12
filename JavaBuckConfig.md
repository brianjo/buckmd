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

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../deprecated-list.html)
-   [Index](../../../../../index-all.html)
-   [Help](../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../allclasses.html)

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
-   [Nested](#nested.class.summary) \| 
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java](package-summary.html)
:::

## Class JavaBuckConfig {#class-javabuckconfig .title title="Class JavaBuckConfig"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.JavaBuckConfig

::: description
-   

    All Implemented Interfaces:
    :   `ConfigView<BuckConfig>`

    ------------------------------------------------------------------------

        public class JavaBuckConfig
        extends Object
        implements ConfigView<BuckConfig>

    ::: block
    A java-specific \"view\" of BuckConfig.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `JavaBuckConfi        | ::: block             |
        |                       | g.DuplicatesLogLevel` | Logging level         |
        |                       |                       | duplicates are        |
        |                       |                       | reported at           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `JavaBuckConfig.Sourc |                       |
        |                       | eAbiVerificationMode` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `JavaBuckConfig.Unus  | ::: block             |
        |                       | edDependenciesAction` | An action that is     |
        |                       |                       | executed when a rule  |
        |                       |                       | that compiles Java    |
        |                       |                       | code has unused       |
        |                       |                       | dependencies.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `JavaBuckConfig.Unus  | ::: block             |
        |                       | edDependenciesConfig` | The same as           |
        |                       |                       | [`JavaBuckConfig.Unus |
        |                       |                       | edDependenciesAction` |
        |                       |                       | ](JavaBuckConfig.Unus |
        |                       |                       | edDependenciesAction. |
        |                       |                       | html "enum in com.fac |
        |                       |                       | ebook.buck.jvm.java") |
        |                       |                       | with a couple of      |
        |                       |                       | extra options to give |
        |                       |                       | greater flexibility.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type      Field                             Description
          ---------------------- --------------------------------- -------------
          `static CommandTool`   `DEFAULT_JAVA_TOOL`                
          `static String`        `PROPERTY_COMPILE_AGAINST_ABIS`    
          `static String`        `SECTION`                          

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Defa                 | `createDefaul         |                       |
        | ultJavaPackageFinder` | tJavaPackageFinder()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `AbiGenerationMode`   | `ge                   |                       |
        |                       | tAbiGenerationMode()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `get                  |                       |
        |                       | DefaultCxxPlatform()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `JavacOptions`        | `g                    |                       |
        |                       | etDefaultJavacOptions |                       |
        |                       | ​(TargetConfiguration  |                       |
        |                       | targetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `JavaOptions`         | `get                  |                       |
        |                       | DefaultJavaOptions()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `JavaOptions`         | `getDefaultJ          |                       |
        |                       | avaOptionsForTests()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuckConfig`          | `getDelegate()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Level`               | `get                  |                       |
        |                       | DuplicatesLogLevel()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `OptionalInt`         | `getDxThreadCount()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Javac                | `getJavacLa           |                       |
        | LanguageLevelOptions` | nguageLevelOptions()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `JavacSpec`           | `getJavacSpec         |                       |
        |                       | ​(TargetConfiguration  |                       |
        |                       | targetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getJavaTempDir()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `JavaBuckConfig.Sourc | `getSourceA           | ::: block             |
        | eAbiVerificationMode` | biVerificationMode()` | Controls a special    |
        |                       |                       | verification mode     |
        |                       |                       | that generates ABIs   |
        |                       |                       | both from source and  |
        |                       |                       | from class files and  |
        |                       |                       | diffs them.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.g                | `getSrcRoots()`       |                       |
        | oogle.common.collect. |                       |                       |
        | ImmutableSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `JavaBuckConfig.Unus  | `getUnused            |                       |
        | edDependenciesConfig` | DependenciesAction()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getUnusedDependenc   |                       |
        |                       | iesBuildozerString()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isUnusedDependencie  |                       |
        |                       | sOnlyPrintCommands()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `s                    | `of​(                  |                       |
        | tatic JavaBuckConfig` | BuckConfig delegate)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `s                    |                       |
        |                       | houldCacheBinaries()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `should               |                       |
        |                       | CompileAgainstAbis()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `shouldDesug          |                       |
        |                       | arInterfaceMethods()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `trackClassUsage      |                       |
        |                       | ​(TargetConfiguration  |                       |
        |                       | targetConfiguration)` |                       |
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

        []{#SECTION}

        -   #### SECTION

                public static final String SECTION

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.jvm.java.JavaBuckConfig.SECTION)

        []{#PROPERTY_COMPILE_AGAINST_ABIS}

        -   #### PROPERTY_COMPILE_AGAINST_ABIS

                public static final String PROPERTY_COMPILE_AGAINST_ABIS

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.jvm.java.JavaBuckConfig.PROPERTY_COMPILE_AGAINST_ABIS)

        []{#DEFAULT_JAVA_TOOL}

        -   #### DEFAULT_JAVA_TOOL

                public static final CommandTool DEFAULT_JAVA_TOOL
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#of(com.facebook.buck.core.config.BuckConfig)}

        -   #### of

            ``` methodSignature
            public static JavaBuckConfig of​(BuckConfig delegate)
            ```

        []{#getDelegate()}

        -   #### getDelegate

            ``` methodSignature
            public BuckConfig getDelegate()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDelegate` in interface `ConfigView<BuckConfig>`

        []{#getDefaultJavaOptions()}

        -   #### getDefaultJavaOptions

            ``` methodSignature
            public JavaOptions getDefaultJavaOptions()
            ```

        []{#getDefaultJavaOptionsForTests()}

        -   #### getDefaultJavaOptionsForTests

            ``` methodSignature
            public JavaOptions getDefaultJavaOptionsForTests()
            ```

        []{#getJavacLanguageLevelOptions()}

        -   #### getJavacLanguageLevelOptions

            ``` methodSignature
            public JavacLanguageLevelOptions getJavacLanguageLevelOptions()
            ```

        []{#getDefaultJavacOptions(com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getDefaultJavacOptions

            ``` methodSignature
            public JavacOptions getDefaultJavacOptions​(TargetConfiguration targetConfiguration)
            ```

        []{#getAbiGenerationMode()}

        -   #### getAbiGenerationMode

            ``` methodSignature
            public AbiGenerationMode getAbiGenerationMode()
            ```

        []{#getSrcRoots()}

        -   #### getSrcRoots

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<String> getSrcRoots()
            ```

        []{#createDefaultJavaPackageFinder()}

        -   #### createDefaultJavaPackageFinder

            ``` methodSignature
            public DefaultJavaPackageFinder createDefaultJavaPackageFinder()
            ```

        []{#trackClassUsage(com.facebook.buck.core.model.TargetConfiguration)}

        -   #### trackClassUsage

            ``` methodSignature
            public boolean trackClassUsage​(TargetConfiguration targetConfiguration)
            ```

        []{#shouldDesugarInterfaceMethods()}

        -   #### shouldDesugarInterfaceMethods

            ``` methodSignature
            public boolean shouldDesugarInterfaceMethods()
            ```

        []{#getJavacSpec(com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getJavacSpec

            ``` methodSignature
            public JavacSpec getJavacSpec​(TargetConfiguration targetConfiguration)
            ```

        []{#shouldCacheBinaries()}

        -   #### shouldCacheBinaries

            ``` methodSignature
            public boolean shouldCacheBinaries()
            ```

        []{#getDxThreadCount()}

        -   #### getDxThreadCount

            ``` methodSignature
            public OptionalInt getDxThreadCount()
            ```

        []{#getSourceAbiVerificationMode()}

        -   #### getSourceAbiVerificationMode

            ``` methodSignature
            public JavaBuckConfig.SourceAbiVerificationMode getSourceAbiVerificationMode()
            ```

            ::: block
            Controls a special verification mode that generates ABIs
            both from source and from class files and diffs them. This
            is a test hook for use during development of the source ABI
            feature. This only has meaning when
            [`getAbiGenerationMode()`](#getAbiGenerationMode()) is one
            of the source modes.
            :::

        []{#shouldCompileAgainstAbis()}

        -   #### shouldCompileAgainstAbis

            ``` methodSignature
            public boolean shouldCompileAgainstAbis()
            ```

        []{#getDefaultCxxPlatform()}

        -   #### getDefaultCxxPlatform

            ``` methodSignature
            public Optional<String> getDefaultCxxPlatform()
            ```

        []{#getUnusedDependenciesAction()}

        -   #### getUnusedDependenciesAction

            ``` methodSignature
            public JavaBuckConfig.UnusedDependenciesConfig getUnusedDependenciesAction()
            ```

        []{#getUnusedDependenciesBuildozerString()}

        -   #### getUnusedDependenciesBuildozerString

            ``` methodSignature
            public Optional<String> getUnusedDependenciesBuildozerString()
            ```

        []{#isUnusedDependenciesOnlyPrintCommands()}

        -   #### isUnusedDependenciesOnlyPrintCommands

            ``` methodSignature
            public boolean isUnusedDependenciesOnlyPrintCommands()
            ```

        []{#getJavaTempDir()}

        -   #### getJavaTempDir

            ``` methodSignature
            public Optional<String> getJavaTempDir()
            ```

        []{#getDuplicatesLogLevel()}

        -   #### getDuplicatesLogLevel

            ``` methodSignature
            public Level getDuplicatesLogLevel()
            ```
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

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../deprecated-list.html)
-   [Index](../../../../../index-all.html)
-   [Help](../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

<div>

-   Summary: 
-   [Nested](#nested.class.summary) \| 
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

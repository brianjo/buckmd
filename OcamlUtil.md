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
-   Nested \| 
-   Field \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.features.ocaml](package-summary.html)
:::

## Class OcamlUtil {#class-ocamlutil .title title="Class OcamlUtil"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.ocaml.OcamlUtil

::: description
-   

    ------------------------------------------------------------------------

        public class OcamlUtil
        extends Object

    ::: block
    Utility functions
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static j             | `ext​(S                | ::: block             |
        | ava.util.function.Pre | tring... extensions)` | Constructs a          |
        | dicate<? super Path>` |                       | Predicate instance    |
        |                       |                       | which returns true if |
        |                       |                       | the input argument    |
        |                       |                       | ends with any String  |
        |                       |                       | in extensions         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static com.go        | `makeArgFile          | ::: block             |
        | ogle.common.collect.I | ​(ProjectFilesystem fi | Creates an arg file   |
        | mmutableList<String>` | lesystem,             | with a given list of  |
        |                       | Path argFile,         | flags                 |
        |                       |     com.google.common | :::                   |
        |                       | .collect.ImmutableLis |                       |
        |                       | t<String> toolPrefix, |                       |
        |                       |             String fl |                       |
        |                       | ag,            Iterab |                       |
        |                       | le<String> flagList)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Path`         | `makeArgFile          | ::: block             |
        |                       | Path​(ProjectFilesyste | Creates a file path   |
        |                       | m filesystem,         | for an arg file       |
        |                       |         BuildTarget b | :::                   |
        |                       | uildTarget,           |                       |
        |                       |       String prefix)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Path`         | `makeLinkerArgF       | ::: block             |
        |                       | ilePath​(ProjectFilesy | Creates a file path   |
        |                       | stem filesystem,      | for a linker arg file |
        |                       |                  Buil | :::                   |
        |                       | dTarget buildTarget)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static java.ut       | `s                    |                       |
        | il.function.Predicate | ourcePathExt​(SourcePa |                       |
        | <? super SourcePath>` | thResolverAdapter res |                       |
        |                       | olver,              S |                       |
        |                       | tring... extensions)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#ext(java.lang.String...)}

        -   #### ext

            ``` methodSignature
            public static java.util.function.Predicate<? super Path> ext​(String... extensions)
            ```

            ::: block
            Constructs a Predicate instance which returns true if the
            input argument ends with any String in extensions
            :::

            [Parameters:]{.paramLabel}
            :   `extensions` - for which to return true

            [Returns:]{.returnLabel}
            :   a Predicate instance

        []{#sourcePathExt(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,java.lang.String...)}

        -   #### sourcePathExt

            ``` methodSignature
            public static java.util.function.Predicate<? super SourcePath> sourcePathExt​(SourcePathResolverAdapter resolver,
                                                                                         String... extensions)
            ```

        []{#makeLinkerArgFilePath(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.model.BuildTarget)}

        -   #### makeLinkerArgFilePath

            ``` methodSignature
            public static Path makeLinkerArgFilePath​(ProjectFilesystem filesystem,
                                                     BuildTarget buildTarget)
            ```

            ::: block
            Creates a file path for a linker arg file
            :::

        []{#makeArgFilePath(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.model.BuildTarget,java.lang.String)}

        -   #### makeArgFilePath

            ``` methodSignature
            public static Path makeArgFilePath​(ProjectFilesystem filesystem,
                                               BuildTarget buildTarget,
                                               String prefix)
            ```

            ::: block
            Creates a file path for an arg file
            :::

        []{#makeArgFile(com.facebook.buck.io.filesystem.ProjectFilesystem,java.nio.file.Path,com.google.common.collect.ImmutableList,java.lang.String,java.lang.Iterable)}

        -   #### makeArgFile

            ``` methodSignature
            public static com.google.common.collect.ImmutableList<String> makeArgFile​(ProjectFilesystem filesystem,
                                                                                      Path argFile,
                                                                                      com.google.common.collect.ImmutableList<String> toolPrefix,
                                                                                      String flag,
                                                                                      Iterable<String> flagList)
            ```

            ::: block
            Creates an arg file with a given list of flags
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
-   Nested \| 
-   Field \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

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
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.rules.modern](package-summary.html)
:::

## Class DefaultOutputPathResolver {#class-defaultoutputpathresolver .title title="Class DefaultOutputPathResolver"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.modern.DefaultOutputPathResolver

::: description
-   

    All Implemented Interfaces:
    :   `OutputPathResolver`

    ------------------------------------------------------------------------

        public class DefaultOutputPathResolver
        extends Object
        implements OutputPathResolver

    ::: block
    Default OutputPathResolver implementation.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                          Description
          -------------------------------------------------------------------------------------------------------------------- -------------
          `DefaultOutputPathResolver​(ProjectFilesystem projectFilesystem,                          BuildTarget buildTarget)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Path`                | `getRootPath()`       | ::: block             |
        |                       |                       | Returns a relative    |
        |                       |                       | path to the root      |
        |                       |                       | directory for build   |
        |                       |                       | outputs.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getTempPath()`       | ::: block             |
        |                       |                       | Returns a relative    |
        |                       |                       | path to the root      |
        |                       |                       | directory for         |
        |                       |                       | intermediate build    |
        |                       |                       | outputs.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `resolvePath​(Ou       | ::: block             |
        |                       | tputPath outputPath)` | Returns a relative    |
        |                       |                       | path to the output.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.rules.modern.OutputPathResolver}

            ### Methods inherited from interface com.facebook.buck.rules.modern.[OutputPathResolver](OutputPathResolver.html "interface in com.facebook.buck.rules.modern")

            `getTempPath`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.model.BuildTarget)}

        -   #### DefaultOutputPathResolver

                public DefaultOutputPathResolver​(ProjectFilesystem projectFilesystem,
                                                 BuildTarget buildTarget)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getTempPath()}

        -   #### getTempPath

            ``` methodSignature
            public Path getTempPath()
            ```

            ::: block
            [Description copied from
            interface: `OutputPathResolver`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns a relative path to the root directory for
            intermediate build outputs.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTempPath` in interface `OutputPathResolver`

        []{#resolvePath(com.facebook.buck.rules.modern.OutputPath)}

        -   #### resolvePath

            ``` methodSignature
            public Path resolvePath​(OutputPath outputPath)
            ```

            ::: block
            [Description copied from
            interface: `OutputPathResolver`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns a relative path to the output.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `resolvePath` in interface `OutputPathResolver`

        []{#getRootPath()}

        -   #### getRootPath

            ``` methodSignature
            public Path getRootPath()
            ```

            ::: block
            [Description copied from
            interface: `OutputPathResolver`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns a relative path to the root directory for build
            outputs.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRootPath` in interface `OutputPathResolver`
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
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

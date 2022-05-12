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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.toolchain.toolprovider.impl](package-summary.html)
:::

## Class ToolProviders {#class-toolproviders .title title="Class ToolProviders"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.toolchain.toolprovider.impl.ToolProviders

::: description
-   

    ------------------------------------------------------------------------

        public class ToolProviders
        extends Object

    ::: block
    Utilities for using or creating
    [`ToolProvider`](../ToolProvider.html "interface in com.facebook.buck.core.toolchain.toolprovider")
    instances.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor         Description
          ------------------- -------------
          `ToolProviders()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static ToolProvider` | `getToolProvider​(So   | ::: block             |
        |                       | urcePath sourcePath)` | Creates a             |
        |                       |                       | [`ToolProvider`       |
        |                       |                       | ](../ToolProvider.htm |
        |                       |                       | l "interface in com.f |
        |                       |                       | acebook.buck.core.too |
        |                       |                       | lchain.toolprovider") |
        |                       |                       | from a                |
        |                       |                       | [`SourcePath`](..     |
        |                       |                       | /../../sourcepath/Sou |
        |                       |                       | rcePath.html "interfa |
        |                       |                       | ce in com.facebook.bu |
        |                       |                       | ck.core.sourcepath"). |
        |                       |                       | :::                   |
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### ToolProviders

                public ToolProviders()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getToolProvider(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### getToolProvider

            ``` methodSignature
            public static ToolProvider getToolProvider​(SourcePath sourcePath)
            ```

            ::: block
            Creates a
            [`ToolProvider`](../ToolProvider.html "interface in com.facebook.buck.core.toolchain.toolprovider")
            from a
            [`SourcePath`](../../../sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath").
            A path reference will just become a
            [`HashedFileTool`](../../tool/impl/HashedFileTool.html "class in com.facebook.buck.core.toolchain.tool.impl")
            referencing that path, and a build target reference will
            require that it references a
            [`BinaryBuildRule`](../../../rules/tool/BinaryBuildRule.html "interface in com.facebook.buck.core.rules.tool")
            and use that\'s executable command.
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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
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
[Package]{.packageLabelInType} [com.facebook.buck.core.sourcepath](package-summary.html)
:::

## Class UnconfiguredSourcePath {#class-unconfiguredsourcepath .title title="Class UnconfiguredSourcePath"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.sourcepath.UnconfiguredSourcePath

::: description
-   

    Direct Known Subclasses:
    :   `UnconfiguredSourcePath.BuildTarget`,
        `UnconfiguredSourcePath.Path`

    ------------------------------------------------------------------------

        public abstract class UnconfiguredSourcePath
        extends Object

    ::: block
    Like
    [`SourcePath`](SourcePath.html "interface in com.facebook.buck.core.sourcepath")
    but when configuration is not yet available.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `UnconfiguredSo       | ::: block             |
        |                       | urcePath.BuildTarget` | [`                    |
        |                       |                       | UnconfiguredBuildTarg |
        |                       |                       | etWithOutputs`](../mo |
        |                       |                       | del/UnconfiguredBuild |
        |                       |                       | TargetWithOutputs.htm |
        |                       |                       | l "class in com.faceb |
        |                       |                       | ook.buck.core.model") |
        |                       |                       | variant of source     |
        |                       |                       | path.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static interface `   | `UnconfiguredS        | ::: block             |
        |                       | ourcePath.Matcher<R>` | Callback for          |
        |                       |                       | [`match(              |
        |                       |                       | Matcher)`](#match(com |
        |                       |                       | .facebook.buck.core.s |
        |                       |                       | ourcepath.Unconfigure |
        |                       |                       | dSourcePath.Matcher)) |
        |                       |                       | operation.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `Unconfi              | ::: block             |
        |                       | guredSourcePath.Path` | [`CellRe              |
        |                       |                       | lativePath`](../model |
        |                       |                       | /CellRelativePath.htm |
        |                       |                       | l "class in com.faceb |
        |                       |                       | ook.buck.core.model") |
        |                       |                       | variant of source     |
        |                       |                       | path.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `abstract <R> R`      | `match​(U              | ::: block             |
        |                       | nconfiguredSourcePath | Type-safe switch      |
        |                       | .Matcher<R> matcher)` | between source path   |
        |                       |                       | variants (@link       |
        |                       |                       | [`UnconfiguredSo      |
        |                       |                       | urcePath`](Unconfigur |
        |                       |                       | edSourcePath.html "cl |
        |                       |                       | ass in com.facebook.b |
        |                       |                       | uck.core.sourcepath") |
        |                       |                       | subclasses).          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#match(com.facebook.buck.core.sourcepath.UnconfiguredSourcePath.Matcher)}

        -   #### match

            ``` methodSignature
            public abstract <R> R match​(UnconfiguredSourcePath.Matcher<R> matcher)
            ```

            ::: block
            Type-safe switch between source path variants (@link
            [`UnconfiguredSourcePath`](UnconfiguredSourcePath.html "class in com.facebook.buck.core.sourcepath")
            subclasses).
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
-   [Nested](#nested.class.summary) \| 
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

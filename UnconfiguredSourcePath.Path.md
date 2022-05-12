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
[Package]{.packageLabelInType} [com.facebook.buck.core.sourcepath](package-summary.html)
:::

## Class UnconfiguredSourcePath.Path {#class-unconfiguredsourcepath.path .title title="Class UnconfiguredSourcePath.Path"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.sourcepath.UnconfiguredSourcePath](UnconfiguredSourcePath.html "class in com.facebook.buck.core.sourcepath")

    -   -   com.facebook.buck.core.sourcepath.UnconfiguredSourcePath.Path

::: description
-   

    Enclosing class:
    :   [UnconfiguredSourcePath](UnconfiguredSourcePath.html "class in com.facebook.buck.core.sourcepath")

    ------------------------------------------------------------------------

        public static class UnconfiguredSourcePath.Path
        extends UnconfiguredSourcePath

    ::: block
    [`CellRelativePath`](../model/CellRelativePath.html "class in com.facebook.buck.core.model")
    variant of source path.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.core.sourcepath.UnconfiguredSourcePath}

            ### Nested classes/interfaces inherited from class com.facebook.buck.core.sourcepath.[UnconfiguredSourcePath](UnconfiguredSourcePath.html "class in com.facebook.buck.core.sourcepath")

            `UnconfiguredSourcePath.BuildTarget, UnconfiguredSourcePath.Matcher<R>, UnconfiguredSourcePath.Path`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                     Description
          ------------------------------- -------------
          `Path​(CellRelativePath path)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `boolean`             | `equals​(Object o)`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `<R> R`               | `match​(U              | ::: block             |
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
        | `String`              | `toString()`          |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.CellRelativePath)}

        -   #### Path

                public Path​(CellRelativePath path)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#match(com.facebook.buck.core.sourcepath.UnconfiguredSourcePath.Matcher)}

        -   #### match

            ``` methodSignature
            public <R> R match​(UnconfiguredSourcePath.Matcher<R> matcher)
            ```

            ::: block
            [Description copied from
            class: `UnconfiguredSourcePath`]{.descfrmTypeLabel}
            :::

            ::: block
            Type-safe switch between source path variants (@link
            [`UnconfiguredSourcePath`](UnconfiguredSourcePath.html "class in com.facebook.buck.core.sourcepath")
            subclasses).
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `match` in class `UnconfiguredSourcePath`

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(Object o)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `Object`

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `Object`

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`
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

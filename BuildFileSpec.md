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
[Package]{.packageLabelInType} [com.facebook.buck.parser.spec](package-summary.html)
:::

## Class BuildFileSpec {#class-buildfilespec .title title="Class BuildFileSpec"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.parser.spec.BuildFileSpec

::: description
-   

    ------------------------------------------------------------------------

        public abstract class BuildFileSpec
        extends Object

    ::: block
    A specification used by the parser, via
    [`TargetNodeSpec`](TargetNodeSpec.html "interface in com.facebook.buck.parser.spec"),
    to match build files.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor         Description
          ------------------- -------------
          `BuildFileSpec()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `                     | `fr                   | ::: block             |
        | static BuildFileSpec` | omPath​(CellRelativePa | Create a              |
        |                       | th cellRelativePath)` | [`BuildFileSpec       |
        |                       |                       | `](BuildFileSpec.html |
        |                       |                       |  "class in com.facebo |
        |                       |                       | ok.buck.parser.spec") |
        |                       |                       | for a package build   |
        |                       |                       | target pattern like   |
        |                       |                       | foo/bar: or           |
        |                       |                       | foo/bar:baz           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `fromRecursi          | ::: block             |
        | static BuildFileSpec` | vePath​(CellRelativePa | Create a              |
        |                       | th cellRelativePath)` | [`BuildFileSpec       |
        |                       |                       | `](BuildFileSpec.html |
        |                       |                       |  "class in com.facebo |
        |                       |                       | ok.buck.parser.spec") |
        |                       |                       | for a recursive build |
        |                       |                       | target pattern like   |
        |                       |                       | foo/bar/\...          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `fromUnconfiguredBu   |                       |
        | static BuildFileSpec` | ildTarget​(Unconfigure |                       |
        |                       | dBuildTarget target)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstr                | `getCe                |                       |
        | act CellRelativePath` | llRelativeBaseName()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract boolean`    | `isRecursive()`       |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
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

        -   #### BuildFileSpec

                public BuildFileSpec()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getCellRelativeBaseName()}

        -   #### getCellRelativeBaseName

            ``` methodSignature
            public abstract CellRelativePath getCellRelativeBaseName()
            ```

        []{#isRecursive()}

        -   #### isRecursive

            ``` methodSignature
            public abstract boolean isRecursive()
            ```

        []{#fromRecursivePath(com.facebook.buck.core.model.CellRelativePath)}

        -   #### fromRecursivePath

            ``` methodSignature
            public static BuildFileSpec fromRecursivePath​(CellRelativePath cellRelativePath)
            ```

            ::: block
            Create a
            [`BuildFileSpec`](BuildFileSpec.html "class in com.facebook.buck.parser.spec")
            for a recursive build target pattern like foo/bar/\...
            :::

            [Returns:]{.returnLabel}
            :   a new
                [`BuildFileSpec`](BuildFileSpec.html "class in com.facebook.buck.parser.spec")
                with [`isRecursive()`](#isRecursive())} set to `true`

        []{#fromPath(com.facebook.buck.core.model.CellRelativePath)}

        -   #### fromPath

            ``` methodSignature
            public static BuildFileSpec fromPath​(CellRelativePath cellRelativePath)
            ```

            ::: block
            Create a
            [`BuildFileSpec`](BuildFileSpec.html "class in com.facebook.buck.parser.spec")
            for a package build target pattern like foo/bar: or
            foo/bar:baz
            :::

            [Returns:]{.returnLabel}
            :   a new
                [`BuildFileSpec`](BuildFileSpec.html "class in com.facebook.buck.parser.spec")
                with [`isRecursive()`](#isRecursive())} set to `false`

        []{#fromUnconfiguredBuildTarget(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### fromUnconfiguredBuildTarget

            ``` methodSignature
            public static BuildFileSpec fromUnconfiguredBuildTarget​(UnconfiguredBuildTarget target)
            ```

            [Returns:]{.returnLabel}
            :   a
                [`BuildFileSpec`](BuildFileSpec.html "class in com.facebook.buck.parser.spec")
                for a specific build target like //foo/bar:baz
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

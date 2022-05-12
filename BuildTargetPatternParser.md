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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.parser.buildtargetpattern](package-summary.html)
:::

## Class BuildTargetPatternParser {#class-buildtargetpatternparser .title title="Class BuildTargetPatternParser"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.parser.buildtargetpattern.BuildTargetPatternParser

::: description
-   

    ------------------------------------------------------------------------

        public class BuildTargetPatternParser
        extends Object

    ::: block
    Factory that parses a string into
    [`BuildTargetPattern`](BuildTargetPattern.html "class in com.facebook.buck.core.parser.buildtargetpattern")
    Pattern may be one of following formats:

    -   Single build target: cell//path/package:target or
        cell//path/package, in which case target name is assumed to be
        the same as package name
    -   All build targets from some package: cell//path/package:
    -   All build targets from some package and all packages down folder
        tree: cell//path/package/\...

    Cell component may be omitted in which case pattern will be
    evaluated in the context of executing or owning cell
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `stati                | `parse​(String pattern | ::: block             |
        | c BuildTargetPattern` | ,      CellNameResolv | Parse a string        |
        |                       | er cellNameResolver)` | representing build    |
        |                       |                       | target pattern        |
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
    -   []{#method.detail}

        ### Method Detail

        []{#parse(java.lang.String,com.facebook.buck.core.cell.nameresolver.CellNameResolver)}

        -   #### parse

            ``` methodSignature
            public static BuildTargetPattern parse​(String pattern,
                                                   CellNameResolver cellNameResolver)
                                            throws BuildTargetParseException
            ```

            ::: block
            Parse a string representing build target pattern
            :::

            [Parameters:]{.paramLabel}
            :   `pattern` - String representing build target pattern,
                for example \"//\...\"

            [Throws:]{.throwsLabel}
            :   `BuildTargetParseException` - If build target pattern is
                invalid; at this moment
                [`BuildTargetParseException`](../../exceptions/BuildTargetParseException.html "class in com.facebook.buck.core.exceptions")
                is unchecked exception but we still want to declare it
                with the hope to make it checked one day; this type of
                exception would be properly handled as user error
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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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

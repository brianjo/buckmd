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

## Class UnconfiguredBuildTargetParser {#class-unconfiguredbuildtargetparser .title title="Class UnconfiguredBuildTargetParser"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.parser.buildtargetpattern.UnconfiguredBuildTargetParser

::: description
-   

    ------------------------------------------------------------------------

        public class UnconfiguredBuildTargetParser
        extends Object

    ::: block
    Factory that parses a string into
    [`UnconfiguredBuildTarget`](../../model/UnconfiguredBuildTarget.html "class in com.facebook.buck.core.model").
    Fully qualified build target name looks like
    \`cell//path/to:target#flavor1,flavor2\`, where \`cell\` and
    \`path/to\` components is allowed to be empty, and flavors may not
    be specified along with \`#\` sign. So a minimum valid build target
    string is \`//:target\` indicating a target named \`target\` at the
    package on the root path of the default cell without flavors
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static Unc           | `                     | ::: block             |
        | onfiguredBuildTarget` | parse​(String target)` | Parse a string        |
        |                       |                       | representing fully    |
        |                       |                       | qualified build       |
        |                       |                       | target, validating    |
        |                       |                       | build target format   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Unc           | `                     | ::: block             |
        | onfiguredBuildTarget` | parse​(String target,  | Parse a string        |
        |                       |      boolean intern)` | representing fully    |
        |                       |                       | qualified build       |
        |                       |                       | target, validating    |
        |                       |                       | build target format   |
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

        []{#parse(java.lang.String)}

        -   #### parse

            ``` methodSignature
            public static UnconfiguredBuildTarget parse​(String target)
                                                 throws BuildTargetParseException
            ```

            ::: block
            Parse a string representing fully qualified build target,
            validating build target format
            Fully qualified build target format is
            \`cell//path/to:target#flavor1,flavor2\` where cell may be
            an empty string, and flavors may be omitted along with \`#\`
            sign

            The target must be in canonical form. Importantly, the cell
            name must be the canonical name.
            :::

            [Parameters:]{.paramLabel}
            :   `target` - String representing fully-qualified build
                target, for example \"//foo/bar:bar\"

            [Throws:]{.throwsLabel}
            :   `BuildTargetParseException` - If build target format is
                invalid; at this moment
                [`BuildTargetParseException`](../../exceptions/BuildTargetParseException.html "class in com.facebook.buck.core.exceptions")
                is unchecked exception but we still want to declare it
                with the hope to make it checked one day; this type of
                exception would be properly handled as user error

        []{#parse(java.lang.String,boolean)}

        -   #### parse

            ``` methodSignature
            public static UnconfiguredBuildTarget parse​(String target,
                                                        boolean intern)
                                                 throws BuildTargetParseException
            ```

            ::: block
            Parse a string representing fully qualified build target,
            validating build target format
            Fully qualified build target format is
            \`cell//path/to:target#flavor1,flavor2\` where cell may be
            an empty string, and flavors may be omitted along with \`#\`
            sign

            The target must be in canonical form. Importantly, the cell
            name must be the canonical name.
            :::

            [Parameters:]{.paramLabel}
            :   `target` - String representing fully-qualified build
                target, for example \"//foo/bar:bar\"
            :   `intern` - Whether to intern parsed instance; once
                interned the instance stays in memory forever but
                subsequent hash map/set operations are faster because
                [`Object.equals(Object)`](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true#equals(java.lang.Object) "class or interface in java.lang"){.externalLink}
                is cheap

            [Throws:]{.throwsLabel}
            :   `BuildTargetParseException` - If build target format is
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

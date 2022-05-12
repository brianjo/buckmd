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
[Package]{.packageLabelInType} [com.facebook.buck.core.test.rule.coercer](package-summary.html)
:::

## Class TestRunnerSpecCoercer {#class-testrunnerspeccoercer .title title="Class TestRunnerSpecCoercer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.test.rule.coercer.TestRunnerSpecCoercer

::: description
-   

    ------------------------------------------------------------------------

        public class TestRunnerSpecCoercer
        extends Object

    ::: block
    Coerces a
    [`TestRunnerSpec`](../TestRunnerSpec.html "class in com.facebook.buck.core.test.rule")
    to a
    [`CoercedTestRunnerSpec`](../CoercedTestRunnerSpec.html "class in com.facebook.buck.core.test.rule")
    by resolving the
    [`StringWithMacros`](../../../../rules/macros/StringWithMacros.html "class in com.facebook.buck.rules.macros")
    to
    [`Arg`](../../../../rules/args/Arg.html "interface in com.facebook.buck.rules.args")s.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static C             | `coerce​(T             | ::: block             |
        | oercedTestRunnerSpec` | estRunnerSpec spec,   | Coerces the given     |
        |                       |      StringWithMacros | freeform JSON with    |
        |                       | Converter converter)` | [`Str                 |
        |                       |                       | ingWithMacros`](../.. |
        |                       |                       | /../../rules/macros/S |
        |                       |                       | tringWithMacros.html  |
        |                       |                       | "class in com.faceboo |
        |                       |                       | k.buck.rules.macros") |
        |                       |                       | in the                |
        |                       |                       | [`                    |
        |                       |                       | TestRunnerSpec`](../T |
        |                       |                       | estRunnerSpec.html "c |
        |                       |                       | lass in com.facebook. |
        |                       |                       | buck.core.test.rule") |
        |                       |                       | to become a freeform  |
        |                       |                       | JSON of               |
        |                       |                       | [`                    |
        |                       |                       | Arg`](../../../../rul |
        |                       |                       | es/args/Arg.html "int |
        |                       |                       | erface in com.faceboo |
        |                       |                       | k.buck.rules.args")s, |
        |                       |                       | contained in          |
        |                       |                       | [`CoercedTestRunn     |
        |                       |                       | erSpec`](../CoercedTe |
        |                       |                       | stRunnerSpec.html "cl |
        |                       |                       | ass in com.facebook.b |
        |                       |                       | uck.core.test.rule"). |
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

        []{#coerce(com.facebook.buck.core.test.rule.TestRunnerSpec,com.facebook.buck.rules.macros.StringWithMacrosConverter)}

        -   #### coerce

            ``` methodSignature
            public static CoercedTestRunnerSpec coerce​(TestRunnerSpec spec,
                                                       StringWithMacrosConverter converter)
            ```

            ::: block
            Coerces the given freeform JSON with
            [`StringWithMacros`](../../../../rules/macros/StringWithMacros.html "class in com.facebook.buck.rules.macros")
            in the
            [`TestRunnerSpec`](../TestRunnerSpec.html "class in com.facebook.buck.core.test.rule")
            to become a freeform JSON of
            [`Arg`](../../../../rules/args/Arg.html "interface in com.facebook.buck.rules.args")s,
            contained in
            [`CoercedTestRunnerSpec`](../CoercedTestRunnerSpec.html "class in com.facebook.buck.core.test.rule").
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

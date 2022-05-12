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
[Package]{.packageLabelInType} [com.facebook.buck.core.test.rule](package-summary.html)
:::

## Class CoercedTestRunnerSpec {#class-coercedtestrunnerspec .title title="Class CoercedTestRunnerSpec"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.test.rule.CoercedTestRunnerSpec

::: description
-   

    ------------------------------------------------------------------------

        public abstract class CoercedTestRunnerSpec
        extends Object

    ::: block
    The freeform JSON test protocol specification. This has the
    [`StringWithMacros`](../../../rules/macros/StringWithMacros.html "class in com.facebook.buck.rules.macros")
    from
    [`TestRunnerSpec`](TestRunnerSpec.html "class in com.facebook.buck.core.test.rule")
    resolved to
    [`Arg`](../../../rules/args/Arg.html "interface in com.facebook.buck.rules.args")s.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                 Description
          --------------------------- -------------
          `CoercedTestRunnerSpec()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `protected void`      | `check()`             |                       |
        +-----------------------+-----------------------+-----------------------+
        | `prote                | `getData()`           |                       |
        | cted abstract Object` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static C             | `of​(Object data)`     |                       |
        | oercedTestRunnerSpec` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `se                   | ::: block             |
        |                       | rialize​(com.fasterxml | Serializes the        |
        |                       | .jackson.core.JsonGen | underlying freeform   |
        |                       | erator jsonGenerator, | JSON of               |
        |                       |           SourcePathR | [`Arg`](../../../rul  |
        |                       | esolverAdapter source | es/args/Arg.html "int |
        |                       | PathResolverAdapter)` | erface in com.faceboo |
        |                       |                       | k.buck.rules.args")s. |
        |                       |                       | :::                   |
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

        -   #### CoercedTestRunnerSpec

                public CoercedTestRunnerSpec()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#of(java.lang.Object)}

        -   #### of

            ``` methodSignature
            public static CoercedTestRunnerSpec of​(Object data)
            ```

        []{#getData()}

        -   #### getData

            ``` methodSignature
            protected abstract Object getData()
            ```

        []{#check()}

        -   #### check

            ``` methodSignature
            @Check
            protected void check()
            ```

        []{#serialize(com.fasterxml.jackson.core.JsonGenerator,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### serialize

            ``` methodSignature
            public void serialize​(com.fasterxml.jackson.core.JsonGenerator jsonGenerator,
                                  SourcePathResolverAdapter sourcePathResolverAdapter)
                           throws IOException
            ```

            ::: block
            Serializes the underlying freeform JSON of
            [`Arg`](../../../rules/args/Arg.html "interface in com.facebook.buck.rules.args")s.
            :::

            [Parameters:]{.paramLabel}
            :   `jsonGenerator` - the json writer
            :   `sourcePathResolverAdapter` - the rule resolver for
                resolving
                [`Arg`](../../../rules/args/Arg.html "interface in com.facebook.buck.rules.args")s

            [Throws:]{.throwsLabel}
            :   `IOException`
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

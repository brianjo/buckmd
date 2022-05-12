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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.skylark.function](package-summary.html)
:::

## Class SkylarkRuleFunctions {#class-skylarkrulefunctions .title title="Class SkylarkRuleFunctions"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.skylark.function.SkylarkRuleFunctions

::: description
-   

    All Implemented Interfaces:
    :   `SkylarkRuleFunctionsApi`

    ------------------------------------------------------------------------

        public class SkylarkRuleFunctions
        extends Object
        implements SkylarkRuleFunctionsApi

    ::: block
    Provides APIs for creating build rules.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Field                 | Description           |
        +=======================+=======================+=======================+
        | `static Set<String>`  | `HIDDEN               | ::: block             |
        |                       | _IMPLICIT_ATTRIBUTES` | The hidden attributes |
        |                       |                       | from                  |
        |                       |                       | IMPLICIT_ATTRIBUTES   |
        |                       |                       | that are hidden from  |
        |                       |                       | user\'s for user      |
        |                       |                       | defined rules         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `stat                 | `IMPLICIT_ATTRIBUTES` | ::: block             |
        | ic com.google.common. |                       | The attributes that   |
        | collect.ImmutableMap< |                       | are applicable to all |
        | String,​Attribute<?>>` |                       | rules.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `stat                 | `IMPL                 |                       |
        | ic com.google.common. | ICIT_TEST_ATTRIBUTES` |                       |
        | collect.ImmutableMap< |                       |                       |
        | String,​Attribute<?>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+

        : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                   Description
          ----------------------------------------------------------------------------------------------------------------------------- -------------
          `SkylarkRuleFunctions​(com.google.common.cache.LoadingCache<String,​com.google.devtools.build.lib.cmdline.Label> labelCache)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                               Method                                                                                                                                                                                                                                                                                                                                                                                      Description
          ----------------------------------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `com.google.devtools.build.lib.cmdline.Label`   `label​(String labelString,      com.google.devtools.build.lib.events.Location loc,      com.google.devtools.build.lib.syntax.Environment env,      com.google.devtools.build.lib.skylarkinterface.StarlarkContext context)`                                                                                                                                                                  
          `UserDefinedProvider`                           `provider​(String doc,         Object fields,         com.google.devtools.build.lib.events.Location location)`                                                                                                                                                                                                                                                                                
          `SkylarkUserDefinedRule`                        `rule​(com.google.devtools.build.lib.syntax.BaseFunction implementation,     com.google.devtools.build.lib.syntax.SkylarkDict<String,​AttributeHolder> attrs,     boolean inferRunInfo,     boolean test,     com.google.devtools.build.lib.events.Location loc,     com.google.devtools.build.lib.syntax.FuncallExpression ast,     com.google.devtools.build.lib.syntax.Environment env)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#IMPLICIT_ATTRIBUTES}

        -   #### IMPLICIT_ATTRIBUTES

                public static final com.google.common.collect.ImmutableMap<String,​Attribute<?>> IMPLICIT_ATTRIBUTES

            ::: block
            The attributes that are applicable to all rules. This will
            expand over time.
            :::

        []{#IMPLICIT_TEST_ATTRIBUTES}

        -   #### IMPLICIT_TEST_ATTRIBUTES

                public static final com.google.common.collect.ImmutableMap<String,​Attribute<?>> IMPLICIT_TEST_ATTRIBUTES

        []{#HIDDEN_IMPLICIT_ATTRIBUTES}

        -   #### HIDDEN_IMPLICIT_ATTRIBUTES

                public static final Set<String> HIDDEN_IMPLICIT_ATTRIBUTES

            ::: block
            The hidden attributes from IMPLICIT_ATTRIBUTES that are
            hidden from user\'s for user defined rules
            :::
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.google.common.cache.LoadingCache)}

        -   #### SkylarkRuleFunctions

                public SkylarkRuleFunctions​(com.google.common.cache.LoadingCache<String,​com.google.devtools.build.lib.cmdline.Label> labelCache)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#label(java.lang.String,com.google.devtools.build.lib.events.Location,com.google.devtools.build.lib.syntax.Environment,com.google.devtools.build.lib.skylarkinterface.StarlarkContext)}

        -   #### label

            ``` methodSignature
            public com.google.devtools.build.lib.cmdline.Label label​(String labelString,
                                                                     com.google.devtools.build.lib.events.Location loc,
                                                                     com.google.devtools.build.lib.syntax.Environment env,
                                                                     com.google.devtools.build.lib.skylarkinterface.StarlarkContext context)
                                                              throws com.google.devtools.build.lib.syntax.EvalException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `label` in interface `SkylarkRuleFunctionsApi`

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`

        []{#rule(com.google.devtools.build.lib.syntax.BaseFunction,com.google.devtools.build.lib.syntax.SkylarkDict,boolean,boolean,com.google.devtools.build.lib.events.Location,com.google.devtools.build.lib.syntax.FuncallExpression,com.google.devtools.build.lib.syntax.Environment)}

        -   #### rule

            ``` methodSignature
            public SkylarkUserDefinedRule rule​(com.google.devtools.build.lib.syntax.BaseFunction implementation,
                                               com.google.devtools.build.lib.syntax.SkylarkDict<String,​AttributeHolder> attrs,
                                               boolean inferRunInfo,
                                               boolean test,
                                               com.google.devtools.build.lib.events.Location loc,
                                               com.google.devtools.build.lib.syntax.FuncallExpression ast,
                                               com.google.devtools.build.lib.syntax.Environment env)
                                        throws com.google.devtools.build.lib.syntax.EvalException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `rule` in interface `SkylarkRuleFunctionsApi`

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`

        []{#provider(java.lang.String,java.lang.Object,com.google.devtools.build.lib.events.Location)}

        -   #### provider

            ``` methodSignature
            public UserDefinedProvider provider​(String doc,
                                                Object fields,
                                                com.google.devtools.build.lib.events.Location location)
                                         throws com.google.devtools.build.lib.syntax.EvalException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `provider` in interface `SkylarkRuleFunctionsApi`

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`
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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

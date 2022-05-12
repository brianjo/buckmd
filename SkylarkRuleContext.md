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
[Package]{.packageLabelInType} [com.facebook.buck.core.starlark.rule](package-summary.html)
:::

## Class SkylarkRuleContext {#class-skylarkrulecontext .title title="Class SkylarkRuleContext"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.starlark.rule.SkylarkRuleContext

::: description
-   

    All Implemented Interfaces:
    :   `com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable`,
        `com.google.devtools.build.lib.skylarkinterface.SkylarkValue`

    ------------------------------------------------------------------------

        public class SkylarkRuleContext
        extends Object

    ::: block
    The context passed to user defined rules\' implementation functions
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `SkylarkRuleContex                | ::: block                         |
        | t​(RuleAnalysisContext context,    | Create a                          |
        |                 com.google.devtoo | [`SkylarkRuleContext`](Skylar     |
        | ls.build.lib.cmdline.Label label, | kRuleContext.html "class in com.f |
        |                    SkylarkRuleCon | acebook.buck.core.starlark.rule") |
        | textAttr skylarkRuleContextAttr)` | to be used in users\'             |
        |                                   | implementation functions          |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+

        : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                               Method                                                                          Description
          ----------------------------------------------- ------------------------------------------------------------------------------- -------------
          `SkylarkRuleContextActionsApi`                  `getActions()`                                                                   
          `SkylarkRuleContextAttr`                        `getAttr()`                                                                      
          `com.google.devtools.build.lib.cmdline.Label`   `getLabel()`                                                                     
          `void`                                          `repr​(com.google.devtools.build.lib.skylarkinterface.SkylarkPrinter printer)`    

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
        -   []{#methods.inherited.from.class.com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable}

            ### Methods inherited from interface com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable

            `debugPrint, str`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.google.devtools.build.lib.skylarkinterface.SkylarkValue}

            ### Methods inherited from interface com.google.devtools.build.lib.skylarkinterface.SkylarkValue

            `isHashable, isImmutable`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.rules.analysis.RuleAnalysisContext,com.google.devtools.build.lib.cmdline.Label,com.facebook.buck.core.starlark.rule.SkylarkRuleContextAttr)}

        -   #### SkylarkRuleContext

                public SkylarkRuleContext​(RuleAnalysisContext context,
                                          com.google.devtools.build.lib.cmdline.Label label,
                                          SkylarkRuleContextAttr skylarkRuleContextAttr)

            ::: block
            Create a
            [`SkylarkRuleContext`](SkylarkRuleContext.html "class in com.facebook.buck.core.starlark.rule")
            to be used in users\' implementation functions
            :::

            [Parameters:]{.paramLabel}
            :   `context` - the context for the analysing this rule.
                Used primarily for creating and manipulating actions
            :   `label` - the label of the new rule being evaluated
            :   `skylarkRuleContextAttr` - a mapping-like representation
                of field names to coerced-transformed values for a given
                rule
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#repr(com.google.devtools.build.lib.skylarkinterface.SkylarkPrinter)}

        -   #### repr

            ``` methodSignature
            public void repr​(com.google.devtools.build.lib.skylarkinterface.SkylarkPrinter printer)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `repr` in
                interface `com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable`

        []{#getAttr()}

        -   #### getAttr

            ``` methodSignature
            public SkylarkRuleContextAttr getAttr()
            ```

        []{#getLabel()}

        -   #### getLabel

            ``` methodSignature
            public com.google.devtools.build.lib.cmdline.Label getLabel()
            ```

        []{#getActions()}

        -   #### getActions

            ``` methodSignature
            public SkylarkRuleContextActionsApi getActions()
            ```
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

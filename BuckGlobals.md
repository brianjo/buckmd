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
[Package]{.packageLabelInType} [com.facebook.buck.skylark.parser](package-summary.html)
:::

## Class BuckGlobals {#class-buckglobals .title title="Class BuckGlobals"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.skylark.parser.BuckGlobals

::: description
-   

    ------------------------------------------------------------------------

        public abstract class BuckGlobals
        extends Object

    ::: block
    Provides access to global Skylark interpreter frames.
    It\'s recommended to use global frames for all globally accessible
    variables for improved performance and easier maintenance, since
    there is only one place to check for variable definitions.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor       Description
          ----------------- -------------
          `BuckGlobals()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.goo              | `getNativeModule()`   | ::: block             |
        | gle.devtools.build.li |                       | Returns a native      |
        | b.syntax.ClassObject` |                       | module with built-in  |
        |                       |                       | functions and Buck    |
        |                       |                       | rules.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static BuckGlobals`  | `of                   | ::: block             |
        |                       | ​(SkylarkFunctionModul | Create an instance of |
        |                       | e skylarkFunctionModu | [`BuckGlobals`        |
        |                       | le,   com.google.comm | ](BuckGlobals.html "c |
        |                       | on.collect.ImmutableS | lass in com.facebook. |
        |                       | et<BaseDescription<?> | buck.skylark.parser") |
        |                       | > descriptions,   Use | :::                   |
        |                       | rDefinedRulesState us |                       |
        |                       | erDefinedRulesState,  |                       |
        |                       |   ImplicitNativeRules |                       |
        |                       | State implicitNativeR |                       |
        |                       | ulesState,   RuleFunc |                       |
        |                       | tionFactory ruleFunct |                       |
        |                       | ionFactory,   com.goo |                       |
        |                       | gle.common.cache.Load |                       |
        |                       | ingCache<String,​com.g |                       |
        |                       | oogle.devtools.build. |                       |
        |                       | lib.cmdline.Label> la |                       |
        |                       | belCache,   KnownUser |                       |
        |                       | DefinedRuleTypes know |                       |
        |                       | nUserDefinedRuleTypes |                       |
        |                       | ,   com.google.common |                       |
        |                       | .collect.ImmutableSet |                       |
        |                       | <BuiltInProvider<?>>  |                       |
        |                       | perFeatureProviders)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### BuckGlobals

                public BuckGlobals()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getNativeModule()}

        -   #### getNativeModule

            ``` methodSignature
            @Lazy
            public com.google.devtools.build.lib.syntax.ClassObject getNativeModule()
            ```

            ::: block
            Returns a native module with built-in functions and Buck
            rules.
            It\'s the module that handles method calls like
            `native.glob` or `  native.cxx_library`.
            :::

        []{#of(com.facebook.buck.skylark.function.SkylarkFunctionModule,com.google.common.collect.ImmutableSet,com.facebook.buck.parser.options.UserDefinedRulesState,com.facebook.buck.parser.options.ImplicitNativeRulesState,com.facebook.buck.skylark.parser.RuleFunctionFactory,com.google.common.cache.LoadingCache,com.facebook.buck.core.starlark.knowntypes.KnownUserDefinedRuleTypes,com.google.common.collect.ImmutableSet)}

        -   #### of

            ``` methodSignature
            public static BuckGlobals of​(SkylarkFunctionModule skylarkFunctionModule,
                                         com.google.common.collect.ImmutableSet<BaseDescription<?>> descriptions,
                                         UserDefinedRulesState userDefinedRulesState,
                                         ImplicitNativeRulesState implicitNativeRulesState,
                                         RuleFunctionFactory ruleFunctionFactory,
                                         com.google.common.cache.LoadingCache<String,​com.google.devtools.build.lib.cmdline.Label> labelCache,
                                         KnownUserDefinedRuleTypes knownUserDefinedRuleTypes,
                                         com.google.common.collect.ImmutableSet<BuiltInProvider<?>> perFeatureProviders)
            ```

            ::: block
            Create an instance of
            [`BuckGlobals`](BuckGlobals.html "class in com.facebook.buck.skylark.parser")
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

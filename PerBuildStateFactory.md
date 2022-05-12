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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.parser](package-summary.html)
:::

## Class PerBuildStateFactory {#class-perbuildstatefactory .title title="Class PerBuildStateFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.parser.PerBuildStateFactory

::: description
-   

    ------------------------------------------------------------------------

        public class PerBuildStateFactory
        extends Object

    ::: block
    Can be used to create
    [`PerBuildState`](PerBuildState.html "class in com.facebook.buck.parser").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          Description
          -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `PerBuildStateFactory​(TypeCoercerFactory typeCoercerFactory,                     ConstructorArgMarshaller marshaller,                     KnownRuleTypesProvider knownRuleTypesProvider,                     ParserPythonInterpreterProvider parserPythonInterpreterProvider,                     Watchman watchman,                     BuckEventBus eventBus,                     UnconfiguredBuildTargetViewFactory unconfiguredBuildTargetFactory,                     TargetConfiguration hostConfiguration)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                                                    Description
          ------------------- ------------------------------------------------------------------------------------------------------------------------- -------------
          `PerBuildState`     `create​(ParsingContext parsingContext,       DaemonicParserState daemonicParserState)`                                     
          `PerBuildState`     `create​(ParsingContext parsingContext,       DaemonicParserState daemonicParserState,       AtomicLong processedBytes)`    

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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.rules.coercer.TypeCoercerFactory,com.facebook.buck.rules.coercer.ConstructorArgMarshaller,com.facebook.buck.core.rules.knowntypes.provider.KnownRuleTypesProvider,com.facebook.buck.parser.ParserPythonInterpreterProvider,com.facebook.buck.io.watchman.Watchman,com.facebook.buck.event.BuckEventBus,com.facebook.buck.core.parser.buildtargetparser.UnconfiguredBuildTargetViewFactory,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### PerBuildStateFactory

                public PerBuildStateFactory​(TypeCoercerFactory typeCoercerFactory,
                                            ConstructorArgMarshaller marshaller,
                                            KnownRuleTypesProvider knownRuleTypesProvider,
                                            ParserPythonInterpreterProvider parserPythonInterpreterProvider,
                                            Watchman watchman,
                                            BuckEventBus eventBus,
                                            UnconfiguredBuildTargetViewFactory unconfiguredBuildTargetFactory,
                                            TargetConfiguration hostConfiguration)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#create(com.facebook.buck.parser.ParsingContext,com.facebook.buck.parser.DaemonicParserState)}

        -   #### create

            ``` methodSignature
            public PerBuildState create​(ParsingContext parsingContext,
                                        DaemonicParserState daemonicParserState)
            ```

        []{#create(com.facebook.buck.parser.ParsingContext,com.facebook.buck.parser.DaemonicParserState,java.util.concurrent.atomic.AtomicLong)}

        -   #### create

            ``` methodSignature
            public PerBuildState create​(ParsingContext parsingContext,
                                        DaemonicParserState daemonicParserState,
                                        AtomicLong processedBytes)
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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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

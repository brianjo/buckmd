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

## Class ParserFactory {#class-parserfactory .title title="Class ParserFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.parser.ParserFactory

::: description
-   

    ------------------------------------------------------------------------

        public class ParserFactory
        extends Object

    ::: block
    Responsible for creating an instance of
    [`Parser`](Parser.html "interface in com.facebook.buck.parser").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor         Description
          ------------------- -------------
          `ParserFactory()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static Parser`       | `create​(TypeCoercerF  | ::: block             |
        |                       | actory typeCoercerFac | Creates an instance   |
        |                       | tory,       Construct | of                    |
        |                       | orArgMarshaller marsh | [                     |
        |                       | aller,       KnownRul | `Parser`](Parser.html |
        |                       | eTypesProvider knownR |  "interface in com.fa |
        |                       | uleTypesProvider,     | cebook.buck.parser"). |
        |                       |    ParserPythonInterp | :::                   |
        |                       | reterProvider parserP |                       |
        |                       | ythonInterpreterProvi |                       |
        |                       | der,       DaemonicPa |                       |
        |                       | rserState daemonicPar |                       |
        |                       | serState,       Targe |                       |
        |                       | tSpecResolver targetS |                       |
        |                       | pecResolver,       Wa |                       |
        |                       | tchman watchman,      |                       |
        |                       |   BuckEventBus eventB |                       |
        |                       | us,       Unconfigure |                       |
        |                       | dBuildTargetViewFacto |                       |
        |                       | ry unconfiguredBuildT |                       |
        |                       | argetFactory,       T |                       |
        |                       | argetConfiguration ho |                       |
        |                       | stConfiguration,      |                       |
        |                       |   boolean buckOutIncl |                       |
        |                       | udeTargetConfigHash)` |                       |
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### ParserFactory

                public ParserFactory()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#create(com.facebook.buck.rules.coercer.TypeCoercerFactory,com.facebook.buck.rules.coercer.ConstructorArgMarshaller,com.facebook.buck.core.rules.knowntypes.provider.KnownRuleTypesProvider,com.facebook.buck.parser.ParserPythonInterpreterProvider,com.facebook.buck.parser.DaemonicParserState,com.facebook.buck.parser.TargetSpecResolver,com.facebook.buck.io.watchman.Watchman,com.facebook.buck.event.BuckEventBus,com.facebook.buck.core.parser.buildtargetparser.UnconfiguredBuildTargetViewFactory,com.facebook.buck.core.model.TargetConfiguration,boolean)}

        -   #### create

            ``` methodSignature
            public static Parser create​(TypeCoercerFactory typeCoercerFactory,
                                        ConstructorArgMarshaller marshaller,
                                        KnownRuleTypesProvider knownRuleTypesProvider,
                                        ParserPythonInterpreterProvider parserPythonInterpreterProvider,
                                        DaemonicParserState daemonicParserState,
                                        TargetSpecResolver targetSpecResolver,
                                        Watchman watchman,
                                        BuckEventBus eventBus,
                                        UnconfiguredBuildTargetViewFactory unconfiguredBuildTargetFactory,
                                        TargetConfiguration hostConfiguration,
                                        boolean buckOutIncludeTargetConfigHash)
            ```

            ::: block
            Creates an instance of
            [`Parser`](Parser.html "interface in com.facebook.buck.parser").
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

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

## Class PackageFileParserFactory {#class-packagefileparserfactory .title title="Class PackageFileParserFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.parser.PackageFileParserFactory

::: description
-   

    All Implemented Interfaces:
    :   `FileParserFactory<PackageFileManifest>`

    ------------------------------------------------------------------------

        public class PackageFileParserFactory
        extends Object
        implements FileParserFactory<PackageFileManifest>

    ::: block
    Factory for creating instances of
    [`PackageFileParser`](api/PackageFileParser.html "interface in com.facebook.buck.parser.api").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                    Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `PackageFileParserFactory​(TypeCoercerFactory typeCoercerFactory,                         ParserPythonInterpreterProvider pythonInterpreterProvider,                         KnownRuleTypesProvider knownRuleTypesProvider,                         boolean enableProfiling)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `PackageFileParser`   | `createFilePa         | ::: block             |
        |                       | rser​(BuckEventBus eve | Callers are           |
        |                       | ntBus,                | responsible for       |
        |                       |   Cell cell,          | managing the          |
        |                       |         Watchman watc | life-cycle of the     |
        |                       | hman,                 | created               |
        |                       |  boolean threadSafe)` | [`PackageF            |
        |                       |                       | ileParser`](api/Packa |
        |                       |                       | geFileParser.html "in |
        |                       |                       | terface in com.facebo |
        |                       |                       | ok.buck.parser.api"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

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

        []{#<init>(com.facebook.buck.rules.coercer.TypeCoercerFactory,com.facebook.buck.parser.ParserPythonInterpreterProvider,com.facebook.buck.core.rules.knowntypes.provider.KnownRuleTypesProvider,boolean)}

        -   #### PackageFileParserFactory

                public PackageFileParserFactory​(TypeCoercerFactory typeCoercerFactory,
                                                ParserPythonInterpreterProvider pythonInterpreterProvider,
                                                KnownRuleTypesProvider knownRuleTypesProvider,
                                                boolean enableProfiling)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#createFileParser(com.facebook.buck.event.BuckEventBus,com.facebook.buck.core.cell.Cell,com.facebook.buck.io.watchman.Watchman,boolean)}

        -   #### createFileParser

            ``` methodSignature
            public PackageFileParser createFileParser​(BuckEventBus eventBus,
                                                      Cell cell,
                                                      Watchman watchman,
                                                      boolean threadSafe)
            ```

            ::: block
            Callers are responsible for managing the life-cycle of the
            created
            [`PackageFileParser`](api/PackageFileParser.html "interface in com.facebook.buck.parser.api").
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `createFileParser` in
                interface `FileParserFactory<PackageFileManifest>`
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

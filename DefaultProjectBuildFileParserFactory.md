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

## Class DefaultProjectBuildFileParserFactory {#class-defaultprojectbuildfileparserfactory .title title="Class DefaultProjectBuildFileParserFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.parser.DefaultProjectBuildFileParserFactory

::: description
-   

    All Implemented Interfaces:
    :   `FileParserFactory<BuildFileManifest>`,
        `ProjectBuildFileParserFactory`

    ------------------------------------------------------------------------

        public class DefaultProjectBuildFileParserFactory
        extends Object
        implements ProjectBuildFileParserFactory
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                  Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `DefaultProjectBuildFileParserFactory​(TypeCoercerFactory typeCoercerFactory,                                     ParserPythonInterpreterProvider pythonInterpreterProvider,                                     boolean enableProfiling,                                     Optional<AtomicLong> processedBytes,                                     KnownRuleTypesProvider knownRuleTypesProvider)`                                                         
          `DefaultProjectBuildFileParserFactory​(TypeCoercerFactory typeCoercerFactory,                                     Console console,                                     ParserPythonInterpreterProvider pythonInterpreterProvider,                                     KnownRuleTypesProvider knownRuleTypesProvider)`                                                                                                                                          
          `DefaultProjectBuildFileParserFactory​(TypeCoercerFactory typeCoercerFactory,                                     Console console,                                     ParserPythonInterpreterProvider pythonInterpreterProvider,                                     KnownRuleTypesProvider knownRuleTypesProvider,                                     boolean enableProfiling,                                     Optional<AtomicLong> processedBytes)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Pr                   | `createFilePa         | ::: block             |
        | ojectBuildFileParser` | rser​(BuckEventBus eve | Callers are           |
        |                       | ntBus,                | responsible for       |
        |                       |   Cell cell,          | managing the          |
        |                       |         Watchman watc | life-cycle of the     |
        |                       | hman,                 | created               |
        |                       |  boolean threadSafe)` | [`ProjectBuildFilePa  |
        |                       |                       | rser`](api/ProjectBui |
        |                       |                       | ldFileParser.html "in |
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

        []{#<init>(com.facebook.buck.rules.coercer.TypeCoercerFactory,com.facebook.buck.util.Console,com.facebook.buck.parser.ParserPythonInterpreterProvider,com.facebook.buck.core.rules.knowntypes.provider.KnownRuleTypesProvider,boolean,java.util.Optional)}

        -   #### DefaultProjectBuildFileParserFactory

                public DefaultProjectBuildFileParserFactory​(TypeCoercerFactory typeCoercerFactory,
                                                            Console console,
                                                            ParserPythonInterpreterProvider pythonInterpreterProvider,
                                                            KnownRuleTypesProvider knownRuleTypesProvider,
                                                            boolean enableProfiling,
                                                            Optional<AtomicLong> processedBytes)

        []{#<init>(com.facebook.buck.rules.coercer.TypeCoercerFactory,com.facebook.buck.parser.ParserPythonInterpreterProvider,boolean,java.util.Optional,com.facebook.buck.core.rules.knowntypes.provider.KnownRuleTypesProvider)}

        -   #### DefaultProjectBuildFileParserFactory

                public DefaultProjectBuildFileParserFactory​(TypeCoercerFactory typeCoercerFactory,
                                                            ParserPythonInterpreterProvider pythonInterpreterProvider,
                                                            boolean enableProfiling,
                                                            Optional<AtomicLong> processedBytes,
                                                            KnownRuleTypesProvider knownRuleTypesProvider)

        []{#<init>(com.facebook.buck.rules.coercer.TypeCoercerFactory,com.facebook.buck.util.Console,com.facebook.buck.parser.ParserPythonInterpreterProvider,com.facebook.buck.core.rules.knowntypes.provider.KnownRuleTypesProvider)}

        -   #### DefaultProjectBuildFileParserFactory

                public DefaultProjectBuildFileParserFactory​(TypeCoercerFactory typeCoercerFactory,
                                                            Console console,
                                                            ParserPythonInterpreterProvider pythonInterpreterProvider,
                                                            KnownRuleTypesProvider knownRuleTypesProvider)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#createFileParser(com.facebook.buck.event.BuckEventBus,com.facebook.buck.core.cell.Cell,com.facebook.buck.io.watchman.Watchman,boolean)}

        -   #### createFileParser

            ``` methodSignature
            public ProjectBuildFileParser createFileParser​(BuckEventBus eventBus,
                                                           Cell cell,
                                                           Watchman watchman,
                                                           boolean threadSafe)
            ```

            ::: block
            Callers are responsible for managing the life-cycle of the
            created
            [`ProjectBuildFileParser`](api/ProjectBuildFileParser.html "interface in com.facebook.buck.parser.api").
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `createFileParser` in
                interface `FileParserFactory<BuildFileManifest>`

            [Specified by:]{.overrideSpecifyLabel}
            :   `createFileParser` in
                interface `ProjectBuildFileParserFactory`
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

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
-   [Nested](#nested.class.summary) \| 
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

## Class ParsingContext {#class-parsingcontext .title title="Class ParsingContext"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.parser.ParsingContext

::: description
-   

    ------------------------------------------------------------------------

        public abstract class ParsingContext
        extends Object

    ::: block
    Contains objects and information that may be used during processing
    a parsing request.
    Note that some of the objects in this context may not be used during
    all of the requests. For this reason this context is created using a
    builder pattern where only necessary parameters are passed. Some of
    the parameters are mandatory and they must be passed to the
    `builder()` method.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                      Description
          ------------------- -------------------------- -------------
          `static class `     `ParsingContext.Builder`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor          Description
          -------------------- -------------
          `ParsingContext()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static Pa            | `builder​(Cel          |                       |
        | rsingContext.Builder` | l cell,        com.go |                       |
        |                       | ogle.common.util.conc |                       |
        |                       | urrent.ListeningExecu |                       |
        |                       | torService executor)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `enableTargetC        |                       |
        |                       | ompatibilityChecks()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `exclude              | ::: block             |
        |                       | UnsupportedTargets()` | Whether targets with  |
        |                       |                       | constraints that are  |
        |                       |                       | not compatible with   |
        |                       |                       | the target platform   |
        |                       |                       | should be excluded.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ParserConfig.App     | `getApply             | ::: block             |
        | lyDefaultFlavorsMode` | DefaultFlavorsMode()` | Controls how flavors  |
        |                       |                       | are appended to the   |
        |                       |                       | build targets.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Cell`       | `getCell()`           | ::: block             |
        |                       |                       | Cell for which the    |
        |                       |                       | parsing request is    |
        |                       |                       | performed             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstr                | `getExecutor()`       | ::: block             |
        | act com.google.common |                       | An executor used      |
        | .util.concurrent.List |                       | during parsing        |
        | eningExecutorService` |                       | request to perform    |
        |                       |                       | async computations    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SpeculativeParsing`  | `get                  | ::: block             |
        |                       | SpeculativeParsing()` | Whether speculative   |
        |                       |                       | parsing is enabled.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `                     | ::: block             |
        |                       | isProfilingEnabled()` | Whether to enable     |
        |                       |                       | profiling during      |
        |                       |                       | parsing request.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `useUnconfigur        |                       |
        |                       | edSelectorResolver()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ParsingContext`      | `withApply            |                       |
        |                       | DefaultFlavorsMode​(Pa |                       |
        |                       | rserConfig.ApplyDefau |                       |
        |                       | ltFlavorsMode value)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ParsingContext`      | `                     |                       |
        |                       | withCell​(Cell value)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ParsingContext`      | `wit                  |                       |
        |                       | hExcludeUnsupportedTa |                       |
        |                       | rgets​(boolean value)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ParsingContext`      | `withSpe              |                       |
        |                       | culativeParsing​(Specu |                       |
        |                       | lativeParsing value)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ParsingContext`      | `withUseUn            |                       |
        |                       | configuredSelectorRes |                       |
        |                       | olver​(boolean value)` |                       |
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

        -   #### ParsingContext

                public ParsingContext()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getCell()}

        -   #### getCell

            ``` methodSignature
            public abstract Cell getCell()
            ```

            ::: block
            Cell for which the parsing request is performed
            :::

        []{#getExecutor()}

        -   #### getExecutor

            ``` methodSignature
            public abstract com.google.common.util.concurrent.ListeningExecutorService getExecutor()
            ```

            ::: block
            An executor used during parsing request to perform async
            computations
            :::

        []{#isProfilingEnabled()}

        -   #### isProfilingEnabled

            ``` methodSignature
            @Default
            public boolean isProfilingEnabled()
            ```

            ::: block
            Whether to enable profiling during parsing request.
            :::

        []{#getSpeculativeParsing()}

        -   #### getSpeculativeParsing

            ``` methodSignature
            @Default
            public SpeculativeParsing getSpeculativeParsing()
            ```

            ::: block
            Whether speculative parsing is enabled.
            Speculative parsing a special mode of parsing when
            dependencies of a target are scheduled for parsing ahead of
            the actual requests for parsing of those targets. This may
            lead to over-parsing is some case and thus needs to be used
            in situations when all of the dependencies of requested
            targets are used later.
            :::

        []{#excludeUnsupportedTargets()}

        -   #### excludeUnsupportedTargets

            ``` methodSignature
            @Default
            public boolean excludeUnsupportedTargets()
            ```

            ::: block
            Whether targets with constraints that are not compatible
            with the target platform should be excluded.
            :::

        []{#getApplyDefaultFlavorsMode()}

        -   #### getApplyDefaultFlavorsMode

            ``` methodSignature
            @Default
            public ParserConfig.ApplyDefaultFlavorsMode getApplyDefaultFlavorsMode()
            ```

            ::: block
            Controls how flavors are appended to the build targets.
            :::

            [See Also:]{.seeLabel}
            :   [`ParserConfig.ApplyDefaultFlavorsMode`](config/ParserConfig.ApplyDefaultFlavorsMode.html "enum in com.facebook.buck.parser.config")

        []{#enableTargetCompatibilityChecks()}

        -   #### enableTargetCompatibilityChecks

            ``` methodSignature
            @Default
            public boolean enableTargetCompatibilityChecks()
            ```

        []{#useUnconfiguredSelectorResolver()}

        -   #### useUnconfiguredSelectorResolver

            ``` methodSignature
            @Default
            public boolean useUnconfiguredSelectorResolver()
            ```

        []{#withCell(com.facebook.buck.core.cell.Cell)}

        -   #### withCell

            ``` methodSignature
            public final ParsingContext withCell​(Cell value)
            ```

        []{#withSpeculativeParsing(com.facebook.buck.parser.SpeculativeParsing)}

        -   #### withSpeculativeParsing

            ``` methodSignature
            public final ParsingContext withSpeculativeParsing​(SpeculativeParsing value)
            ```

        []{#withExcludeUnsupportedTargets(boolean)}

        -   #### withExcludeUnsupportedTargets

            ``` methodSignature
            public final ParsingContext withExcludeUnsupportedTargets​(boolean value)
            ```

        []{#withApplyDefaultFlavorsMode(com.facebook.buck.parser.config.ParserConfig.ApplyDefaultFlavorsMode)}

        -   #### withApplyDefaultFlavorsMode

            ``` methodSignature
            public final ParsingContext withApplyDefaultFlavorsMode​(ParserConfig.ApplyDefaultFlavorsMode value)
            ```

        []{#withUseUnconfiguredSelectorResolver(boolean)}

        -   #### withUseUnconfiguredSelectorResolver

            ``` methodSignature
            public final ParsingContext withUseUnconfiguredSelectorResolver​(boolean value)
            ```

        []{#builder(com.facebook.buck.core.cell.Cell,com.google.common.util.concurrent.ListeningExecutorService)}

        -   #### builder

            ``` methodSignature
            public static ParsingContext.Builder builder​(Cell cell,
                                                         com.google.common.util.concurrent.ListeningExecutorService executor)
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
-   [Nested](#nested.class.summary) \| 
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

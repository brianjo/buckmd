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
[Package]{.packageLabelInType} [com.facebook.buck.cli](package-summary.html)
:::

## Class AdditionalOptionsCmdLineParser {#class-additionaloptionscmdlineparser .title title="Class AdditionalOptionsCmdLineParser"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   org.kohsuke.args4j.CmdLineParser

    -   -   com.facebook.buck.cli.AdditionalOptionsCmdLineParser

::: description
-   

    ------------------------------------------------------------------------

        public class AdditionalOptionsCmdLineParser
        extends org.kohsuke.args4j.CmdLineParser

    ::: block
    `CmdLineParser` with nested options via the
    [`AdditionalOptions`](AdditionalOptions.html "annotation in com.facebook.buck.cli")
    annotation.
    Fields annotated with it should be of classes which have a default
    constructor, and will be automatically instantiated.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `AdditionalOpt                    | ::: block                         |
        | ionsCmdLineParser​(org.pf4j.Plugin | Creates a new command line owner  |
        | Manager pluginManager,            | that parses arguments/options and |
        |                     Object bean)` | set them into the given object.   |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+

        : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type          Method                 Description
          -------------------------- ---------------------- -------------
          `org.pf4j.PluginManager`   `getPluginManager()`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.org.kohsuke.args4j.CmdLineParser}

            ### Methods inherited from class org.kohsuke.args4j.CmdLineParser

            `addArgument, addOption, createOptionHandler, getArguments, getOptions, getProperties, isOption, parseArgument, parseArgument, printExample, printExample, printExample, printExample, printOption, printSingleLineUsage, printSingleLineUsage, printUsage, printUsage, printUsage, registerHandler, setUsageWidth, stopOptionParsing`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(org.pf4j.PluginManager,java.lang.Object)}

        -   #### AdditionalOptionsCmdLineParser

                public AdditionalOptionsCmdLineParser​(org.pf4j.PluginManager pluginManager,
                                                      Object bean)

            ::: block
            Creates a new command line owner that parses
            arguments/options and set them into the given object.
            :::

            [Parameters:]{.paramLabel}
            :   `bean` - instance of a class annotated by `Option`,
                `Argument` and
                [`AdditionalOptions`](AdditionalOptions.html "annotation in com.facebook.buck.cli").
                This object will receive values. If this is null, the
                processing will be skipped, which is useful if you\'d
                like to feed metadata from other sources.

            [Throws:]{.throwsLabel}
            :   `org.kohsuke.args4j.IllegalAnnotationError` - if the
                option bean class is using args4j annotations
                incorrectly.

            [See Also:]{.seeLabel}
            :   `CmdLineParser(Object)`
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getPluginManager()}

        -   #### getPluginManager

            ``` methodSignature
            public org.pf4j.PluginManager getPluginManager()
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

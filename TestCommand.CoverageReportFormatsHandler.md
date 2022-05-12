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
-   [Field](#field.summary) \| 
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

## Class TestCommand.CoverageReportFormatsHandler {#class-testcommand.coveragereportformatshandler .title title="Class TestCommand.CoverageReportFormatsHandler"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   org.kohsuke.args4j.spi.OptionHandler\<[CoverageReportFormat](../test/CoverageReportFormat.html "enum in com.facebook.buck.test")\>

    -   -   com.facebook.buck.cli.TestCommand.CoverageReportFormatsHandler

::: description
-   

    Enclosing class:
    :   [TestCommand](TestCommand.html "class in com.facebook.buck.cli")

    ------------------------------------------------------------------------

        public static class TestCommand.CoverageReportFormatsHandler
        extends org.kohsuke.args4j.spi.OptionHandler<CoverageReportFormat>

    ::: block
    args4j does not support parsing repeated (or delimiter separated)
    Enums by default.
    [`TestCommand.CoverageReportFormatsHandler`](TestCommand.CoverageReportFormatsHandler.html "class in com.facebook.buck.cli")
    implements args4j behavior for CoverageReportFormat.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.org.kohsuke.args4j.spi.OptionHandler}

            ### Fields inherited from class org.kohsuke.args4j.spi.OptionHandler

            `option, owner, setter`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                        Description
          ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `CoverageReportFormatsHandler​(org.kohsuke.args4j.CmdLineParser parser,                             org.kohsuke.args4j.OptionDef option,                             org.kohsuke.args4j.spi.Setter<CoverageReportFormat> setter)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                       Description
          ------------------- ------------------------------------------------------------ -------------
          `String`            `getDefaultMetaVariable()`                                    
          `String`            `getMetaVariable​(ResourceBundle rb)`                          
          `int`               `parseArguments​(org.kohsuke.args4j.spi.Parameters params)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.org.kohsuke.args4j.spi.OptionHandler}

            ### Methods inherited from class org.kohsuke.args4j.spi.OptionHandler

            `getNameAndMeta, getNameAndMeta`

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

        []{#<init>(org.kohsuke.args4j.CmdLineParser,org.kohsuke.args4j.OptionDef,org.kohsuke.args4j.spi.Setter)}

        -   #### CoverageReportFormatsHandler

                public CoverageReportFormatsHandler​(org.kohsuke.args4j.CmdLineParser parser,
                                                    org.kohsuke.args4j.OptionDef option,
                                                    org.kohsuke.args4j.spi.Setter<CoverageReportFormat> setter)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#parseArguments(org.kohsuke.args4j.spi.Parameters)}

        -   #### parseArguments

            ``` methodSignature
            public int parseArguments​(org.kohsuke.args4j.spi.Parameters params)
                               throws org.kohsuke.args4j.CmdLineException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `parseArguments` in
                class `org.kohsuke.args4j.spi.OptionHandler<CoverageReportFormat>`

            [Throws:]{.throwsLabel}
            :   `org.kohsuke.args4j.CmdLineException`

        []{#getDefaultMetaVariable()}

        -   #### getDefaultMetaVariable

            ``` methodSignature
            public String getDefaultMetaVariable()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDefaultMetaVariable` in
                class `org.kohsuke.args4j.spi.OptionHandler<CoverageReportFormat>`

        []{#getMetaVariable(java.util.ResourceBundle)}

        -   #### getMetaVariable

            ``` methodSignature
            public String getMetaVariable​(ResourceBundle rb)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `getMetaVariable` in
                class `org.kohsuke.args4j.spi.OptionHandler<CoverageReportFormat>`
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
-   [Field](#field.summary) \| 
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

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

## Class AdditionalOptionsSubCommandHandler {#class-additionaloptionssubcommandhandler .title title="Class AdditionalOptionsSubCommandHandler"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   org.kohsuke.args4j.spi.OptionHandler\<[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}\>

    -   -   org.kohsuke.args4j.spi.SubCommandHandler

        -   -   com.facebook.buck.cli.AdditionalOptionsSubCommandHandler

::: description
-   

    ------------------------------------------------------------------------

        public class AdditionalOptionsSubCommandHandler
        extends org.kohsuke.args4j.spi.SubCommandHandler
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

          Constructor                                                                                                                                                                                                                            Description
          -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `AdditionalOptionsSubCommandHandler​(org.kohsuke.args4j.CmdLineParser parser,                                   org.kohsuke.args4j.OptionDef option,                                   org.kohsuke.args4j.spi.Setter<Object> setter)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                              Method                                                                                 Description
          ---------------------------------------------- -------------------------------------------------------------------------------------- -------------
          `protected org.kohsuke.args4j.CmdLineParser`   `configureParser​(Object subCmd,                org.kohsuke.args4j.spi.SubCommand c)`    
          `int`                                          `parseArguments​(org.kohsuke.args4j.spi.Parameters params)`                              

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.org.kohsuke.args4j.spi.SubCommandHandler}

            ### Methods inherited from class org.kohsuke.args4j.spi.SubCommandHandler

            `fallback, getDefaultMetaVariable, getMetaVariable, instantiate, subCommand`

        ```{=html}
        <!-- -->
        ```
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

        -   #### AdditionalOptionsSubCommandHandler

                public AdditionalOptionsSubCommandHandler​(org.kohsuke.args4j.CmdLineParser parser,
                                                          org.kohsuke.args4j.OptionDef option,
                                                          org.kohsuke.args4j.spi.Setter<Object> setter)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#configureParser(java.lang.Object,org.kohsuke.args4j.spi.SubCommand)}

        -   #### configureParser

            ``` methodSignature
            protected org.kohsuke.args4j.CmdLineParser configureParser​(Object subCmd,
                                                                       org.kohsuke.args4j.spi.SubCommand c)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `configureParser` in
                class `org.kohsuke.args4j.spi.SubCommandHandler`

        []{#parseArguments(org.kohsuke.args4j.spi.Parameters)}

        -   #### parseArguments

            ``` methodSignature
            public int parseArguments​(org.kohsuke.args4j.spi.Parameters params)
                               throws org.kohsuke.args4j.CmdLineException
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `parseArguments` in
                class `org.kohsuke.args4j.spi.SubCommandHandler`

            [Throws:]{.throwsLabel}
            :   `org.kohsuke.args4j.CmdLineException`
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

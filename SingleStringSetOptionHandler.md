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

## Class SingleStringSetOptionHandler {#class-singlestringsetoptionhandler .title title="Class SingleStringSetOptionHandler"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   org.kohsuke.args4j.spi.OptionHandler\<java.util.function.Supplier\<com.google.common.collect.ImmutableSet\<[String](http://docs.oracle.com/javase/7/docs/api/java/lang/String.html?is-external=true "class or interface in java.lang"){.externalLink}\>\>\>

    -   -   com.facebook.buck.cli.SingleStringSetOptionHandler

::: description
-   

    ------------------------------------------------------------------------

        public class SingleStringSetOptionHandler
        extends org.kohsuke.args4j.spi.OptionHandler<java.util.function.Supplier<com.google.common.collect.ImmutableSet<String>>>

    ::: block
    An option handler that allows an option to be specified multiple
    times and coaleced into a set of strings, but only allows one value
    for each specification of the option. This is useful to not cause
    ambiguity when used in conjunction with other options that consume
    multiple values
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

          Constructor                                                                                                                                                                                                                                                                                       Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `SingleStringSetOptionHandler​(org.kohsuke.args4j.CmdLineParser parser,                             org.kohsuke.args4j.OptionDef option,                             org.kohsuke.args4j.spi.Setter<? super java.util.function.Supplier<com.google.common.collect.ImmutableSet<String>>> setter)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                       Description
          ------------------- ------------------------------------------------------------ -------------
          `String`            `getDefaultMetaVariable()`                                    
          `int`               `parseArguments​(org.kohsuke.args4j.spi.Parameters params)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.org.kohsuke.args4j.spi.OptionHandler}

            ### Methods inherited from class org.kohsuke.args4j.spi.OptionHandler

            `getMetaVariable, getNameAndMeta, getNameAndMeta`

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

        -   #### SingleStringSetOptionHandler

                public SingleStringSetOptionHandler​(org.kohsuke.args4j.CmdLineParser parser,
                                                    org.kohsuke.args4j.OptionDef option,
                                                    org.kohsuke.args4j.spi.Setter<? super java.util.function.Supplier<com.google.common.collect.ImmutableSet<String>>> setter)
                                             throws org.kohsuke.args4j.CmdLineException

            [Throws:]{.throwsLabel}
            :   `org.kohsuke.args4j.CmdLineException`
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
                class `org.kohsuke.args4j.spi.OptionHandler<java.util.function.Supplier<com.google.common.collect.ImmutableSet<String>>>`

            [Throws:]{.throwsLabel}
            :   `org.kohsuke.args4j.CmdLineException`

        []{#getDefaultMetaVariable()}

        -   #### getDefaultMetaVariable

            ``` methodSignature
            public String getDefaultMetaVariable()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDefaultMetaVariable` in
                class `org.kohsuke.args4j.spi.OptionHandler<java.util.function.Supplier<com.google.common.collect.ImmutableSet<String>>>`
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

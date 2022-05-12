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

## Class EnvironmentOverrideOptionHandler {#class-environmentoverrideoptionhandler .title title="Class EnvironmentOverrideOptionHandler"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   org.kohsuke.args4j.spi.OptionHandler\<[Map](http://docs.oracle.com/javase/7/docs/api/java/util/Map.html?is-external=true "class or interface in java.util"){.externalLink}\<?,​?\>\>

    -   -   org.kohsuke.args4j.spi.MapOptionHandler

        -   -   com.facebook.buck.cli.EnvironmentOverrideOptionHandler

::: description
-   

    ------------------------------------------------------------------------

        public class EnvironmentOverrideOptionHandler
        extends org.kohsuke.args4j.spi.MapOptionHandler

    ::: block
    OptionHandler used for specifying environment overrides.
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

          Constructor                                                                                                                                                                                                                                Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `EnvironmentOverrideOptionHandler​(org.kohsuke.args4j.CmdLineParser parser,                                 org.kohsuke.args4j.OptionDef option,                                 org.kohsuke.args4j.spi.Setter<? super Map<?,​?>> setter)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                        Description
          ------------------- ------------------------------------------------------------- -------------
          `protected void`    `addToMap​(Map m,         String key,         String value)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.org.kohsuke.args4j.spi.MapOptionHandler}

            ### Methods inherited from class org.kohsuke.args4j.spi.MapOptionHandler

            `addToMap, createNewCollection, getDefaultMetaVariable, parseArguments`

        ```{=html}
        <!-- -->
        ```
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

        -   #### EnvironmentOverrideOptionHandler

                public EnvironmentOverrideOptionHandler​(org.kohsuke.args4j.CmdLineParser parser,
                                                        org.kohsuke.args4j.OptionDef option,
                                                        org.kohsuke.args4j.spi.Setter<? super Map<?,​?>> setter)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#addToMap(java.util.Map,java.lang.String,java.lang.String)}

        -   #### addToMap

            ``` methodSignature
            protected void addToMap​(Map m,
                                    String key,
                                    String value)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `addToMap` in
                class `org.kohsuke.args4j.spi.MapOptionHandler`
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

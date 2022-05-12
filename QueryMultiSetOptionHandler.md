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

## Class QueryMultiSetOptionHandler {#class-querymultisetoptionhandler .title title="Class QueryMultiSetOptionHandler"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   org.kohsuke.args4j.spi.OptionHandler\<[String](http://docs.oracle.com/javase/7/docs/api/java/lang/String.html?is-external=true "class or interface in java.lang"){.externalLink}\>

    -   -   com.facebook.buck.cli.QueryMultiSetOptionHandler

::: description
-   

    ------------------------------------------------------------------------

        public class QueryMultiSetOptionHandler
        extends org.kohsuke.args4j.spi.OptionHandler<String>

    ::: block
    A simple option handler whose main job is to not freak out when it
    sees \`\--\`, which is used by QueryCommand as a separator between
    different sets. Most option handlers stop parsing as soon as they
    see a param starting with \`-\`.
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

          Constructor                                                                                                                                                                                                    Description
          -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `QueryMultiSetOptionHandler​(org.kohsuke.args4j.CmdLineParser parser,                           org.kohsuke.args4j.OptionDef option,                           org.kohsuke.args4j.spi.Setter<String> setter)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `String`              | `getD                 | ::: block             |
        |                       | efaultMetaVariable()` | Returns `"STRING[]"`. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `parseArguments​(      | ::: block             |
        |                       | org.kohsuke.args4j.sp | Tries to parse        |
        |                       | i.Parameters params)` | `String[]` argument   |
        |                       |                       | from `Parameters`.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

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

        -   #### QueryMultiSetOptionHandler

                public QueryMultiSetOptionHandler​(org.kohsuke.args4j.CmdLineParser parser,
                                                  org.kohsuke.args4j.OptionDef option,
                                                  org.kohsuke.args4j.spi.Setter<String> setter)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getDefaultMetaVariable()}

        -   #### getDefaultMetaVariable

            ``` methodSignature
            public String getDefaultMetaVariable()
            ```

            ::: block
            Returns `"STRING[]"`.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDefaultMetaVariable` in
                class `org.kohsuke.args4j.spi.OptionHandler<String>`

            [Returns:]{.returnLabel}
            :   return \"STRING\[\]\";

        []{#parseArguments(org.kohsuke.args4j.spi.Parameters)}

        -   #### parseArguments

            ``` methodSignature
            public int parseArguments​(org.kohsuke.args4j.spi.Parameters params)
                               throws org.kohsuke.args4j.CmdLineException
            ```

            ::: block
            Tries to parse `String[]` argument from `Parameters`.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `parseArguments` in
                class `org.kohsuke.args4j.spi.OptionHandler<String>`

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

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

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../deprecated-list.html)
-   [Index](../../../../../index-all.html)
-   [Help](../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.util.config](package-summary.html)
:::

## Class RawConfig.Builder {#class-rawconfig.builder .title title="Class RawConfig.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.config.RawConfig.Builder

::: description
-   

    Enclosing class:
    :   [RawConfig](RawConfig.html "class in com.facebook.buck.util.config")

    ------------------------------------------------------------------------

        public static class RawConfig.Builder
        extends Object

    ::: block
    A builder for
    [`RawConfig`](RawConfig.html "class in com.facebook.buck.util.config")s.
    Unless otherwise stated, duplicate keys overwrites earlier ones.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor   Description
          ------------- -------------
          `Builder()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `RawConfig`           | `build()`             |                       |
        +-----------------------+-----------------------+-----------------------+
        | `RawConfig.Builder`   | `put​(String           | ::: block             |
        |                       |  section,    String k | Put a single value.   |
        |                       | ey,    String value)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RawConfig.Builder`   | `putA                 | ::: block             |
        |                       | ll​(RawConfig config)` | Merge the values from |
        |                       |                       | another `RawConfig`.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `<M ext               | `putAll​(M             | ::: block             |
        | ends Map<String,​Strin | ap<String,​M> config)` | Merge raw config      |
        | g>>RawConfig.Builder` |                       | values into this      |
        |                       |                       | config.               |
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

        []{#<init>()}

        -   #### Builder

                public Builder()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#putAll(java.util.Map)}

        -   #### putAll

            ``` methodSignature
            public <M extends Map<String,​String>> RawConfig.Builder putAll​(Map<String,​M> config)
            ```

            ::: block
            Merge raw config values into this config.
            :::

        []{#putAll(com.facebook.buck.util.config.RawConfig)}

        -   #### putAll

            ``` methodSignature
            public RawConfig.Builder putAll​(RawConfig config)
            ```

            ::: block
            Merge the values from another `RawConfig`.
            :::

        []{#put(java.lang.String,java.lang.String,java.lang.String)}

        -   #### put

            ``` methodSignature
            public RawConfig.Builder put​(String section,
                                         String key,
                                         String value)
            ```

            ::: block
            Put a single value.
            :::

        []{#build()}

        -   #### build

            ``` methodSignature
            public RawConfig build()
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

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../deprecated-list.html)
-   [Index](../../../../../index-all.html)
-   [Help](../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../allclasses.html)

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

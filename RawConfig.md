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
[Package]{.packageLabelInType} [com.facebook.buck.util.config](package-summary.html)
:::

## Class RawConfig {#class-rawconfig .title title="Class RawConfig"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.config.RawConfig

::: description
-   

    ------------------------------------------------------------------------

        public abstract class RawConfig
        extends Object

    ::: block
    Hierarchical configuration of section/key/value triples.
    This class only implements the simple construction/storage/retrieval
    of these values. Other classes like
    [`Config`](Config.html "class in com.facebook.buck.util.config")
    implements accessors that interpret the values as other types.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `RawConfig.Builder`   | ::: block             |
        |                       |                       | A builder for         |
        |                       |                       | [`RawConf             |
        |                       |                       | ig`](RawConfig.html " |
        |                       |                       | class in com.facebook |
        |                       |                       | .buck.util.config")s. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor     Description
          --------------- -------------
          `RawConfig()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `stat                 | `builder()`           |                       |
        | ic RawConfig.Builder` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.c         | `getSection           | ::: block             |
        | ommon.collect.Immutab | ​(String sectionName)` | Retrieve a section by |
        | leMap<String,​String>` |                       | name.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getValu              | ::: block             |
        |                       | e​(String sectionName, | Retrieve a value from |
        |                       |          String key)` | a named section.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstr                | `getValues()`         |                       |
        | act com.google.common |                       |                       |
        | .collect.ImmutableMap |                       |                       |
        | <String,​com.google.co |                       |                       |
        | mmon.collect.Immutabl |                       |                       |
        | eMap<String,​String>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static RawConfig`    | `of()`                | ::: block             |
        |                       |                       | Returns an empty      |
        |                       |                       | config.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static RawConfig`    | `of​(                  |                       |
        |                       | Map<String,​? extends  |                       |
        |                       | com.google.common.col |                       |
        |                       | lect.ImmutableMap<Str |                       |
        |                       | ing,​String>> values)` |                       |
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

        -   #### RawConfig

                public RawConfig()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getValues()}

        -   #### getValues

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableMap<String,​com.google.common.collect.ImmutableMap<String,​String>> getValues()
            ```

        []{#getSection(java.lang.String)}

        -   #### getSection

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​String> getSection​(String sectionName)
            ```

            ::: block
            Retrieve a section by name.
            :::

            [Returns:]{.returnLabel}
            :   The contents of the named section. If the section does
                not exist, the empty map.

        []{#getValue(java.lang.String,java.lang.String)}

        -   #### getValue

            ``` methodSignature
            public Optional<String> getValue​(String sectionName,
                                             String key)
            ```

            ::: block
            Retrieve a value from a named section.
            :::

        []{#of()}

        -   #### of

            ``` methodSignature
            public static RawConfig of()
            ```

            ::: block
            Returns an empty config.
            :::

        []{#of(java.util.Map)}

        -   #### of

            ``` methodSignature
            public static RawConfig of​(Map<String,​? extends com.google.common.collect.ImmutableMap<String,​String>> values)
            ```

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static RawConfig.Builder builder()
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

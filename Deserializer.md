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
[Package]{.packageLabelInType} [com.facebook.buck.rules.modern](package-summary.html)
:::

## Class Deserializer {#class-deserializer .title title="Class Deserializer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.modern.Deserializer

::: description
-   

    ------------------------------------------------------------------------

        public class Deserializer
        extends Object

    ::: block
    Implements deserialization of Buildables.
    This works by walking all referenced fields and creating them with a
    ValueCreator. It uses Objenesis to create objects and then injects
    the field values via reflection.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static interface `   | `Dese                 | ::: block             |
        |                       | rializer.ClassFinder` | Used for looking up   |
        |                       |                       | classes.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static interface `   | `Deser                | ::: block             |
        |                       | ializer.DataProvider` | DataProviders are     |
        |                       |                       | used for              |
        |                       |                       | deserializing         |
        |                       |                       | \"dynamic\" objects.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                   Description
          ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `Deserializer​(java.util.function.Function<Optional<String>,​ProjectFilesystem> cellMap,             Deserializer.ClassFinder classFinder,             java.util.function.Supplier<SourcePathResolverAdapter> pathResolver,             ToolchainProvider toolchainProvider)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type              Method                                                                         Description
          ------------------------------ ------------------------------------------------------------------------------ -------------
          `<T extends AddsToRuleKey>T`   `deserialize​(Deserializer.DataProvider provider,            Class<T> clazz)`    

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

        []{#<init>(java.util.function.Function,com.facebook.buck.rules.modern.Deserializer.ClassFinder,java.util.function.Supplier,com.facebook.buck.core.toolchain.ToolchainProvider)}

        -   #### Deserializer

                public Deserializer​(java.util.function.Function<Optional<String>,​ProjectFilesystem> cellMap,
                                    Deserializer.ClassFinder classFinder,
                                    java.util.function.Supplier<SourcePathResolverAdapter> pathResolver,
                                    ToolchainProvider toolchainProvider)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#deserialize(com.facebook.buck.rules.modern.Deserializer.DataProvider,java.lang.Class)}

        -   #### deserialize

            ``` methodSignature
            public <T extends AddsToRuleKey> T deserialize​(Deserializer.DataProvider provider,
                                                           Class<T> clazz)
                                                    throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`
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

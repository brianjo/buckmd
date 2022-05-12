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
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.util.zip](package-summary.html)
:::

## Interface JarBuilder.Observer {#interface-jarbuilder.observer .title title="Interface JarBuilder.Observer"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `LoggingJarBuilderObserver`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [JarBuilder](JarBuilder.html "class in com.facebook.buck.util.zip")

    ------------------------------------------------------------------------

        public static interface JarBuilder.Observer
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type              Field        Description
          ------------------------------ ------------ -------------
          `static JarBuilder.Observer`   `IGNORING`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                               Description
          ------------------- ------------------------------------------------------------------------------------ -------------
          `void`              `onDuplicateEntry​(String jarFile,                 JarEntrySupplier entrySupplier)`    
          `void`              `onEntryOmitted​(String jarFile,               JarEntrySupplier entrySupplier)`        

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#IGNORING}

        -   #### IGNORING

                static final JarBuilder.Observer IGNORING
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#onDuplicateEntry(java.lang.String,com.facebook.buck.util.zip.JarEntrySupplier)}

        -   #### onDuplicateEntry

            ``` methodSignature
            void onDuplicateEntry​(String jarFile,
                                  JarEntrySupplier entrySupplier)
            ```

        []{#onEntryOmitted(java.lang.String,com.facebook.buck.util.zip.JarEntrySupplier)}

        -   #### onEntryOmitted

            ``` methodSignature
            void onEntryOmitted​(String jarFile,
                                JarEntrySupplier entrySupplier)
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
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

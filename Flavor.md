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
[Package]{.packageLabelInType} [com.facebook.buck.core.model](package-summary.html)
:::

## Interface Flavor {#interface-flavor .title title="Interface Flavor"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `Comparable<Flavor>`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `InternalFlavor`, `UserFlavor`

    ------------------------------------------------------------------------

        public interface Flavor
        extends Comparable<Flavor>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                         Description
          ------------------- ----------------------------- -------------
          `static Pattern`    `INVALID_FLAVOR_CHARACTERS`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                    Description
          ------------------- ----------------------------------------- -------------
          `default void`      `check()`                                  
          `default int`       `compareTo​(Flavor that)`                   
          `String`            `getName()`                                
          `static String`     `replaceInvalidCharacters​(String name)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
          .tableTab}[[Default
          Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#INVALID_FLAVOR_CHARACTERS}

        -   #### INVALID_FLAVOR_CHARACTERS

                static final Pattern INVALID_FLAVOR_CHARACTERS
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#replaceInvalidCharacters(java.lang.String)}

        -   #### replaceInvalidCharacters

            ``` methodSignature
            static String replaceInvalidCharacters​(String name)
            ```

        []{#getName()}

        -   #### getName

            ``` methodSignature
            String getName()
            ```

        []{#check()}

        -   #### check

            ``` methodSignature
            default void check()
            ```

        []{#compareTo(com.facebook.buck.core.model.Flavor)}

        -   #### compareTo

            ``` methodSignature
            default int compareTo​(Flavor that)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `compareTo` in interface `Comparable<Flavor>`
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

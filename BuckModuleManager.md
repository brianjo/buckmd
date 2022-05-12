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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.core.module](package-summary.html)
:::

## Interface BuckModuleManager {#interface-buckmodulemanager .title title="Interface BuckModuleManager"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `DefaultBuckModuleManager`

    ------------------------------------------------------------------------

        public interface BuckModuleManager

    ::: block
    Provides access to module information.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                        Method                                     Description
          -------------------------------------------------------- ------------------------------------------ -------------
          `com.google.common.collect.ImmutableSortedSet<String>`   `getModuleDependencies​(String moduleId)`    
          `String`                                                 `getModuleHash​(Class<?> cls)`               
          `String`                                                 `getModuleHash​(String moduleId)`            
          `com.google.common.collect.ImmutableSortedSet<String>`   `getModuleIds()`                            
          `boolean`                                                `isClassInModule​(Class<?> cls)`             

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#isClassInModule(java.lang.Class)}

        -   #### isClassInModule

            ``` methodSignature
            boolean isClassInModule​(Class<?> cls)
            ```

        []{#getModuleHash(java.lang.Class)}

        -   #### getModuleHash

            ``` methodSignature
            String getModuleHash​(Class<?> cls)
            ```

        []{#getModuleHash(java.lang.String)}

        -   #### getModuleHash

            ``` methodSignature
            String getModuleHash​(String moduleId)
            ```

            [Returns:]{.returnLabel}
            :   the hash of module\'s content (which includes code and
                resources.)

        []{#getModuleIds()}

        -   #### getModuleIds

            ``` methodSignature
            com.google.common.collect.ImmutableSortedSet<String> getModuleIds()
            ```

            [Returns:]{.returnLabel}
            :   IDs of all modules known to this instance.

        []{#getModuleDependencies(java.lang.String)}

        -   #### getModuleDependencies

            ``` methodSignature
            com.google.common.collect.ImmutableSortedSet<String> getModuleDependencies​(String moduleId)
            ```

            [Returns:]{.returnLabel}
            :   IDs of all modules the provided module depends on.
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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

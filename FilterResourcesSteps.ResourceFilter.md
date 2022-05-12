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
[Package]{.packageLabelInType} [com.facebook.buck.android](package-summary.html)
:::

## Class FilterResourcesSteps.ResourceFilter {#class-filterresourcessteps.resourcefilter .title title="Class FilterResourcesSteps.ResourceFilter"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.FilterResourcesSteps.ResourceFilter

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [FilterResourcesSteps](FilterResourcesSteps.html "class in com.facebook.buck.android")

    ------------------------------------------------------------------------

        public static class FilterResourcesSteps.ResourceFilter
        extends Object
        implements AddsToRuleKey

    ::: block
    Helper class for interpreting the resource_filter argument to
    android_binary().
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                     Description
          ----------------------------------------------- -------------
          `ResourceFilter​(List<String> resourceFilter)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                Method                Description
          -------------------------------- --------------------- -------------
          `Set<ResourceFilters.Density>`   `getDensities()`       
          `String`                         `getDescription()`     
          `boolean`                        `isEnabled()`          
          `boolean`                        `shouldDownscale()`    

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

        []{#<init>(java.util.List)}

        -   #### ResourceFilter

                public ResourceFilter​(List<String> resourceFilter)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#shouldDownscale()}

        -   #### shouldDownscale

            ``` methodSignature
            public boolean shouldDownscale()
            ```

        []{#getDensities()}

        -   #### getDensities

            ``` methodSignature
            @Nullable
            public Set<ResourceFilters.Density> getDensities()
            ```

        []{#isEnabled()}

        -   #### isEnabled

            ``` methodSignature
            public boolean isEnabled()
            ```

        []{#getDescription()}

        -   #### getDescription

            ``` methodSignature
            public String getDescription()
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

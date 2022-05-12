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
-   [Nested](#nested.class.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.android](package-summary.html)
:::

## Class FilterResourcesSteps {#class-filterresourcessteps .title title="Class FilterResourcesSteps"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.FilterResourcesSteps

::: description
-   

    ------------------------------------------------------------------------

        public class FilterResourcesSteps
        extends Object

    ::: block
    This
    [`Step`](../step/Step.html "interface in com.facebook.buck.step")
    copies `res` directories to a different location, while filtering
    out certain resources.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `FilterRe             |                       |
        |                       | sourcesSteps.Builder` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `F                    |                       |
        |                       | ilterResourcesSteps.D |                       |
        |                       | efaultDrawableFinder` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static interface `   | `FilterResources      |                       |
        |                       | Steps.DrawableFinder` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static interface `   | `FilterResour         |                       |
        |                       | cesSteps.ImageScaler` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `FilterResources      | ::: block             |
        |                       | Steps.ResourceFilter` | Helper class for      |
        |                       |                       | interpreting the      |
        |                       |                       | resource_filter       |
        |                       |                       | argument to           |
        |                       |                       | android_binary().     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                       Method             Description
          --------------------------------------- ------------------ -------------
          `static FilterResourcesSteps.Builder`   `builder()`         
          `Step`                                  `getCopyStep()`     
          `Step`                                  `getScaleStep()`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
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
    -   []{#method.detail}

        ### Method Detail

        []{#getCopyStep()}

        -   #### getCopyStep

            ``` methodSignature
            public Step getCopyStep()
            ```

        []{#getScaleStep()}

        -   #### getScaleStep

            ``` methodSignature
            public Step getScaleStep()
            ```

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static FilterResourcesSteps.Builder builder()
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
-   [Nested](#nested.class.summary) \| 
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

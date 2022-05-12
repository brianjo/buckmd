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
[Package]{.packageLabelInType} [com.facebook.buck.android.packageable](package-summary.html)
:::

## Class NoopAndroidPackageableFilter {#class-noopandroidpackageablefilter .title title="Class NoopAndroidPackageableFilter"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.packageable.NoopAndroidPackageableFilter

::: description
-   

    All Implemented Interfaces:
    :   `AndroidPackageableFilter`

    ------------------------------------------------------------------------

        public class NoopAndroidPackageableFilter
        extends Object
        implements AndroidPackageableFilter

    ::: block
    Indicates that no filtering is done.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                        Description
          ---------------------------------- -------------
          `NoopAndroidPackageableFilter()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `boolean`             | `shouldExclud         | ::: block             |
        |                       | eNonNativeTarget​(Buil | Encapsulates the      |
        |                       | dTarget buildTarget)` | filtering logic of    |
        |                       |                       | non-native targets    |
        |                       |                       | (java libraries,      |
        |                       |                       | resources, etc.)      |
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

        -   #### NoopAndroidPackageableFilter

                public NoopAndroidPackageableFilter()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#shouldExcludeNonNativeTarget(com.facebook.buck.core.model.BuildTarget)}

        -   #### shouldExcludeNonNativeTarget

            ``` methodSignature
            public boolean shouldExcludeNonNativeTarget​(BuildTarget buildTarget)
            ```

            ::: block
            [Description copied from
            interface: `AndroidPackageableFilter`]{.descfrmTypeLabel}
            :::

            ::: block
            Encapsulates the filtering logic of non-native targets (java
            libraries, resources, etc.)
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `shouldExcludeNonNativeTarget` in
                interface `AndroidPackageableFilter`

            [Returns:]{.returnLabel}
            :   `true` if the given target (that represents a target
                with non-native code, like java library or resources)
                should be excluded from the collection.
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
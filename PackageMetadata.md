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
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.parser.api](package-summary.html)
:::

## Class PackageMetadata {#class-packagemetadata .title title="Class PackageMetadata"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.parser.api.PackageMetadata

::: description
-   

    ------------------------------------------------------------------------

        public abstract class PackageMetadata
        extends Object

    ::: block
    Describes the attributes of a package rule in a package file.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Field                 | Description           |
        +=======================+=======================+=======================+
        | `static com.facebook  | `EMPTY_SINGLETON`     | ::: block             |
        | .buck.parser.api.Immu |                       | A singleton instance  |
        | tablePackageMetadata` |                       | with no               |
        |                       |                       | v                     |
        |                       |                       | isibility/within_view |
        |                       |                       | entries.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor           Description
          --------------------- -------------
          `PackageMetadata()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                            Method                                                                                                                           Description
          ------------------------------------------------------------ -------------------------------------------------------------------------------------------------------------------------------- -------------
          `abstract com.google.common.collect.ImmutableList<String>`   `getVisibility()`                                                                                                                 
          `abstract com.google.common.collect.ImmutableList<String>`   `getWithinView()`                                                                                                                 
          `static PackageMetadata`                                     `of​(com.google.common.collect.ImmutableList<String> visibility,   com.google.common.collect.ImmutableList<String> withinView)`    

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
    -   []{#field.detail}

        ### Field Detail

        []{#EMPTY_SINGLETON}

        -   #### EMPTY_SINGLETON

                public static final com.facebook.buck.parser.api.ImmutablePackageMetadata EMPTY_SINGLETON

            ::: block
            A singleton instance with no visibility/within_view entries.
            :::
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### PackageMetadata

                public PackageMetadata()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getVisibility()}

        -   #### getVisibility

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<String> getVisibility()
            ```

            [Returns:]{.returnLabel}
            :   the visibility defined in the package.

        []{#getWithinView()}

        -   #### getWithinView

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<String> getWithinView()
            ```

            [Returns:]{.returnLabel}
            :   the within_view defined in the package.

        []{#of(com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableList)}

        -   #### of

            ``` methodSignature
            public static PackageMetadata of​(com.google.common.collect.ImmutableList<String> visibility,
                                             com.google.common.collect.ImmutableList<String> withinView)
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
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
-   Field \| 
-   Required \| 
-   Optional

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Element

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
[Package]{.packageLabelInType} [com.facebook.buck.core.util.immutables](package-summary.html)
:::

## Annotation Type RuleArg {#annotation-type-rulearg .title title="Annotation Type RuleArg"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        @Target({TYPE,PACKAGE,ANNOTATION_TYPE})
        @Retention(RUNTIME)
        public @interface RuleArg

    ::: block
    Immutable generator for data transfer objects. These are objects
    that are, or belong on rule args. These types can be coerced by the
    parser from python/starlark into java objects.
    This style:

    1.  Does not add the Immutable prefix on generated classes
    2.  Strips off the Abstract name prefix when processing the parent
        interface or abstract class
    3.  Supports isFoo() / getFoo() getters in the parent interface or
        abstract class
    4.  Supports setFoo() setters in the parent interface or abstract
        class
    5.  Ensures the generated class is public (even if the parent
        interface or abstract class is package private)
    6.  Disable generating with\* methods by default, as they cause
        excessive codegen.
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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

<div>

-   Summary: 
-   Field \| 
-   Required \| 
-   Optional

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Element

</div>

[]{#skip.navbar.bottom}
:::

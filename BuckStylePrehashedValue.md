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

## Annotation Type BuckStylePrehashedValue {#annotation-type-buckstyleprehashedvalue .title title="Annotation Type BuckStylePrehashedValue"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        @Target({TYPE,PACKAGE,ANNOTATION_TYPE})
        @Retention(RUNTIME)
        public @interface BuckStylePrehashedValue

    ::: block
    This is similar to
    [`BuckStyleValue`](BuckStyleValue.html "annotation in com.facebook.buck.core.util.immutables")
    but with prehash.
    Value-style objects with prehashing.

    Value-style objects have all attributes as \"of\" constructor
    parameters, do not have builders, \"with\" methods, \"copy\"
    methods.

    When using this annotation, it\'s unnecessary to explicitly use
    \@Value.Immutable.

    If the Value.Immutable behavior needs to be customized, you must
    explicitly set the values set in the defaults here (otherwise a
    linter will yell at you).
    :::

    [See Also:]{.seeLabel}
    :   [Immutable user
        guide](http://immutables.github.io/immutable.html#tuples)
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

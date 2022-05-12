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

## Annotation Type BuckStyleValue {#annotation-type-buckstylevalue .title title="Annotation Type BuckStyleValue"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        @Target({TYPE,PACKAGE,ANNOTATION_TYPE})
        @Retention(RUNTIME)
        public @interface BuckStyleValue

    ::: block
    Value-style objects.
    The generated immutable will be package private only so that the
    immutable generated class is not used. The declaring
    interface/abstract class should re-expose constructors as
    appropriate (like auto-value). It is intended that all users of the
    immutable ever only refer to the interface/abstract class so that
    the underlying immmutable implementation can change freely.

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
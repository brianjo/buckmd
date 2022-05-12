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
[Package]{.packageLabelInType} [com.facebook.buck.cli](package-summary.html)
:::

## Annotation Type AdditionalOptions {#annotation-type-additionaloptions .title title="Annotation Type AdditionalOptions"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        @Retention(RUNTIME)
        @Target(FIELD)
        public @interface AdditionalOptions

    ::: block
    If this annotation is used on a field in one of the `..Options`
    classes (e.g. subclasses of
    [`AbstractCommand`](AbstractCommand.html "class in com.facebook.buck.cli")),
    then a
    [`AdditionalOptionsCmdLineParser`](AdditionalOptionsCmdLineParser.html "class in com.facebook.buck.cli")
    will recursively look for options/arguments in the (class of the)
    field and add them to the parser, almost allowing traits for
    options.
    Usage example:

         class MyOptions{
           @AdditionalOptions
           public ReusableSubOptions subOptions;
           @Option(...)
           public String someOption;
         }
         class ReusableSubOptions{
           @Option(...)
           public String someSubOption;
         }
         
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

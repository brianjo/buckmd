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
[Package]{.packageLabelInType} [com.facebook.buck.parser.implicit](package-summary.html)
:::

## Class PackageImplicitIncludesFinder {#class-packageimplicitincludesfinder .title title="Class PackageImplicitIncludesFinder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.parser.implicit.PackageImplicitIncludesFinder

::: description
-   

    ------------------------------------------------------------------------

        public class PackageImplicitIncludesFinder
        extends Object

    ::: block
    Given a configuration, find packages that should be implicitly
    included for a given build file
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Optio                | `                     | ::: block             |
        | nal<ImplicitInclude>` | findIncludeForBuildFi | Find the file (if     |
        |                       | le​(Path packagePath)` | any) that should be   |
        |                       |                       | included implicitly   |
        |                       |                       | for a given build     |
        |                       |                       | file path             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static PackageIm     | `fromConfigurati      | ::: block             |
        | plicitIncludesFinder` | on​(com.google.common. | Create a              |
        |                       | collect.ImmutableMap< | [`Package             |
        |                       | String,​ImplicitInclud | ImplicitIncludesFinde |
        |                       | e> packageToInclude)` | r`](PackageImplicitIn |
        |                       |                       | cludesFinder.html "cl |
        |                       |                       | ass in com.facebook.b |
        |                       |                       | uck.parser.implicit") |
        |                       |                       | from configuration in |
        |                       |                       | .buckconfig           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

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

        []{#fromConfiguration(com.google.common.collect.ImmutableMap)}

        -   #### fromConfiguration

            ``` methodSignature
            public static PackageImplicitIncludesFinder fromConfiguration​(com.google.common.collect.ImmutableMap<String,​ImplicitInclude> packageToInclude)
            ```

            ::: block
            Create a
            [`PackageImplicitIncludesFinder`](PackageImplicitIncludesFinder.html "class in com.facebook.buck.parser.implicit")
            from configuration in .buckconfig
            :::

            [Parameters:]{.paramLabel}
            :   `packageToInclude` - A mapping of package paths to file
                that should be included

            [Returns:]{.returnLabel}
            :   A
                [`PackageImplicitIncludesFinder`](PackageImplicitIncludesFinder.html "class in com.facebook.buck.parser.implicit")
                instance

        []{#findIncludeForBuildFile(java.nio.file.Path)}

        -   #### findIncludeForBuildFile

            ``` methodSignature
            public Optional<ImplicitInclude> findIncludeForBuildFile​(@Nullable
                                                                     Path packagePath)
            ```

            ::: block
            Find the file (if any) that should be included implicitly
            for a given build file path
            :::

            [Parameters:]{.paramLabel}
            :   `packagePath` - The path to a package relative to the
                cell root.

            [Returns:]{.returnLabel}
            :   The path to a file and symbols that should be implicitly
                included for the given package.
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

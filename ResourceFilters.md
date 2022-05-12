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
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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

## Class ResourceFilters {#class-resourcefilters .title title="Class ResourceFilters"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.ResourceFilters

::: description
-   

    ------------------------------------------------------------------------

        public class ResourceFilters
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `Res                  | ::: block             |
        |                       | ourceFilters.Density` | Represents the names  |
        |                       |                       | and values of valid   |
        |                       |                       | densities for         |
        |                       |                       | resources as defined  |
        |                       |                       | in                    |
        |                       |                       | http://de             |
        |                       |                       | veloper.android.com/g |
        |                       |                       | uide/topics/resources |
        |                       |                       | /providing-resources. |
        |                       |                       | html#DensityQualifier |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `Resour               |                       |
        |                       | ceFilters.Qualifiers` |                       |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Field                 | Description           |
        +=======================+=======================+=======================+
        | `static com.g         | `SUPPORTED_           | ::: block             |
        | oogle.common.collect. | RESOURCE_DIRECTORIES` | The set of supported  |
        | ImmutableSet<String>` |                       | directories in        |
        |                       |                       | resource folders.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `                     | `createDens           | ::: block             |
        | static java.util.func | ityFilter​(ProjectFile | Given a set of target |
        | tion.Predicate<Path>` | system filesystem,    | densities, returns a  |
        |                       |                  Set< | `Predicate` that      |
        |                       | ResourceFilters.Densi | fails for any         |
        |                       | ty> targetDensities)` | non-drawable resource |
        |                       |                       | of a different        |
        |                       |                       | density.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `cr                   | ::: block             |
        | static java.util.func | eateImageDensityFilte | Given a list of paths |
        | tion.Predicate<Path>` | r​(Collection<Path> ca | of available          |
        |                       | ndidates,             | drawables, and a      |
        |                       |              Set<Reso | target screen         |
        |                       | urceFilters.Density>  | density, returns a    |
        |                       | targetDensities,      | `Predicate` that      |
        |                       |                     b | fails for drawables   |
        |                       | oolean canDownscale)` | of a different        |
        |                       |                       | density, whenever     |
        |                       |                       | they can be safely    |
        |                       |                       | removed.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
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

        []{#SUPPORTED_RESOURCE_DIRECTORIES}

        -   #### SUPPORTED_RESOURCE_DIRECTORIES

                public static final com.google.common.collect.ImmutableSet<String> SUPPORTED_RESOURCE_DIRECTORIES

            ::: block
            The set of supported directories in resource folders. This
            is defined in
            http://developer.android.com/guide/topics/resources/providing-resources.html#table1
            :::
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#createImageDensityFilter(java.util.Collection,java.util.Set,boolean)}

        -   #### createImageDensityFilter

            ``` methodSignature
            public static java.util.function.Predicate<Path> createImageDensityFilter​(Collection<Path> candidates,
                                                                                      Set<ResourceFilters.Density> targetDensities,
                                                                                      boolean canDownscale)
            ```

            ::: block
            Given a list of paths of available drawables, and a target
            screen density, returns a `Predicate` that fails for
            drawables of a different density, whenever they can be
            safely removed.
            :::

            [Parameters:]{.paramLabel}
            :   `candidates` - list of available drawables
            :   `targetDensities` - set of e.g. `"mdpi"`, `"ldpi"` etc.
            :   `canDownscale` - if no exact match is available, retain
                the highest quality

            [Returns:]{.returnLabel}
            :   a predicate as above

        []{#createDensityFilter(com.facebook.buck.io.filesystem.ProjectFilesystem,java.util.Set)}

        -   #### createDensityFilter

            ``` methodSignature
            public static java.util.function.Predicate<Path> createDensityFilter​(ProjectFilesystem filesystem,
                                                                                 Set<ResourceFilters.Density> targetDensities)
            ```

            ::: block
            Given a set of target densities, returns a `Predicate` that
            fails for any non-drawable resource of a different density.
            Special consideration exists for the default density
            ([`ResourceFilters.Density.NO_QUALIFIER`](ResourceFilters.Density.html#NO_QUALIFIER)
            when the target does not exists.
            :::
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
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

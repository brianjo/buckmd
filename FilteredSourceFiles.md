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
[Package]{.packageLabelInType} [com.facebook.buck.features.go](package-summary.html)
:::

## Class FilteredSourceFiles {#class-filteredsourcefiles .title title="Class FilteredSourceFiles"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.go.FilteredSourceFiles

::: description
-   

    All Implemented Interfaces:
    :   `Iterable<Path>`

    ------------------------------------------------------------------------

        public class FilteredSourceFiles
        extends Object
        implements Iterable<Path>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                              Description
          -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `FilteredSourceFiles​(List<Path> rawSrcFiles,                    com.facebook.buck.features.go.GoPlatform platform,                    List<com.facebook.buck.features.go.GoListStep.ListType> fileTypes)`                                                 
          `FilteredSourceFiles​(List<Path> rawSrcFiles,                    List<Path> extraSrcFiles,                    com.facebook.buck.features.go.GoPlatform platform,                    List<com.facebook.buck.features.go.GoListStep.ListType> fileTypes)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type          Method               Description
          -------------------------- -------------------- -------------
          `Collection<GoListStep>`   `getFilterSteps()`    
          `Iterator<Path>`           `iterator()`          

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Iterable}

            ### Methods inherited from interface java.lang.[Iterable](http://docs.oracle.com/javase/7/docs/api/java/lang/Iterable.html?is-external=true "class or interface in java.lang"){.externalLink}

            `forEach, spliterator`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.util.List,com.facebook.buck.features.go.GoPlatform,java.util.List)}

        -   #### FilteredSourceFiles

                public FilteredSourceFiles​(List<Path> rawSrcFiles,
                                           com.facebook.buck.features.go.GoPlatform platform,
                                           List<com.facebook.buck.features.go.GoListStep.ListType> fileTypes)

        []{#<init>(java.util.List,java.util.List,com.facebook.buck.features.go.GoPlatform,java.util.List)}

        -   #### FilteredSourceFiles

                public FilteredSourceFiles​(List<Path> rawSrcFiles,
                                           List<Path> extraSrcFiles,
                                           com.facebook.buck.features.go.GoPlatform platform,
                                           List<com.facebook.buck.features.go.GoListStep.ListType> fileTypes)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getFilterSteps()}

        -   #### getFilterSteps

            ``` methodSignature
            public Collection<GoListStep> getFilterSteps()
            ```

        []{#iterator()}

        -   #### iterator

            ``` methodSignature
            public Iterator<Path> iterator()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `iterator` in interface `Iterable<Path>`
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

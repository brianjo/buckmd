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
[Package]{.packageLabelInType} [com.facebook.buck.cxx](package-summary.html)
:::

## Class CxxDeps.Builder {#class-cxxdeps.builder .title title="Class CxxDeps.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.CxxDeps.Builder

::: description
-   

    Enclosing class:
    :   [CxxDeps](CxxDeps.html "class in com.facebook.buck.cxx")

    ------------------------------------------------------------------------

        public static class CxxDeps.Builder
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                                           Description
          ------------------- ---------------------------------------------------------------------------------------------------------------- -------------
          `CxxDeps.Builder`   `addDep​(BuildTarget target)`                                                                                      
          `CxxDeps.Builder`   `addDep​(SourcePath path)`                                                                                         
          `CxxDeps.Builder`   `addDep​(Optional<SourcePath> path)`                                                                               
          `CxxDeps.Builder`   `addDeps​(CxxDeps cxxDeps)`                                                                                        
          `CxxDeps.Builder`   `addDeps​(Iterable<BuildTarget> targets)`                                                                          
          `CxxDeps.Builder`   `addPlatformDeps​(PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<BuildTarget>> targets)`    
          `CxxDeps`           `build()`                                                                                                         

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
    -   []{#method.detail}

        ### Method Detail

        []{#addDep(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addDep

            ``` methodSignature
            public CxxDeps.Builder addDep​(SourcePath path)
            ```

        []{#addDep(java.util.Optional)}

        -   #### addDep

            ``` methodSignature
            public CxxDeps.Builder addDep​(Optional<SourcePath> path)
            ```

        []{#addDep(com.facebook.buck.core.model.BuildTarget)}

        -   #### addDep

            ``` methodSignature
            public CxxDeps.Builder addDep​(BuildTarget target)
            ```

        []{#addDeps(java.lang.Iterable)}

        -   #### addDeps

            ``` methodSignature
            public CxxDeps.Builder addDeps​(Iterable<BuildTarget> targets)
            ```

        []{#addPlatformDeps(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### addPlatformDeps

            ``` methodSignature
            public CxxDeps.Builder addPlatformDeps​(PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<BuildTarget>> targets)
            ```

        []{#addDeps(com.facebook.buck.cxx.CxxDeps)}

        -   #### addDeps

            ``` methodSignature
            public CxxDeps.Builder addDeps​(CxxDeps cxxDeps)
            ```

        []{#build()}

        -   #### build

            ``` methodSignature
            public CxxDeps build()
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

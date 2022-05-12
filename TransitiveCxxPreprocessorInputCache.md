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
[Package]{.packageLabelInType} [com.facebook.buck.cxx](package-summary.html)
:::

## Class TransitiveCxxPreprocessorInputCache {#class-transitivecxxpreprocessorinputcache .title title="Class TransitiveCxxPreprocessorInputCache"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.TransitiveCxxPreprocessorInputCache

::: description
-   

    ------------------------------------------------------------------------

        public class TransitiveCxxPreprocessorInputCache
        extends Object

    ::: block
    Transitive C++ preprocessor input cache
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                 Description
          --------------------------------------------------------------------------- -------------
          `TransitiveCxxPreprocessorInputCache​(CxxPreprocessorDep preprocessorDep)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static com.google    | `co                   |                       |
        | .common.collect.Immut | mputeTransitiveCxxToP |                       |
        | ableMap<BuildTarget,​C | reprocessorInputMap​(C |                       |
        | xxPreprocessorInput>` | xxPlatform key,       |                       |
        |                       |                       |                       |
        |                       |                 CxxPr |                       |
        |                       | eprocessorDep preproc |                       |
        |                       | essorDep,             |                       |
        |                       |                       |                       |
        |                       |           boolean inc |                       |
        |                       | ludeDep,              |                       |
        |                       |                       |                       |
        |                       |          ActionGraphB |                       |
        |                       | uilder graphBuilder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `getUnchecked         | ::: block             |
        | .common.collect.Immut | ​(CxxPlatform key,     | Get a value from the  |
        | ableMap<BuildTarget,​C |          ActionGraphB | cache                 |
        | xxPreprocessorInput>` | uilder graphBuilder)` | :::                   |
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.cxx.CxxPreprocessorDep)}

        -   #### TransitiveCxxPreprocessorInputCache

                public TransitiveCxxPreprocessorInputCache​(CxxPreprocessorDep preprocessorDep)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getUnchecked(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getUnchecked

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<BuildTarget,​CxxPreprocessorInput> getUnchecked​(CxxPlatform key,
                                                                                                               ActionGraphBuilder graphBuilder)
            ```

            ::: block
            Get a value from the cache
            :::

        []{#computeTransitiveCxxToPreprocessorInputMap(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.cxx.CxxPreprocessorDep,boolean,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### computeTransitiveCxxToPreprocessorInputMap

            ``` methodSignature
            public static com.google.common.collect.ImmutableMap<BuildTarget,​CxxPreprocessorInput> computeTransitiveCxxToPreprocessorInputMap​(@Nonnull
                                                                                                                                                    CxxPlatform key,
                                                                                                                                                    CxxPreprocessorDep preprocessorDep,
                                                                                                                                                    boolean includeDep,
                                                                                                                                                    ActionGraphBuilder graphBuilder)
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

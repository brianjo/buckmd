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
[Package]{.packageLabelInType} [com.facebook.buck.android](package-summary.html)
:::

## Class AndroidLibraryGraphEnhancer {#class-androidlibrarygraphenhancer .title title="Class AndroidLibraryGraphEnhancer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.AndroidLibraryGraphEnhancer

::: description
-   

    ------------------------------------------------------------------------

        public class AndroidLibraryGraphEnhancer
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                       Description
          ------------------- --------------------------- -------------
          `static Flavor`     `DUMMY_R_DOT_JAVA_FLAVOR`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    Description
          -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `AndroidLibraryGraphEnhancer​(BuildTarget buildTarget,                            ProjectFilesystem projectFilesystem,                            SortedSet<BuildRule> buildRuleDeps,                            Javac javac,                            JavacOptions javacOptions,                            DependencyMode resourceDependencyMode,                            boolean forceFinalResourceIds,                            Optional<String> resourceUnionPackage,                            Optional<String> finalRName,                            boolean useOldStyleableFormat,                            boolean skipNonUnionRDotJava)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type           Method                                                                                                                                  Description
          --------------------------- --------------------------------------------------------------------------------------------------------------------------------------- -------------
          `Optional<DummyRDotJava>`   `getBuildableForAndroidResources​(ActionGraphBuilder graphBuilder,                                boolean createBuildableIfEmptyDeps)`    
          `static BuildTarget`        `getDummyRDotJavaTarget​(BuildTarget buildTarget)`                                                                                        

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
    -   []{#field.detail}

        ### Field Detail

        []{#DUMMY_R_DOT_JAVA_FLAVOR}

        -   #### DUMMY_R\_DOT_JAVA_FLAVOR

                public static final Flavor DUMMY_R_DOT_JAVA_FLAVOR
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,java.util.SortedSet,com.facebook.buck.jvm.java.Javac,com.facebook.buck.jvm.java.JavacOptions,com.facebook.buck.util.DependencyMode,boolean,java.util.Optional,java.util.Optional,boolean,boolean)}

        -   #### AndroidLibraryGraphEnhancer

                public AndroidLibraryGraphEnhancer​(BuildTarget buildTarget,
                                                   ProjectFilesystem projectFilesystem,
                                                   SortedSet<BuildRule> buildRuleDeps,
                                                   Javac javac,
                                                   JavacOptions javacOptions,
                                                   DependencyMode resourceDependencyMode,
                                                   boolean forceFinalResourceIds,
                                                   Optional<String> resourceUnionPackage,
                                                   Optional<String> finalRName,
                                                   boolean useOldStyleableFormat,
                                                   boolean skipNonUnionRDotJava)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getDummyRDotJavaTarget(com.facebook.buck.core.model.BuildTarget)}

        -   #### getDummyRDotJavaTarget

            ``` methodSignature
            public static BuildTarget getDummyRDotJavaTarget​(BuildTarget buildTarget)
            ```

        []{#getBuildableForAndroidResources(com.facebook.buck.core.rules.ActionGraphBuilder,boolean)}

        -   #### getBuildableForAndroidResources

            ``` methodSignature
            public Optional<DummyRDotJava> getBuildableForAndroidResources​(ActionGraphBuilder graphBuilder,
                                                                           boolean createBuildableIfEmptyDeps)
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

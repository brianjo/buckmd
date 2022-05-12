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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java](package-summary.html)
:::

## Class JavaLibraryRules {#class-javalibraryrules .title title="Class JavaLibraryRules"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.JavaLibraryRules

::: description
-   

    ------------------------------------------------------------------------

        public class JavaLibraryRules
        extends Object

    ::: block
    Common utilities for working with
    [`JavaLibrary`](../core/JavaLibrary.html "interface in com.facebook.buck.jvm.core")
    objects.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                    Method                                                                                                                                         Description
          -------------------------------------------------------------------- ---------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `static com.google.common.collect.ImmutableSortedSet<BuildRule>`     `getAbiRules​(ActionGraphBuilder graphBuilder,            Iterable<BuildRule> inputs)`                                                           
          `static com.google.common.collect.ImmutableMap<String,​SourcePath>`   `getNativeLibraries​(Iterable<BuildRule> deps,                   CxxPlatform cxxPlatform,                   ActionGraphBuilder graphBuilder)`    
          `static com.google.common.collect.ImmutableSortedSet<BuildRule>`     `getSourceOnlyAbiRules​(ActionGraphBuilder graphBuilder,                      Iterable<BuildRule> inputs)`                                       

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
    -   []{#method.detail}

        ### Method Detail

        []{#getNativeLibraries(java.lang.Iterable,com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getNativeLibraries

            ``` methodSignature
            public static com.google.common.collect.ImmutableMap<String,​SourcePath> getNativeLibraries​(Iterable<BuildRule> deps,
                                                                                                             CxxPlatform cxxPlatform,
                                                                                                             ActionGraphBuilder graphBuilder)
            ```

            [Returns:]{.returnLabel}
            :   all the transitive native libraries a rule depends on,
                represented as a map from their system-specific library
                names to their
                [`SourcePath`](../../core/sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")
                objects.

        []{#getAbiRules(com.facebook.buck.core.rules.ActionGraphBuilder,java.lang.Iterable)}

        -   #### getAbiRules

            ``` methodSignature
            public static com.google.common.collect.ImmutableSortedSet<BuildRule> getAbiRules​(ActionGraphBuilder graphBuilder,
                                                                                              Iterable<BuildRule> inputs)
            ```

        []{#getSourceOnlyAbiRules(com.facebook.buck.core.rules.ActionGraphBuilder,java.lang.Iterable)}

        -   #### getSourceOnlyAbiRules

            ``` methodSignature
            public static com.google.common.collect.ImmutableSortedSet<BuildRule> getSourceOnlyAbiRules​(ActionGraphBuilder graphBuilder,
                                                                                                        Iterable<BuildRule> inputs)
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

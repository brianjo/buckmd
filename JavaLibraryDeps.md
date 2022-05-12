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
-   [Nested](#nested.class.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java](package-summary.html)
:::

## Class JavaLibraryDeps {#class-javalibrarydeps .title title="Class JavaLibraryDeps"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.JavaLibraryDeps

::: description
-   

    ------------------------------------------------------------------------

        public abstract class JavaLibraryDeps
        extends Object

    ::: block
    Holds dependencies from a
    [`JavaLibraryDescription.CoreArg`](JavaLibraryDescription.CoreArg.html "interface in com.facebook.buck.jvm.java")
    after they\'ve been resolved from
    [`BuildTarget`](../../core/model/BuildTarget.html "class in com.facebook.buck.core.model")s
    to
    [`BuildRule`](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")s,
    including resolving queries and (TODO:jkeljo) exports.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                       Description
          ------------------- --------------------------- -------------
          `static class `     `JavaLibraryDeps.Builder`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor           Description
          --------------------- -------------
          `JavaLibraryDeps()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                           Method                                                                                                                                                                                                Description
          ----------------------------------------------------------- ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `com.google.common.collect.ImmutableSortedSet<BuildRule>`   `getDeps()`                                                                                                                                                                                            
          `com.google.common.collect.ImmutableSortedSet<BuildRule>`   `getExportedDeps()`                                                                                                                                                                                    
          `com.google.common.collect.ImmutableSortedSet<BuildRule>`   `getExportedProvidedDeps()`                                                                                                                                                                            
          `com.google.common.collect.ImmutableSortedSet<BuildRule>`   `getProvidedDeps()`                                                                                                                                                                                    
          `com.google.common.collect.ImmutableSortedSet<BuildRule>`   `getRuntimeDeps()`                                                                                                                                                                                     
          `com.google.common.collect.ImmutableSortedSet<BuildRule>`   `getSourceOnlyAbiDeps()`                                                                                                                                                                               
          `static JavaLibraryDeps`                                    `newInstance​(JavaLibraryDescription.CoreArg args,            BuildRuleResolver resolver,            TargetConfiguration targetConfiguration,            ConfiguredCompilerFactory compilerFactory)`    

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

        []{#<init>()}

        -   #### JavaLibraryDeps

                public JavaLibraryDeps()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#newInstance(com.facebook.buck.jvm.java.JavaLibraryDescription.CoreArg,com.facebook.buck.core.rules.BuildRuleResolver,com.facebook.buck.core.model.TargetConfiguration,com.facebook.buck.jvm.java.ConfiguredCompilerFactory)}

        -   #### newInstance

            ``` methodSignature
            public static JavaLibraryDeps newInstance​(JavaLibraryDescription.CoreArg args,
                                                      BuildRuleResolver resolver,
                                                      TargetConfiguration targetConfiguration,
                                                      ConfiguredCompilerFactory compilerFactory)
            ```

        []{#getDeps()}

        -   #### getDeps

            ``` methodSignature
            @Lazy
            public com.google.common.collect.ImmutableSortedSet<BuildRule> getDeps()
            ```

        []{#getProvidedDeps()}

        -   #### getProvidedDeps

            ``` methodSignature
            @Lazy
            public com.google.common.collect.ImmutableSortedSet<BuildRule> getProvidedDeps()
            ```

        []{#getExportedDeps()}

        -   #### getExportedDeps

            ``` methodSignature
            @Lazy
            public com.google.common.collect.ImmutableSortedSet<BuildRule> getExportedDeps()
            ```

        []{#getExportedProvidedDeps()}

        -   #### getExportedProvidedDeps

            ``` methodSignature
            @Lazy
            public com.google.common.collect.ImmutableSortedSet<BuildRule> getExportedProvidedDeps()
            ```

        []{#getSourceOnlyAbiDeps()}

        -   #### getSourceOnlyAbiDeps

            ``` methodSignature
            @Lazy
            public com.google.common.collect.ImmutableSortedSet<BuildRule> getSourceOnlyAbiDeps()
            ```

        []{#getRuntimeDeps()}

        -   #### getRuntimeDeps

            ``` methodSignature
            @Lazy
            public com.google.common.collect.ImmutableSortedSet<BuildRule> getRuntimeDeps()
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
-   [Nested](#nested.class.summary) \| 
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

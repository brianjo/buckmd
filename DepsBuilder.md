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

## Class DepsBuilder {#class-depsbuilder .title title="Class DepsBuilder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.DepsBuilder

::: description
-   

    ------------------------------------------------------------------------

        public class DepsBuilder
        extends Object

    ::: block
    Builder suitable for generating the dependency list of a build rule.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                      Description
          ------------------------------------------------ -------------
          `DepsBuilder​(SourcePathRuleFinder ruleFinder)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                           Method                                                       Description
          ----------------------------------------------------------- ------------------------------------------------------------ -------------
          `DepsBuilder`                                               `add​(BuildRule buildRule)`                                    
          `DepsBuilder`                                               `add​(SourcePath sourcePath)`                                  
          `DepsBuilder`                                               `add​(com.facebook.buck.cxx.CompilerDelegate delegate)`        
          `DepsBuilder`                                               `add​(CxxSource source)`                                       
          `DepsBuilder`                                               `add​(com.facebook.buck.cxx.PreprocessorDelegate delegate)`    
          `com.google.common.collect.ImmutableSortedSet<BuildRule>`   `build()`                                                     

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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.rules.SourcePathRuleFinder)}

        -   #### DepsBuilder

                public DepsBuilder​(SourcePathRuleFinder ruleFinder)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#build()}

        -   #### build

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<BuildRule> build()
            ```

        []{#add(com.facebook.buck.cxx.CxxSource)}

        -   #### add

            ``` methodSignature
            public DepsBuilder add​(CxxSource source)
            ```

        []{#add(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### add

            ``` methodSignature
            public DepsBuilder add​(SourcePath sourcePath)
            ```

        []{#add(com.facebook.buck.core.rules.BuildRule)}

        -   #### add

            ``` methodSignature
            public DepsBuilder add​(BuildRule buildRule)
            ```

        []{#add(com.facebook.buck.cxx.PreprocessorDelegate)}

        -   #### add

            ``` methodSignature
            public DepsBuilder add​(com.facebook.buck.cxx.PreprocessorDelegate delegate)
            ```

        []{#add(com.facebook.buck.cxx.CompilerDelegate)}

        -   #### add

            ``` methodSignature
            public DepsBuilder add​(com.facebook.buck.cxx.CompilerDelegate delegate)
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

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

## Class CxxPreprocessorInput {#class-cxxpreprocessorinput .title title="Class CxxPreprocessorInput"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.CxxPreprocessorInput

::: description
-   

    ------------------------------------------------------------------------

        public abstract class CxxPreprocessorInput
        extends Object

    ::: block
    The components that get contributed to a top-level run of the C++
    preprocessor.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                            Description
          ------------------- -------------------------------- -------------
          `static class `     `CxxPreprocessorInput.Builder`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                Description
          -------------------------- -------------
          `CxxPreprocessorInput()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                          Method                                            Description
          -------------------------------------------------------------------------- ------------------------------------------------- -------------
          `static CxxPreprocessorInput.Builder`                                      `builder()`                                        
          `static CxxPreprocessorInput`                                              `concat​(Iterable<CxxPreprocessorInput> inputs)`    
          `Iterable<BuildRule>`                                                      `getDeps​(BuildRuleResolver ruleResolver)`          
          `abstract com.google.common.collect.ImmutableSet<FrameworkPath>`           `getFrameworks()`                                  
          `abstract com.google.common.collect.ImmutableList<CxxHeaders>`             `getIncludes()`                                    
          `abstract com.google.common.collect.Multimap<CxxSource.Type,​Arg>`          `getPreprocessorFlags()`                           
          `protected abstract com.google.common.collect.ImmutableSet<BuildTarget>`   `getRules()`                                       
          `static CxxPreprocessorInput`                                              `of()`                                             

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
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

        -   #### CxxPreprocessorInput

                public CxxPreprocessorInput()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getPreprocessorFlags()}

        -   #### getPreprocessorFlags

            ``` methodSignature
            public abstract com.google.common.collect.Multimap<CxxSource.Type,​Arg> getPreprocessorFlags()
            ```

        []{#getIncludes()}

        -   #### getIncludes

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<CxxHeaders> getIncludes()
            ```

        []{#getFrameworks()}

        -   #### getFrameworks

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSet<FrameworkPath> getFrameworks()
            ```

        []{#getRules()}

        -   #### getRules

            ``` methodSignature
            protected abstract com.google.common.collect.ImmutableSet<BuildTarget> getRules()
            ```

        []{#getDeps(com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### getDeps

            ``` methodSignature
            public Iterable<BuildRule> getDeps​(BuildRuleResolver ruleResolver)
            ```

        []{#concat(java.lang.Iterable)}

        -   #### concat

            ``` methodSignature
            public static CxxPreprocessorInput concat​(Iterable<CxxPreprocessorInput> inputs)
            ```

        []{#of()}

        -   #### of

            ``` methodSignature
            public static CxxPreprocessorInput of()
            ```

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static CxxPreprocessorInput.Builder builder()
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

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
[Package]{.packageLabelInType} [com.facebook.buck.cxx](package-summary.html)
:::

## Class CxxDeps {#class-cxxdeps .title title="Class CxxDeps"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.CxxDeps

::: description
-   

    ------------------------------------------------------------------------

        public abstract class CxxDeps
        extends Object

    ::: block
    The group of
    [`BuildTarget`](../core/model/BuildTarget.html "class in com.facebook.buck.core.model")s
    from C/C++ constructor args which comprise a C/C++ descriptions
    logical C/C++ deps used to find dependency
    [`NativeLinkableGroup`](toolchain/nativelink/NativeLinkableGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink")s
    or
    [`CxxPreprocessorDep`](CxxPreprocessorDep.html "interface in com.facebook.buck.cxx")s.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class               Description
          ------------------- ------------------- -------------
          `static class `     `CxxDeps.Builder`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field              Description
          ------------------- ------------------ -------------
          `static CxxDeps`    `EMPTY_INSTANCE`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor   Description
          ------------- -------------
          `CxxDeps()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                                                                                         Method                                                                                      Description
          ----------------------------------------------------------------------------------------------------------------------------------------- ------------------------------------------------------------------------------------------- -------------
          `static CxxDeps.Builder`                                                                                                                  `builder()`                                                                                  
          `static CxxDeps.Builder`                                                                                                                  `builder​(CxxDeps deps)`                                                                      
          `static CxxDeps`                                                                                                                          `concat​(CxxDeps... cxxDeps)`                                                                 
          `static CxxDeps`                                                                                                                          `concat​(Iterable<CxxDeps> cxxDeps)`                                                          
          `void`                                                                                                                                    `forEach​(CxxPlatform platform,        java.util.function.Consumer<BuildTarget> consumer)`    
          `void`                                                                                                                                    `forEachForAllPlatforms​(java.util.function.Consumer<BuildTarget> consumer)`                  
          `com.google.common.collect.ImmutableSet<BuildRule>`                                                                                       `get​(BuildRuleResolver resolver,    CxxPlatform cxxPlatform)`                                
          `abstract com.google.common.collect.ImmutableList<BuildTarget>`                                                                           `getDeps()`                                                                                  
          `com.google.common.collect.ImmutableSet<BuildRule>`                                                                                       `getForAllPlatforms​(BuildRuleResolver resolver)`                                             
          `abstract com.google.common.collect.ImmutableList<PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<BuildTarget>>>`   `getPlatformDeps()`                                                                          

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
    -   []{#field.detail}

        ### Field Detail

        []{#EMPTY_INSTANCE}

        -   #### EMPTY_INSTANCE

                public static final CxxDeps EMPTY_INSTANCE
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### CxxDeps

                public CxxDeps()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getDeps()}

        -   #### getDeps

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<BuildTarget> getDeps()
            ```

        []{#getPlatformDeps()}

        -   #### getPlatformDeps

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<BuildTarget>>> getPlatformDeps()
            ```

        []{#forEachForAllPlatforms(java.util.function.Consumer)}

        -   #### forEachForAllPlatforms

            ``` methodSignature
            public void forEachForAllPlatforms​(java.util.function.Consumer<BuildTarget> consumer)
            ```

        []{#getForAllPlatforms(com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### getForAllPlatforms

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<BuildRule> getForAllPlatforms​(BuildRuleResolver resolver)
            ```

        []{#forEach(com.facebook.buck.cxx.toolchain.CxxPlatform,java.util.function.Consumer)}

        -   #### forEach

            ``` methodSignature
            public void forEach​(CxxPlatform platform,
                                java.util.function.Consumer<BuildTarget> consumer)
            ```

        []{#get(com.facebook.buck.core.rules.BuildRuleResolver,com.facebook.buck.cxx.toolchain.CxxPlatform)}

        -   #### get

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<BuildRule> get​(BuildRuleResolver resolver,
                                                                         CxxPlatform cxxPlatform)
            ```

        []{#concat(java.lang.Iterable)}

        -   #### concat

            ``` methodSignature
            public static CxxDeps concat​(Iterable<CxxDeps> cxxDeps)
            ```

        []{#concat(com.facebook.buck.cxx.CxxDeps...)}

        -   #### concat

            ``` methodSignature
            public static CxxDeps concat​(CxxDeps... cxxDeps)
            ```

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static CxxDeps.Builder builder()
            ```

        []{#builder(com.facebook.buck.cxx.CxxDeps)}

        -   #### builder

            ``` methodSignature
            public static CxxDeps.Builder builder​(CxxDeps deps)
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

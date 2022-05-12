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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java](package-summary.html)
:::

## Class JavaTestDescription.CxxLibraryEnhancement {#class-javatestdescription.cxxlibraryenhancement .title title="Class JavaTestDescription.CxxLibraryEnhancement"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.JavaTestDescription.CxxLibraryEnhancement

::: description
-   

    Enclosing class:
    :   [JavaTestDescription](JavaTestDescription.html "class in com.facebook.buck.jvm.java")

    ------------------------------------------------------------------------

        public static class JavaTestDescription.CxxLibraryEnhancement
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                                         Field                     Description
          --------------------------------------------------------- ------------------------- -------------
          `com.google.common.collect.ImmutableMap<String,​String>`   `nativeLibsEnvironment`    
          `BuildRuleParams`                                         `updatedParams`            

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                         Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `CxxLibraryEnhancement​(BuildTarget buildTarget,                      ProjectFilesystem projectFilesystem,                      BuildRuleParams params,                      Optional<Boolean> useCxxLibraries,                      com.google.common.collect.ImmutableSet<BuildTarget> cxxLibraryWhitelist,                      ActionGraphBuilder graphBuilder,                      CxxPlatform cxxPlatform)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type            Method                                                                                                                                                                                                                                                                                                              Description
          ---------------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `static MappedSymlinkTree`   `buildNativeLibsSymlinkTreeRule​(BuildTarget buildTarget,                               ProjectFilesystem projectFilesystem,                               ActionGraphBuilder graphBuilder,                               BuildRuleParams buildRuleParams,                               CxxPlatform cxxPlatform)`    

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

        []{#updatedParams}

        -   #### updatedParams

                public final BuildRuleParams updatedParams

        []{#nativeLibsEnvironment}

        -   #### nativeLibsEnvironment

                public final com.google.common.collect.ImmutableMap<String,​String> nativeLibsEnvironment
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams,java.util.Optional,com.google.common.collect.ImmutableSet,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.cxx.toolchain.CxxPlatform)}

        -   #### CxxLibraryEnhancement

                public CxxLibraryEnhancement​(BuildTarget buildTarget,
                                             ProjectFilesystem projectFilesystem,
                                             BuildRuleParams params,
                                             Optional<Boolean> useCxxLibraries,
                                             com.google.common.collect.ImmutableSet<BuildTarget> cxxLibraryWhitelist,
                                             ActionGraphBuilder graphBuilder,
                                             CxxPlatform cxxPlatform)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#buildNativeLibsSymlinkTreeRule(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.cxx.toolchain.CxxPlatform)}

        -   #### buildNativeLibsSymlinkTreeRule

            ``` methodSignature
            public static MappedSymlinkTree buildNativeLibsSymlinkTreeRule​(BuildTarget buildTarget,
                                                                           ProjectFilesystem projectFilesystem,
                                                                           ActionGraphBuilder graphBuilder,
                                                                           BuildRuleParams buildRuleParams,
                                                                           CxxPlatform cxxPlatform)
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

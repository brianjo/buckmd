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

## Class MachoDylibStubRuleFactory {#class-machodylibstubrulefactory .title title="Class MachoDylibStubRuleFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.MachoDylibStubRuleFactory

::: description
-   

    All Implemented Interfaces:
    :   `SharedLibraryInterfaceFactory`

    ------------------------------------------------------------------------

        public abstract class MachoDylibStubRuleFactory
        extends Object
        implements SharedLibraryInterfaceFactory

    ::: block
    Factor which can create rules for scrubbed dylib stubs
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                     Description
          ------------------------------- -------------
          `MachoDylibStubRuleFactory()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                    Method                                                                                                                                                                                                                                                                                                                                                                                                                                                    Description
          ------------------------------------ --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `BuildRule`                          `createSharedInterfaceLibraryFromLibrary​(BuildTarget target,                                        ProjectFilesystem projectFilesystem,                                        BuildRuleResolver resolver,                                        CxxPlatform cxxPlatform,                                        SourcePath library)`                                                                                                                    
          `BuildRule`                          `createSharedInterfaceLibraryFromLinkableInput​(BuildTarget target,                                              ProjectFilesystem projectFilesystem,                                              BuildRuleResolver resolver,                                              String libName,                                              Linker linker,                                              com.google.common.collect.ImmutableList<Arg> args)`    
          `static MachoDylibStubRuleFactory`   `from​(MachoDylibStubParams params)`                                                                                                                                                                                                                                                                                                                                                                                                                        

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

        -   #### MachoDylibStubRuleFactory

                public MachoDylibStubRuleFactory()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#createSharedInterfaceLibraryFromLibrary(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleResolver,com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### createSharedInterfaceLibraryFromLibrary

            ``` methodSignature
            public BuildRule createSharedInterfaceLibraryFromLibrary​(BuildTarget target,
                                                                     ProjectFilesystem projectFilesystem,
                                                                     BuildRuleResolver resolver,
                                                                     CxxPlatform cxxPlatform,
                                                                     SourcePath library)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `createSharedInterfaceLibraryFromLibrary` in
                interface `SharedLibraryInterfaceFactory`

            [Returns:]{.returnLabel}
            :   a rule building a shared library interface from an
                existing shared library.

        []{#createSharedInterfaceLibraryFromLinkableInput(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleResolver,java.lang.String,com.facebook.buck.cxx.toolchain.linker.Linker,com.google.common.collect.ImmutableList)}

        -   #### createSharedInterfaceLibraryFromLinkableInput

            ``` methodSignature
            public BuildRule createSharedInterfaceLibraryFromLinkableInput​(BuildTarget target,
                                                                           ProjectFilesystem projectFilesystem,
                                                                           BuildRuleResolver resolver,
                                                                           String libName,
                                                                           Linker linker,
                                                                           com.google.common.collect.ImmutableList<Arg> args)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `createSharedInterfaceLibraryFromLinkableInput` in
                interface `SharedLibraryInterfaceFactory`

            [Returns:]{.returnLabel}
            :   a rule building a shared library interface from a shared
                link line

        []{#from(com.facebook.buck.cxx.toolchain.MachoDylibStubParams)}

        -   #### from

            ``` methodSignature
            public static MachoDylibStubRuleFactory from​(MachoDylibStubParams params)
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

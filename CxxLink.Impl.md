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

## Class CxxLink.Impl {#class-cxxlink.impl .title title="Class CxxLink.Impl"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.CxxLink.Impl

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`, `Buildable`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [CxxLink](CxxLink.html "class in com.facebook.buck.cxx")

    ------------------------------------------------------------------------

        public static class CxxLink.Impl
        extends Object
        implements Buildable

    ::: block
    Buildable implementation of CxxLink.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                Description
          -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `Impl​(Linker linker,     Path output,     com.google.common.collect.ImmutableMap<String,​Path> extraOutputs,     com.google.common.collect.ImmutableList<Arg> args,     Optional<LinkOutputPostprocessor> postprocessor,     boolean thinLto,     boolean fatLto,     BuildTarget buildTarget,     com.google.common.collect.ImmutableSortedSet<Path> relativeCellRoots)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                 Method                                                                                                                                                                                                 Description
          ------------------------------------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `com.google.common.collect.ImmutableList<Step>`   `getBuildSteps​(BuildContext context,              ProjectFilesystem filesystem,              OutputPathResolver outputPathResolver,              BuildCellRelativePathFactory buildCellPathFactory)`    

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

        []{#<init>(com.facebook.buck.cxx.toolchain.linker.Linker,java.nio.file.Path,com.google.common.collect.ImmutableMap,com.google.common.collect.ImmutableList,java.util.Optional,boolean,boolean,com.facebook.buck.core.model.BuildTarget,com.google.common.collect.ImmutableSortedSet)}

        -   #### Impl

                public Impl​(Linker linker,
                            Path output,
                            com.google.common.collect.ImmutableMap<String,​Path> extraOutputs,
                            com.google.common.collect.ImmutableList<Arg> args,
                            Optional<LinkOutputPostprocessor> postprocessor,
                            boolean thinLto,
                            boolean fatLto,
                            BuildTarget buildTarget,
                            com.google.common.collect.ImmutableSortedSet<Path> relativeCellRoots)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBuildSteps(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.rules.modern.OutputPathResolver,com.facebook.buck.rules.modern.BuildCellRelativePathFactory)}

        -   #### getBuildSteps

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Step> getBuildSteps​(BuildContext context,
                                                                               ProjectFilesystem filesystem,
                                                                               OutputPathResolver outputPathResolver,
                                                                               BuildCellRelativePathFactory buildCellPathFactory)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildSteps` in interface `Buildable`
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

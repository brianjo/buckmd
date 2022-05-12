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
[Package]{.packageLabelInType} [com.facebook.buck.cxx](package-summary.html)
:::

## Class CxxPrepareForLinkStep {#class-cxxprepareforlinkstep .title title="Class CxxPrepareForLinkStep"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.CxxPrepareForLinkStep

::: description
-   

    ------------------------------------------------------------------------

        public class CxxPrepareForLinkStep
        extends Object

    ::: block
    Prepares argfile for the CxxLinkStep, so all arguments to the linker
    will be stored in a single file. CxxLinkStep then would pass it to
    the linker via \@path/to/the.argsfile command. This allows us to
    break the constraints that command line sets for the maximum length
    of the commands.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                        Method                                                                                                                                                                                                                                                                                                                 Description
          -------------------------------------------------------- ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `static com.google.common.collect.ImmutableList<Step>`   `create​(Path argFilePath,       Path fileListPath,       Iterable<Arg> linkerArgsToSupportFileList,       Path output,       com.google.common.collect.ImmutableList<Arg> args,       Linker linker,       CanonicalCellName currentCellName,       Path currentCellPath,       SourcePathResolverAdapter resolver)`    

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

        []{#create(java.nio.file.Path,java.nio.file.Path,java.lang.Iterable,java.nio.file.Path,com.google.common.collect.ImmutableList,com.facebook.buck.cxx.toolchain.linker.Linker,com.facebook.buck.core.cell.name.CanonicalCellName,java.nio.file.Path,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### create

            ``` methodSignature
            public static com.google.common.collect.ImmutableList<Step> create​(Path argFilePath,
                                                                               Path fileListPath,
                                                                               Iterable<Arg> linkerArgsToSupportFileList,
                                                                               Path output,
                                                                               com.google.common.collect.ImmutableList<Arg> args,
                                                                               Linker linker,
                                                                               CanonicalCellName currentCellName,
                                                                               Path currentCellPath,
                                                                               SourcePathResolverAdapter resolver)
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

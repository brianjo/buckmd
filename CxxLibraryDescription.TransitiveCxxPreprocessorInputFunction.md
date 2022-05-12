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

## Interface CxxLibraryDescription.TransitiveCxxPreprocessorInputFunction {#interface-cxxlibrarydescription.transitivecxxpreprocessorinputfunction .title title="Interface CxxLibraryDescription.TransitiveCxxPreprocessorInputFunction"}
:::

::: contentContainer
::: description
-   

    Enclosing class:
    :   [CxxLibraryDescription](CxxLibraryDescription.html "class in com.facebook.buck.cxx")

    ```{=html}
    <!-- -->
    ```

    Functional Interface:
    :   This is a functional interface and can therefore be used as the
        assignment target for a lambda expression or method reference.

    ------------------------------------------------------------------------

        @FunctionalInterface
        public static interface CxxLibraryDescription.TransitiveCxxPreprocessorInputFunction

    ::: block
    This is a hack to allow fine grained control over how the transitive
    `  CxxPreprocessorInput`s are found. Since not all `Description`s
    which use `  CxxLibraryDescription` generate a `CxxLibrary`,
    blinding attempting to require it will not work.
    Therefore for those other rules, we create the list from scratch.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `java                 | `apply​(BuildTa        |                       |
        | .util.stream.Stream<C | rget target,      Act |                       |
        | xxPreprocessorInput>` | ionGraphBuilder graph |                       |
        |                       | Builder,      CxxPlat |                       |
        |                       | form cxxPlatform,     |                       |
        |                       |   com.google.common.c |                       |
        |                       | ollect.ImmutableSet<B |                       |
        |                       | uildRule> deps,       |                       |
        |                       | CxxDeps privateDeps)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `stati                | `fromDeps()`          | ::: block             |
        | c CxxLibraryDescripti |                       | Retrieve the          |
        | on.TransitiveCxxPrepr |                       | transitive            |
        | ocessorInputFunction` |                       | [`CxxPreprocessorInpu |
        |                       |                       | t`](CxxPreprocessorIn |
        |                       |                       | put.html "class in co |
        |                       |                       | m.facebook.buck.cxx") |
        |                       |                       | from an explicitly    |
        |                       |                       | specified deps list.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `stati                | `fromLibraryRule()`   | ::: block             |
        | c CxxLibraryDescripti |                       | Retrieve the          |
        | on.TransitiveCxxPrepr |                       | transitive            |
        | ocessorInputFunction` |                       | CxxPreprocessorInput  |
        |                       |                       | from the CxxLibrary   |
        |                       |                       | rule.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#apply(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.cxx.toolchain.CxxPlatform,com.google.common.collect.ImmutableSet,com.facebook.buck.cxx.CxxDeps)}

        -   #### apply

            ``` methodSignature
            java.util.stream.Stream<CxxPreprocessorInput> apply​(BuildTarget target,
                                                                ActionGraphBuilder graphBuilder,
                                                                CxxPlatform cxxPlatform,
                                                                com.google.common.collect.ImmutableSet<BuildRule> deps,
                                                                CxxDeps privateDeps)
            ```

        []{#fromLibraryRule()}

        -   #### fromLibraryRule

            ``` methodSignature
            static CxxLibraryDescription.TransitiveCxxPreprocessorInputFunction fromLibraryRule()
            ```

            ::: block
            Retrieve the transitive CxxPreprocessorInput from the
            CxxLibrary rule.
            This is used by CxxLibrary and AppleLibrary. Rules that do
            not generate a CxxLibrary rule (namely AppleTest) cannot use
            this.
            :::

        []{#fromDeps()}

        -   #### fromDeps

            ``` methodSignature
            static CxxLibraryDescription.TransitiveCxxPreprocessorInputFunction fromDeps()
            ```

            ::: block
            Retrieve the transitive
            [`CxxPreprocessorInput`](CxxPreprocessorInput.html "class in com.facebook.buck.cxx")
            from an explicitly specified deps list.
            This is used by AppleTest, which doesn\'t generate a
            CxxLibrary rule that computes this.
            :::
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

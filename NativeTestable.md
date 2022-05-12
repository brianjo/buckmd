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

## Interface NativeTestable {#interface-nativetestable .title title="Interface NativeTestable"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `AppleBundle`, `CxxBinary`, `CxxLibraryGroup`

    ------------------------------------------------------------------------

        public interface NativeTestable

    ::: block
    Interface marking a rule as having tests.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `                     | `getPrivateCxxP       | ::: block             |
        | CxxPreprocessorInput` | reprocessorInput​(CxxP | Return the            |
        |                       | latform cxxPlatform,  | [`CxxPreprocessorInpu |
        |                       |                       | t`](CxxPreprocessorIn |
        |                       |          ActionGraphB | put.html "class in co |
        |                       | uilder graphBuilder)` | m.facebook.buck.cxx") |
        |                       |                       | to expose private     |
        |                       |                       | headers of this rule. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isTestedBy​(Bui       | ::: block             |
        |                       | ldTarget testTarget)` | Return true if this   |
        |                       |                       | rule is tested by     |
        |                       |                       | `testTarget`, false   |
        |                       |                       | otherwise.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#isTestedBy(com.facebook.buck.core.model.BuildTarget)}

        -   #### isTestedBy

            ``` methodSignature
            boolean isTestedBy​(BuildTarget testTarget)
            ```

            ::: block
            Return true if this rule is tested by `testTarget`, false
            otherwise.
            :::

        []{#getPrivateCxxPreprocessorInput(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getPrivateCxxPreprocessorInput

            ``` methodSignature
            CxxPreprocessorInput getPrivateCxxPreprocessorInput​(CxxPlatform cxxPlatform,
                                                                ActionGraphBuilder graphBuilder)
            ```

            ::: block
            Return the
            [`CxxPreprocessorInput`](CxxPreprocessorInput.html "class in com.facebook.buck.cxx")
            to expose private headers of this rule. This is used to
            propagate private headers to the test testing this object.
            For convenience, tests can see private headers visible in
            the rule being tested.
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

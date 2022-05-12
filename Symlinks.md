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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.impl](package-summary.html)
:::

## Interface Symlinks {#interface-symlinks .title title="Interface Symlinks"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `AddsToRuleKey`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `SymlinkDir`, `SymlinkMap`, `SymlinkPack`

    ------------------------------------------------------------------------

        public interface Symlinks
        extends AddsToRuleKey

    ::: block
    Interface representing symlinks processed by
    [`SymlinkTree`](SymlinkTree.html "class in com.facebook.buck.core.rules.impl").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `forEachSymlinkBuil   | ::: block             |
        |                       | dDep​(SourcePathRuleFi | Run `consumer` on all |
        |                       | nder finder,          | [`BuildRule`]         |
        |                       |               java.ut | (../BuildRule.html "i |
        |                       | il.function.Consumer< | nterface in com.faceb |
        |                       | BuildRule> consumer)` | ook.buck.core.rules") |
        |                       |                       | build dependencies    |
        |                       |                       | for this group of     |
        |                       |                       | symlinks.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `forEach              | ::: block             |
        |                       | SymlinkInput​(java.uti | Run `consumer` on all |
        |                       | l.function.Consumer<S | [`SourcePath`]        |
        |                       | ourcePath> consumer)` | (../../sourcepath/Sou |
        |                       |                       | rcePath.html "interfa |
        |                       |                       | ce in com.facebook.bu |
        |                       |                       | ck.core.sourcepath")s |
        |                       |                       | in this groups of     |
        |                       |                       | links.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SymlinkPaths`        | `resolveSymlink       | ::: block             |
        |                       | Paths​(SourcePathResol | Resolve all           |
        |                       | verAdapter resolver)` | [`SourcePath`]        |
        |                       |                       | (../../sourcepath/Sou |
        |                       |                       | rcePath.html "interfa |
        |                       |                       | ce in com.facebook.bu |
        |                       |                       | ck.core.sourcepath")s |
        |                       |                       | into                  |
        |                       |                       | [`Path`](http://docs  |
        |                       |                       | .oracle.com/javase/7/ |
        |                       |                       | docs/api/java/nio/fil |
        |                       |                       | e/Path.html?is-extern |
        |                       |                       | al=true "class or int |
        |                       |                       | erface in java.nio.fi |
        |                       |                       | le"){.externalLink}s, |
        |                       |                       | represented by        |
        |                       |                       | [`Symlink             |
        |                       |                       | Paths`](../../../step |
        |                       |                       | /fs/SymlinkPaths.html |
        |                       |                       |  "interface in com.fa |
        |                       |                       | cebook.buck.step.fs") |
        |                       |                       | (for use with         |
        |                       |                       | [                     |
        |                       |                       | `SymlinkTreeMergeStep |
        |                       |                       | `](../../../step/fs/S |
        |                       |                       | ymlinkTreeMergeStep.h |
        |                       |                       | tml "class in com.fac |
        |                       |                       | ebook.buck.step.fs"). |
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

        []{#forEachSymlinkInput(java.util.function.Consumer)}

        -   #### forEachSymlinkInput

            ``` methodSignature
            void forEachSymlinkInput​(java.util.function.Consumer<SourcePath> consumer)
            ```

            ::: block
            Run `consumer` on all
            [`SourcePath`](../../sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")s
            in this groups of links. Used by
            [`SymlinkTree`](SymlinkTree.html "class in com.facebook.buck.core.rules.impl")
            to compose runtime deps.
            :::

        []{#forEachSymlinkBuildDep(com.facebook.buck.core.rules.SourcePathRuleFinder,java.util.function.Consumer)}

        -   #### forEachSymlinkBuildDep

            ``` methodSignature
            void forEachSymlinkBuildDep​(SourcePathRuleFinder finder,
                                        java.util.function.Consumer<BuildRule> consumer)
            ```

            ::: block
            Run `consumer` on all
            [`BuildRule`](../BuildRule.html "interface in com.facebook.buck.core.rules")
            build dependencies for this group of symlinks.
            :::

        []{#resolveSymlinkPaths(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### resolveSymlinkPaths

            ``` methodSignature
            SymlinkPaths resolveSymlinkPaths​(SourcePathResolverAdapter resolver)
            ```

            ::: block
            Resolve all
            [`SourcePath`](../../sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")s
            into
            [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}s,
            represented by
            [`SymlinkPaths`](../../../step/fs/SymlinkPaths.html "interface in com.facebook.buck.step.fs")
            (for use with
            [`SymlinkTreeMergeStep`](../../../step/fs/SymlinkTreeMergeStep.html "class in com.facebook.buck.step.fs").
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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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

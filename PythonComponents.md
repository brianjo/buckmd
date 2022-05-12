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
-   [Nested](#nested.class.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.features.python](package-summary.html)
:::

## Interface PythonComponents {#interface-pythoncomponents .title title="Interface PythonComponents"}
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
    :   `PythonMappedComponents`

    ------------------------------------------------------------------------

        public interface PythonComponents
        extends AddsToRuleKey

    ::: block
    Interface representing the modules, resources, etc. that
    dependencies contribute to Python binaries, used to model how these
    components should be handled by
    [`BuildRule`](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")s
    (e.g. how they\'re hashed into rule keys).
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Interface             | Description           |
        +=======================+=======================+=======================+
        | `static interface `   | `Pytho                | ::: block             |
        |                       | nComponents.Resolved` | Resolve this          |
        |                       |                       | [`Python              |
        |                       |                       | Components`](PythonCo |
        |                       |                       | mponents.html "interf |
        |                       |                       | ace in com.facebook.b |
        |                       |                       | uck.features.python") |
        |                       |                       | into a class usable   |
        |                       |                       | by                    |
        |                       |                       | [`Step`               |
        |                       |                       | ](../../step/Step.htm |
        |                       |                       | l "interface in com.f |
        |                       |                       | acebook.buck.step")s. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Symlinks`            | `asSymlinks()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `                     | ::: block             |
        |                       | forEachInput​(java.uti | Run `consumer` on all |
        |                       | l.function.Consumer<S | [`SourcePath`](../.   |
        |                       | ourcePath> consumer)` | ./core/sourcepath/Sou |
        |                       |                       | rcePath.html "interfa |
        |                       |                       | ce in com.facebook.bu |
        |                       |                       | ck.core.sourcepath")s |
        |                       |                       | contained in this     |
        |                       |                       | object.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pytho                | `resolvePythonCompo   | ::: block             |
        | nComponents.Resolved` | nents​(SourcePathResol | Convert this          |
        |                       | verAdapter resolver)` | [`Python              |
        |                       |                       | Components`](PythonCo |
        |                       |                       | mponents.html "interf |
        |                       |                       | ace in com.facebook.b |
        |                       |                       | uck.features.python") |
        |                       |                       | to a                  |
        |                       |                       | [`Pyth                |
        |                       |                       | onComponents.Resolved |
        |                       |                       | `](PythonComponents.R |
        |                       |                       | esolved.html "interfa |
        |                       |                       | ce in com.facebook.bu |
        |                       |                       | ck.features.python"), |
        |                       |                       | where all             |
        |                       |                       | [`SourcePath`](../.   |
        |                       |                       | ./core/sourcepath/Sou |
        |                       |                       | rcePath.html "interfa |
        |                       |                       | ce in com.facebook.bu |
        |                       |                       | ck.core.sourcepath")s |
        |                       |                       | have been resolved to |
        |                       |                       | [`Path`](http://doc   |
        |                       |                       | s.oracle.com/javase/7 |
        |                       |                       | /docs/api/java/nio/fi |
        |                       |                       | le/Path.html?is-exter |
        |                       |                       | nal=true "class or in |
        |                       |                       | terface in java.nio.f |
        |                       |                       | ile"){.externalLink}s |
        |                       |                       | for use with          |
        |                       |                       | [`Step`               |
        |                       |                       | ](../../step/Step.htm |
        |                       |                       | l "interface in com.f |
        |                       |                       | acebook.buck.step")s. |
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

        []{#forEachInput(java.util.function.Consumer)}

        -   #### forEachInput

            ``` methodSignature
            void forEachInput​(java.util.function.Consumer<SourcePath> consumer)
            ```

            ::: block
            Run `consumer` on all
            [`SourcePath`](../../core/sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")s
            contained in this object.
            :::

        []{#resolvePythonComponents(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### resolvePythonComponents

            ``` methodSignature
            PythonComponents.Resolved resolvePythonComponents​(SourcePathResolverAdapter resolver)
            ```

            ::: block
            Convert this
            [`PythonComponents`](PythonComponents.html "interface in com.facebook.buck.features.python")
            to a
            [`PythonComponents.Resolved`](PythonComponents.Resolved.html "interface in com.facebook.buck.features.python"),
            where all
            [`SourcePath`](../../core/sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")s
            have been resolved to
            [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}s
            for use with
            [`Step`](../../step/Step.html "interface in com.facebook.buck.step")s.
            :::

        []{#asSymlinks()}

        -   #### asSymlinks

            ``` methodSignature
            Symlinks asSymlinks()
            ```

            [Returns:]{.returnLabel}
            :   a
                [`Symlinks`](../../core/rules/impl/Symlinks.html "interface in com.facebook.buck.core.rules.impl")
                used to symlink the components contained in this object
                via a
                [`SymlinkTree`](../../core/rules/impl/SymlinkTree.html "class in com.facebook.buck.core.rules.impl")
                rule.
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
-   [Nested](#nested.class.summary) \| 
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

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
[Package]{.packageLabelInType} [com.facebook.buck.cxx.toolchain](package-summary.html)
:::

## Interface ArchiverProvider {#interface-archiverprovider .title title="Interface ArchiverProvider"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        public interface ArchiverProvider
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Interface             | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `ArchiverProvide      | ::: block             |
        |                       | r.LegacyArchiverType` | .buckconfig accepts   |
        |                       |                       | this and we combine   |
        |                       |                       | it with the current   |
        |                       |                       | platform to determine |
        |                       |                       | the archiver type.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `A                    | ::: block             |
        |                       | rchiverProvider.Type` | Optional type that    |
        |                       |                       | can be specified by   |
        |                       |                       | cxx.archiver_type to  |
        |                       |                       | indicate the given    |
        |                       |                       | archiver is llvm-lib. |
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
        | `sta                  | `f                    | ::: block             |
        | tic ArchiverProvider` | rom​(ToolProvider tool | Creates an            |
        |                       | Provider,     Archive | appropriate           |
        |                       | rProvider.Type type)` | ArchiverProvider      |
        |                       |                       | instance for the      |
        |                       |                       | given parameters.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `from​(Too             | ::: block             |
        | tic ArchiverProvider` | lProvider archiver,   | [Deprecate            |
        |                       |    Platform platform, | d.]{.deprecatedLabel} |
        |                       |      Optional<Archive |                       |
        |                       | rProvider.LegacyArchi | :                     |
        |                       | verType> legacyType)` | :: deprecationComment |
        |                       |                       | Use the non-legacy    |
        |                       |                       | type.                 |
        |                       |                       | :::                   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `fro                  |                       |
        | tic ArchiverProvider` | m​(Archiver archiver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `I                    | `getParseTimeDeps     |                       |
        | terable<BuildTarget>` | ​(TargetConfiguration  |                       |
        |                       | targetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Archiver`            | `                     |                       |
        |                       | resolve​(BuildRuleReso |                       |
        |                       | lver resolver,        |                       |
        |                       |  TargetConfiguration  |                       |
        |                       | targetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Deprecated
        Methods](javascript:show(32);)[ ]{.tabEnd}]{#t6 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#resolve(com.facebook.buck.core.rules.BuildRuleResolver,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### resolve

            ``` methodSignature
            Archiver resolve​(BuildRuleResolver resolver,
                             TargetConfiguration targetConfiguration)
            ```

        []{#getParseTimeDeps(com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getParseTimeDeps

            ``` methodSignature
            Iterable<BuildTarget> getParseTimeDeps​(TargetConfiguration targetConfiguration)
            ```

        []{#from(com.facebook.buck.cxx.toolchain.Archiver)}

        -   #### from

            ``` methodSignature
            static ArchiverProvider from​(Archiver archiver)
            ```

        []{#from(com.facebook.buck.core.toolchain.toolprovider.ToolProvider,com.facebook.buck.util.environment.Platform,java.util.Optional)}

        -   #### from

            ``` methodSignature
            @Deprecated
            static ArchiverProvider from​(ToolProvider archiver,
                                         Platform platform,
                                         Optional<ArchiverProvider.LegacyArchiverType> legacyType)
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}

            ::: deprecationComment
            Use the non-legacy type.
            :::
            :::

            ::: block
            Creates an appropriate ArchiverProvider instance for the
            given parameters.
            :::

        []{#from(com.facebook.buck.core.toolchain.toolprovider.ToolProvider,com.facebook.buck.cxx.toolchain.ArchiverProvider.Type)}

        -   #### from

            ``` methodSignature
            static ArchiverProvider from​(ToolProvider toolProvider,
                                         ArchiverProvider.Type type)
            ```

            ::: block
            Creates an appropriate ArchiverProvider instance for the
            given parameters.
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

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
[Package]{.packageLabelInType} [com.facebook.buck.rules.modern.impl](package-summary.html)
:::

## Class ModernBuildableSupport {#class-modernbuildablesupport .title title="Class ModernBuildableSupport"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.modern.impl.ModernBuildableSupport

::: description
-   

    ------------------------------------------------------------------------

        public class ModernBuildableSupport
        extends Object

    ::: block
    ModernBuildableSupport provides methods to make using, implementing
    and migrating to ModernBuildRules easier.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static Re            | `getDerivedAr         |                       |
        | cordArtifactVerifier` | tifactVerifier​(BuildT |                       |
        |                       | arget buildTarget,    |                       |
        |                       |                       |                       |
        |                       |    ProjectFilesystem  |                       |
        |                       | filesystem,           |                       |
        |                       |                  Adds |                       |
        |                       | ToRuleKey buildable)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Re            | `getDe                | ::: block             |
        | cordArtifactVerifier` | rivedArtifactVerifier | Derives an            |
        |                       | ​(BuildTarget target,  | ArtifactVerifier from |
        |                       |                       | the \@AddToRuleKey    |
        |                       |      ProjectFilesyste | annotated fields.     |
        |                       | m filesystem,         | :::                   |
        |                       |                    Ad |                       |
        |                       | dsToRuleKey buildable |                       |
        |                       | ,                     |                       |
        |                       |        BuildableConte |                       |
        |                       | xt buildableContext)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static BuildCel      | `newCellRe            | ::: block             |
        | lRelativePathFactory` | lativePathFactory​(Pat | Creates a             |
        |                       | h buildCellRootPath,  | BuildCe               |
        |                       |                       | llRelativePathFactory |
        |                       |      ProjectFilesyste | for a build root and  |
        |                       | m projectFilesystem)` | filesystem pair.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `stati                | `                     |                       |
        | c OutputPathResolver` | newOutputPathResolver |                       |
        |                       | ​(BuildTarget buildTar |                       |
        |                       | get,                  |                       |
        |                       |      ProjectFilesyste |                       |
        |                       | m projectFilesystem)` |                       |
        +-----------------------+-----------------------+-----------------------+

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

        []{#newCellRelativePathFactory(java.nio.file.Path,com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### newCellRelativePathFactory

            ``` methodSignature
            public static BuildCellRelativePathFactory newCellRelativePathFactory​(Path buildCellRootPath,
                                                                                  ProjectFilesystem projectFilesystem)
            ```

            ::: block
            Creates a BuildCellRelativePathFactory for a build root and
            filesystem pair.
            :::

        []{#newOutputPathResolver(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### newOutputPathResolver

            ``` methodSignature
            public static OutputPathResolver newOutputPathResolver​(BuildTarget buildTarget,
                                                                   ProjectFilesystem projectFilesystem)
            ```

        []{#getDerivedArtifactVerifier(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rulekey.AddsToRuleKey,com.facebook.buck.core.build.buildable.context.BuildableContext)}

        -   #### getDerivedArtifactVerifier

            ``` methodSignature
            public static RecordArtifactVerifier getDerivedArtifactVerifier​(BuildTarget target,
                                                                            ProjectFilesystem filesystem,
                                                                            AddsToRuleKey buildable,
                                                                            BuildableContext buildableContext)
            ```

            ::: block
            Derives an ArtifactVerifier from the \@AddToRuleKey
            annotated fields.
            :::

        []{#getDerivedArtifactVerifier(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rulekey.AddsToRuleKey)}

        -   #### getDerivedArtifactVerifier

            ``` methodSignature
            public static RecordArtifactVerifier getDerivedArtifactVerifier​(BuildTarget buildTarget,
                                                                            ProjectFilesystem filesystem,
                                                                            AddsToRuleKey buildable)
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

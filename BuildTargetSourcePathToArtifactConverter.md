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
[Package]{.packageLabelInType} [com.facebook.buck.core.artifact](package-summary.html)
:::

## Class BuildTargetSourcePathToArtifactConverter {#class-buildtargetsourcepathtoartifactconverter .title title="Class BuildTargetSourcePathToArtifactConverter"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.artifact.BuildTargetSourcePathToArtifactConverter

::: description
-   

    ------------------------------------------------------------------------

        public class BuildTargetSourcePathToArtifactConverter
        extends Object

    ::: block
    Utility for converting legacy
    [`ExplicitBuildTargetSourcePath`](../sourcepath/ExplicitBuildTargetSourcePath.html "class in com.facebook.buck.core.sourcepath")
    from rules to new
    [`Artifact`](Artifact.html "interface in com.facebook.buck.core.artifact")s.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type        Method                                                                  Description
          ------------------------ ----------------------------------------------------------------------- -------------
          `static BuildArtifact`   `convert​(ProjectFilesystem filesystem,        SourcePath sourcePath)`    

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

        []{#convert(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### convert

            ``` methodSignature
            public static BuildArtifact convert​(ProjectFilesystem filesystem,
                                                SourcePath sourcePath)
            ```

            [Parameters:]{.paramLabel}
            :   `sourcePath` - the
                [`SourcePath`](../sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")
                of the legacy target. This should be a
                [`BuildTargetSourcePath`](../sourcepath/BuildTargetSourcePath.html "interface in com.facebook.buck.core.sourcepath")
                of either
                [`ExplicitBuildTargetSourcePath`](../sourcepath/ExplicitBuildTargetSourcePath.html "class in com.facebook.buck.core.sourcepath")
                or
                [`ForwardingBuildTargetSourcePath`](../sourcepath/ForwardingBuildTargetSourcePath.html "class in com.facebook.buck.core.sourcepath").

            [Returns:]{.returnLabel}
            :   a
                [`BuildArtifact`](BuildArtifact.html "interface in com.facebook.buck.core.artifact")
                that refers to the
                [`SourcePath`](../sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")
                of a legacy
                [`BuildRule`](../rules/BuildRule.html "interface in com.facebook.buck.core.rules").
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

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
[Package]{.packageLabelInType} [com.facebook.buck.core.artifact.converter](package-summary.html)
:::

## Class DefaultInfoArtifactsRetriever {#class-defaultinfoartifactsretriever .title title="Class DefaultInfoArtifactsRetriever"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.artifact.converter.DefaultInfoArtifactsRetriever

::: description
-   

    ------------------------------------------------------------------------

        public class DefaultInfoArtifactsRetriever
        extends Object

    ::: block
    Utility class for getting artifacts from
    [`DefaultInfo`](../../rules/providers/lib/DefaultInfo.html "class in com.facebook.buck.core.rules.providers.lib").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `                     | `getArtifacts​(        | ::: block             |
        | static Set<Artifact>` | DefaultInfo defaultIn | Returns the           |
        |                       | fo,             Build | [`Artifact`](.        |
        |                       | TargetWithOutputs bui | ./Artifact.html "inte |
        |                       | ldTargetWithOutputs)` | rface in com.facebook |
        |                       |                       | .buck.core.artifact") |
        |                       |                       | instances associated  |
        |                       |                       | with the given        |
        |                       |                       | [                     |
        |                       |                       | `BuildTarget`](../../ |
        |                       |                       | model/BuildTarget.htm |
        |                       |                       | l "class in com.faceb |
        |                       |                       | ook.buck.core.model") |
        |                       |                       | and                   |
        |                       |                       | [`                    |
        |                       |                       | OutputLabel`](../../m |
        |                       |                       | odel/OutputLabel.html |
        |                       |                       |  "class in com.facebo |
        |                       |                       | ok.buck.core.model"). |
        |                       |                       | :::                   |
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

        []{#getArtifacts(com.facebook.buck.core.rules.providers.lib.DefaultInfo,com.facebook.buck.core.model.BuildTargetWithOutputs)}

        -   #### getArtifacts

            ``` methodSignature
            public static Set<Artifact> getArtifacts​(DefaultInfo defaultInfo,
                                                     BuildTargetWithOutputs buildTargetWithOutputs)
            ```

            ::: block
            Returns the
            [`Artifact`](../Artifact.html "interface in com.facebook.buck.core.artifact")
            instances associated with the given
            [`BuildTarget`](../../model/BuildTarget.html "class in com.facebook.buck.core.model")
            and
            [`OutputLabel`](../../model/OutputLabel.html "class in com.facebook.buck.core.model").
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

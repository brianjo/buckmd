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
[Package]{.packageLabelInType} [com.facebook.buck.artifact_cache](package-summary.html)
:::

## Class ArtifactUploader {#class-artifactuploader .title title="Class ArtifactUploader"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.artifact_cache.ArtifactUploader

::: description
-   

    ------------------------------------------------------------------------

        public class ArtifactUploader
        extends Object

    ::: block
    ArtifactUploader contains the logic of how to take a list of
    artifact paths and metadata and store that to the ArtifactCache.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor            Description
          ---------------------- -------------
          `ArtifactUploader()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `s                    | `performUploadTo      | ::: block             |
        | tatic com.google.comm | ArtifactCache​(com.goo | As method name says   |
        | on.util.concurrent.Li | gle.common.collect.Im | :::                   |
        | stenableFuture<Unit>` | mutableSet<RuleKey> r |                       |
        |                       | uleKeys,              |                       |
        |                       |                 Artif |                       |
        |                       | actCache artifactCach |                       |
        |                       | e,                    |                       |
        |                       |           BuckEventBu |                       |
        |                       | s eventBus,           |                       |
        |                       |                    co |                       |
        |                       | m.google.common.colle |                       |
        |                       | ct.ImmutableMap<Strin |                       |
        |                       | g,​String> buildMetada |                       |
        |                       | ta,                   |                       |
        |                       |            SortedSet< |                       |
        |                       | Path> pathsToIncludeI |                       |
        |                       | nArchive,             |                       |
        |                       |                  Buil |                       |
        |                       | dRule buildRule,      |                       |
        |                       |                       |                       |
        |                       |    long buildTimeMs)` |                       |
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### ArtifactUploader

                public ArtifactUploader()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#performUploadToArtifactCache(com.google.common.collect.ImmutableSet,com.facebook.buck.artifact_cache.ArtifactCache,com.facebook.buck.event.BuckEventBus,com.google.common.collect.ImmutableMap,java.util.SortedSet,com.facebook.buck.core.rules.BuildRule,long)}

        -   #### performUploadToArtifactCache

            ``` methodSignature
            public static com.google.common.util.concurrent.ListenableFuture<Unit> performUploadToArtifactCache​(com.google.common.collect.ImmutableSet<RuleKey> ruleKeys,
                                                                                                                ArtifactCache artifactCache,
                                                                                                                BuckEventBus eventBus,
                                                                                                                com.google.common.collect.ImmutableMap<String,​String> buildMetadata,
                                                                                                                SortedSet<Path> pathsToIncludeInArchive,
                                                                                                                BuildRule buildRule,
                                                                                                                long buildTimeMs)
            ```

            ::: block
            As method name says
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

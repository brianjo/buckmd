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

## Class AbstractArtifactCacheEventFactory {#class-abstractartifactcacheeventfactory .title title="Class AbstractArtifactCacheEventFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.artifact_cache.AbstractArtifactCacheEventFactory

::: description
-   

    All Implemented Interfaces:
    :   `ArtifactCacheEventFactory`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `DirArtifactCacheEvent.DirArtifactCacheEventFactory`,
        `SQLiteArtifactCacheEvent.SQLiteArtifactCacheEventFactory`

    ------------------------------------------------------------------------

        public abstract class AbstractArtifactCacheEventFactory
        extends Object
        implements ArtifactCacheEventFactory
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                                                                                                                                                                                                                     Description
          -------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `protected `   `AbstractArtifactCacheEventFactory​(java.util.function.Function<String,​UnconfiguredBuildTarget> unconfiguredBuildTargetFactory,                                  TargetConfigurationSerializer targetConfigurationSerializer)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                   Method                                                                                                                                                                                                                                                   Description
          ----------------------------------- -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `protected Optional<BuildTarget>`   `getTarget​(com.google.common.collect.ImmutableMap<String,​String> metadata)`                                                                                                                                                                               
          `static Optional<BuildTarget>`      `getTarget​(java.util.function.Function<String,​UnconfiguredBuildTarget> unconfiguredBuildTargetFactory,          TargetConfigurationSerializer targetConfigurationSerializer,          com.google.common.collect.ImmutableMap<String,​String> metadata)`    
          `static Optional<BuildTarget>`      `getTarget​(java.util.function.Function<String,​UnconfiguredBuildTarget> unconfiguredBuildTargetFactory,          String target,          TargetConfiguration targetConfiguration)`                                                                         

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.artifact_cache.ArtifactCacheEventFactory}

            ### Methods inherited from interface com.facebook.buck.artifact_cache.[ArtifactCacheEventFactory](ArtifactCacheEventFactory.html "interface in com.facebook.buck.artifact_cache")

            `newContainsFinishedEvent, newContainsStartedEvent, newFetchFinishedEvent, newFetchStartedEvent, newStoreFinishedEvent, newStoreStartedEvent`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.util.function.Function,com.facebook.buck.core.model.TargetConfigurationSerializer)}

        -   #### AbstractArtifactCacheEventFactory

                protected AbstractArtifactCacheEventFactory​(java.util.function.Function<String,​UnconfiguredBuildTarget> unconfiguredBuildTargetFactory,
                                                            TargetConfigurationSerializer targetConfigurationSerializer)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getTarget(com.google.common.collect.ImmutableMap)}

        -   #### getTarget

            ``` methodSignature
            protected final Optional<BuildTarget> getTarget​(com.google.common.collect.ImmutableMap<String,​String> metadata)
            ```

        []{#getTarget(java.util.function.Function,com.facebook.buck.core.model.TargetConfigurationSerializer,com.google.common.collect.ImmutableMap)}

        -   #### getTarget

            ``` methodSignature
            public static Optional<BuildTarget> getTarget​(java.util.function.Function<String,​UnconfiguredBuildTarget> unconfiguredBuildTargetFactory,
                                                          TargetConfigurationSerializer targetConfigurationSerializer,
                                                          com.google.common.collect.ImmutableMap<String,​String> metadata)
            ```

        []{#getTarget(java.util.function.Function,java.lang.String,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getTarget

            ``` methodSignature
            public static Optional<BuildTarget> getTarget​(java.util.function.Function<String,​UnconfiguredBuildTarget> unconfiguredBuildTargetFactory,
                                                          @Nullable
                                                          String target,
                                                          TargetConfiguration targetConfiguration)
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

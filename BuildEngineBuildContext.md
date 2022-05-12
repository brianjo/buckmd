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
[Package]{.packageLabelInType} [com.facebook.buck.core.build.engine](package-summary.html)
:::

## Class BuildEngineBuildContext {#class-buildenginebuildcontext .title title="Class BuildEngineBuildContext"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.build.engine.BuildEngineBuildContext

::: description
-   

    ------------------------------------------------------------------------

        public abstract class BuildEngineBuildContext
        extends Object

    ::: block
    Per-build context used by
    [`BuildEngine`](BuildEngine.html "interface in com.facebook.buck.core.build.engine").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                   Description
          ----------------------------- -------------
          `BuildEngineBuildContext()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `BuildInfoRecorder`   | `createBui            | ::: block             |
        |                       | ldInfoRecorder​(BuildT | Creates an            |
        |                       | arget buildTarget,    | [`BuildI              |
        |                       |                       | nfoRecorder`](buildin |
        |                       | ProjectFilesystem fil | fo/BuildInfoRecorder. |
        |                       | esystem,              | html "class in com.fa |
        |                       |            BuildInfoS | cebook.buck.core.buil |
        |                       | tore buildInfoStore)` | d.engine.buildinfo"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OnDiskBuildInfo`     | `createO              | ::: block             |
        |                       | nDiskBuildInfoFor​(Bui | Creates an            |
        |                       | ldTarget target,      | [`OnDisk              |
        |                       |                     P | BuildInfo`](buildinfo |
        |                       | rojectFilesystem file | /OnDiskBuildInfo.html |
        |                       | system,               |  "interface in com.fa |
        |                       |            BuildInfoS | cebook.buck.core.buil |
        |                       | tore buildInfoStore)` | d.engine.buildinfo"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ab                   | `getArtifactCache()`  |                       |
        | stract ArtifactCache` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `a                    | `getBuildContext()`   | ::: block             |
        | bstract BuildContext` |                       | `BuildContext` used   |
        |                       |                       | by various rules to   |
        |                       |                       | generate              |
        |                       |                       | [`Step`](.            |
        |                       |                       | ./../../step/Step.htm |
        |                       |                       | l "interface in com.f |
        |                       |                       | acebook.buck.step")s. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract BuildId`    | `getBuildId()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Clock`      | `getClock()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getEnvironment()`    |                       |
        | abstract com.google.c |                       |                       |
        | ommon.collect.Immutab |                       |                       |
        | leMap<String,​String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuckEventBus`        | `getEventBus()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isKeepGoing()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Bui           | `of​(BuildConte        |                       |
        | ldEngineBuildContext` | xt buildContext,   Ar |                       |
        |                       | tifactCache artifactC |                       |
        |                       | ache,   Clock clock,  |                       |
        |                       |   BuildId buildId,    |                       |
        |                       | Map<String,​? extends  |                       |
        |                       | String> environment,  |                       |
        |                       |   boolean keepGoing)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Bui                  | `withA                |                       |
        | ldEngineBuildContext` | rtifactCache​(Artifact |                       |
        |                       | Cache artifactCache)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Bui                  | `wi                   |                       |
        | ldEngineBuildContext` | thBuildContext​(BuildC |                       |
        |                       | ontext buildContext)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Bui                  | `withBuil             |                       |
        | ldEngineBuildContext` | dId​(BuildId buildId)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Bui                  | `withKeepGoin         |                       |
        | ldEngineBuildContext` | g​(boolean keepGoing)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
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

        -   #### BuildEngineBuildContext

                public BuildEngineBuildContext()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBuildContext()}

        -   #### getBuildContext

            ``` methodSignature
            public abstract BuildContext getBuildContext()
            ```

            ::: block
            `BuildContext` used by various rules to generate
            [`Step`](../../../step/Step.html "interface in com.facebook.buck.step")s.
            :::

        []{#getArtifactCache()}

        -   #### getArtifactCache

            ``` methodSignature
            public abstract ArtifactCache getArtifactCache()
            ```

        []{#getClock()}

        -   #### getClock

            ``` methodSignature
            public abstract Clock getClock()
            ```

        []{#getBuildId()}

        -   #### getBuildId

            ``` methodSignature
            public abstract BuildId getBuildId()
            ```

        []{#getEnvironment()}

        -   #### getEnvironment

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableMap<String,​String> getEnvironment()
            ```

        []{#isKeepGoing()}

        -   #### isKeepGoing

            ``` methodSignature
            @Default
            public boolean isKeepGoing()
            ```

        []{#createOnDiskBuildInfoFor(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.build.engine.buildinfo.BuildInfoStore)}

        -   #### createOnDiskBuildInfoFor

            ``` methodSignature
            public OnDiskBuildInfo createOnDiskBuildInfoFor​(BuildTarget target,
                                                            ProjectFilesystem filesystem,
                                                            BuildInfoStore buildInfoStore)
            ```

            ::: block
            Creates an
            [`OnDiskBuildInfo`](buildinfo/OnDiskBuildInfo.html "interface in com.facebook.buck.core.build.engine.buildinfo").
            This method should be visible to
            [`AbstractBuildRule`](../../rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl"),
            but not
            [`BuildRule`](../../rules/BuildRule.html "interface in com.facebook.buck.core.rules")s
            in general.
            :::

        []{#createBuildInfoRecorder(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.build.engine.buildinfo.BuildInfoStore)}

        -   #### createBuildInfoRecorder

            ``` methodSignature
            public BuildInfoRecorder createBuildInfoRecorder​(BuildTarget buildTarget,
                                                             ProjectFilesystem filesystem,
                                                             BuildInfoStore buildInfoStore)
            ```

            ::: block
            Creates an
            [`BuildInfoRecorder`](buildinfo/BuildInfoRecorder.html "class in com.facebook.buck.core.build.engine.buildinfo").
            This method should be visible to
            [`AbstractBuildRule`](../../rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl"),
            but not
            [`BuildRule`](../../rules/BuildRule.html "interface in com.facebook.buck.core.rules")s
            in general.
            :::

        []{#getEventBus()}

        -   #### getEventBus

            ``` methodSignature
            public final BuckEventBus getEventBus()
            ```

        []{#of(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.artifact_cache.ArtifactCache,com.facebook.buck.util.timing.Clock,com.facebook.buck.core.model.BuildId,java.util.Map,boolean)}

        -   #### of

            ``` methodSignature
            public static BuildEngineBuildContext of​(BuildContext buildContext,
                                                     ArtifactCache artifactCache,
                                                     Clock clock,
                                                     BuildId buildId,
                                                     Map<String,​? extends String> environment,
                                                     boolean keepGoing)
            ```

        []{#withBuildContext(com.facebook.buck.core.build.context.BuildContext)}

        -   #### withBuildContext

            ``` methodSignature
            public BuildEngineBuildContext withBuildContext​(BuildContext buildContext)
            ```

        []{#withArtifactCache(com.facebook.buck.artifact_cache.ArtifactCache)}

        -   #### withArtifactCache

            ``` methodSignature
            public BuildEngineBuildContext withArtifactCache​(ArtifactCache artifactCache)
            ```

        []{#withKeepGoing(boolean)}

        -   #### withKeepGoing

            ``` methodSignature
            public BuildEngineBuildContext withKeepGoing​(boolean keepGoing)
            ```

        []{#withBuildId(com.facebook.buck.core.model.BuildId)}

        -   #### withBuildId

            ``` methodSignature
            public BuildEngineBuildContext withBuildId​(BuildId buildId)
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

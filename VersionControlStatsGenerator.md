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
[Package]{.packageLabelInType} [com.facebook.buck.util.versioncontrol](package-summary.html)
:::

## Class VersionControlStatsGenerator {#class-versioncontrolstatsgenerator .title title="Class VersionControlStatsGenerator"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.versioncontrol.VersionControlStatsGenerator

::: description
-   

    ------------------------------------------------------------------------

        public class VersionControlStatsGenerator
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `VersionContro        | ::: block             |
        |                       | lStatsGenerator.Mode` | Modes the generator   |
        |                       |                       | can get stats in, in  |
        |                       |                       | order from least      |
        |                       |                       | comprehensive to most |
        |                       |                       | comprehensive.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                          Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `VersionControlStatsGenerator​(VersionControlCmdLineInterface versionControlCmdLineInterface,                             Optional<com.facebook.buck.util.versioncontrol.FastVersionControlStats> pregeneratedVersionControlStats)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Optional<Full        | `generateStat         |                       |
        | VersionControlStats>` | s​(VersionControlStats |                       |
        |                       | Generator.Mode mode)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `co                   | `gener                | ::: block             |
        | m.google.common.util. | ateStatsAsync​(boolean | Generate              |
        | concurrent.Listenable |  shouldUploadBuildRep | [`Full                |
        | Future<Optional<FullV | ort,                  | VersionControlStats`] |
        | ersionControlStats>>` |   boolean shouldPreGe | (FullVersionControlSt |
        |                       | nerate,               | ats.html "interface i |
        |                       |      BuckEventBus buc | n com.facebook.buck.u |
        |                       | kEventBus,            | til.versioncontrol"). |
        |                       |         com.google.co | :::                   |
        |                       | mmon.util.concurrent. |                       |
        |                       | ListeningExecutorServ |                       |
        |                       | ice executorService)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
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

        []{#<init>(com.facebook.buck.util.versioncontrol.VersionControlCmdLineInterface,java.util.Optional)}

        -   #### VersionControlStatsGenerator

                public VersionControlStatsGenerator​(VersionControlCmdLineInterface versionControlCmdLineInterface,
                                                    Optional<com.facebook.buck.util.versioncontrol.FastVersionControlStats> pregeneratedVersionControlStats)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#generateStatsAsync(boolean,boolean,com.facebook.buck.event.BuckEventBus,com.google.common.util.concurrent.ListeningExecutorService)}

        -   #### generateStatsAsync

            ``` methodSignature
            public com.google.common.util.concurrent.ListenableFuture<Optional<FullVersionControlStats>> generateStatsAsync​(boolean shouldUploadBuildReport,
                                                                                                                            boolean shouldPreGenerate,
                                                                                                                            BuckEventBus buckEventBus,
                                                                                                                            com.google.common.util.concurrent.ListeningExecutorService executorService)
            ```

            ::: block
            Generate
            [`FullVersionControlStats`](FullVersionControlStats.html "interface in com.facebook.buck.util.versioncontrol").
            The parameters define which mode is generated
            :::

            [Parameters:]{.paramLabel}
            :   `shouldUploadBuildReport` - if this buck build will
                upload a full build report then we generate
                [`FullVersionControlStats`](FullVersionControlStats.html "interface in com.facebook.buck.util.versioncontrol"),
                otherwise just generate `SlowVersionControlStats`.
            :   `shouldPreGenerate` - if true, return a
                `FastVersionControlStats` regardless of
                `      shouldUploadBuildReport`\'s value
            :   `buckEventBus` - the eventBus to which post the
                [`VersionControlStatsEvent`](VersionControlStatsEvent.html "class in com.facebook.buck.util.versioncontrol")
            :   `executorService` - to which this future is attached to.
                Preferably a diskIO executor Service.

        []{#generateStats(com.facebook.buck.util.versioncontrol.VersionControlStatsGenerator.Mode)}

        -   #### generateStats

            ``` methodSignature
            public Optional<FullVersionControlStats> generateStats​(VersionControlStatsGenerator.Mode mode)
                                                            throws InterruptedException
            ```

            [Throws:]{.throwsLabel}
            :   `InterruptedException`
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

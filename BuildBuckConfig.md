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
[Package]{.packageLabelInType} [com.facebook.buck.command.config](package-summary.html)
:::

## Class BuildBuckConfig {#class-buildbuckconfig .title title="Class BuildBuckConfig"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.command.config.BuildBuckConfig

::: description
-   

    All Implemented Interfaces:
    :   `ConfigView<BuckConfig>`

    ------------------------------------------------------------------------

        public abstract class BuildBuckConfig
        extends Object
        implements ConfigView<BuckConfig>

    ::: block
    Some configuration options that may affect the build in some way.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor           Description
          --------------------- -------------
          `BuildBuckConfig()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `boolean`             | `createBuildOut       | ::: block             |
        |                       | putSymLinksEnabled()` | Whether to create     |
        |                       |                       | symlinks of build     |
        |                       |                       | output in             |
        |                       |                       | buck-out/last.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `ge                   |                       |
        |                       | tBuckOutCompatLink()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `long`                | `getBuildInputRu      |                       |
        |                       | leKeyFileSizeLimit()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<com.goo     | `                     |                       |
        | gle.common.collect.Im | getBuildPrehookScript |                       |
        | mutableList<String>>` | InterpreterAndArgs()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getBuildVersions()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getDefaultMaxi       |                       |
        |                       | mumNumberOfThreads()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract BuckConfig` | `getDelegate()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `FileHashCacheMode`   | `ge                   |                       |
        |                       | tFileHashCacheMode()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `H                    | `getHas               |                       |
        | ashedBuckOutLinkMode` | hedBuckOutLinkMode()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getKeySeed()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getMaxActio          |                       |
        |                       | nGraphCacheEntries()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getNumThreads()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getNumThrea          |                       |
        |                       | ds​(int defaultValue)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getNumThrea          |                       |
        |                       | dsForSchedulerPool()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getPathTo            |                       |
        |                       | BuildPrehookScript()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getRuleKeyCaching()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getShoul             | ::: block             |
        |                       | dDeleteTemporaries()` | Whether to delete     |
        |                       |                       | temporary files       |
        |                       |                       | generated to run a    |
        |                       |                       | build rule            |
        |                       |                       | immediately after the |
        |                       |                       | rule is run.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `                     |                       |
        |                       | getTargetsVersions()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isEmbedded           |                       |
        |                       | CellBuckOutEnabled()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `of​(                  |                       |
        | atic BuildBuckConfig` | BuckConfig delegate)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `shouldBuckOutInclu   |                       |
        |                       | deTargetConfigHash()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `useBuckBinaryHash()` | ::: block             |
        |                       |                       | Whether Buck should   |
        |                       |                       | use Buck binary hash  |
        |                       |                       | or git commit id as   |
        |                       |                       | the core key in all   |
        |                       |                       | rule keys.            |
        |                       |                       | :::                   |
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

        -   #### BuildBuckConfig

                public BuildBuckConfig()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getDelegate()}

        -   #### getDelegate

            ``` methodSignature
            public abstract BuckConfig getDelegate()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDelegate` in interface `ConfigView<BuckConfig>`

        []{#of(com.facebook.buck.core.config.BuckConfig)}

        -   #### of

            ``` methodSignature
            public static BuildBuckConfig of​(BuckConfig delegate)
            ```

        []{#getMaxActionGraphCacheEntries()}

        -   #### getMaxActionGraphCacheEntries

            ``` methodSignature
            @Lazy
            public int getMaxActionGraphCacheEntries()
            ```

        []{#useBuckBinaryHash()}

        -   #### useBuckBinaryHash

            ``` methodSignature
            @Lazy
            public boolean useBuckBinaryHash()
            ```

            ::: block
            Whether Buck should use Buck binary hash or git commit id as
            the core key in all rule keys.
            The binary hash reflects the code that can affect the
            content of artifacts.

            By default git commit id is used as the core key.
            :::

            [Returns:]{.returnLabel}
            :   `True` if binary hash should be used as the core key

        []{#getKeySeed()}

        -   #### getKeySeed

            ``` methodSignature
            @Lazy
            public int getKeySeed()
            ```

        []{#getNumThreads()}

        -   #### getNumThreads

            ``` methodSignature
            @Lazy
            public int getNumThreads()
            ```

            [Returns:]{.returnLabel}
            :   the number of threads Buck should use.

        []{#getNumThreadsForSchedulerPool()}

        -   #### getNumThreadsForSchedulerPool

            ``` methodSignature
            @Lazy
            public int getNumThreadsForSchedulerPool()
            ```

            [Returns:]{.returnLabel}
            :   the number of threads to be used for the scheduled
                executor thread pool.

        []{#getBuildInputRuleKeyFileSizeLimit()}

        -   #### getBuildInputRuleKeyFileSizeLimit

            ``` methodSignature
            @Lazy
            public long getBuildInputRuleKeyFileSizeLimit()
            ```

            [Returns:]{.returnLabel}
            :   the maximum size of files input based rule keys will be
                willing to hash.

        []{#getDefaultMaximumNumberOfThreads()}

        -   #### getDefaultMaximumNumberOfThreads

            ``` methodSignature
            @Lazy
            public int getDefaultMaximumNumberOfThreads()
            ```

        []{#getNumThreads(int)}

        -   #### getNumThreads

            ``` methodSignature
            public int getNumThreads​(int defaultValue)
            ```

            [Returns:]{.returnLabel}
            :   the number of threads Buck should use or the specified
                defaultValue if it is not set.

        []{#getBuckOutCompatLink()}

        -   #### getBuckOutCompatLink

            ``` methodSignature
            @Lazy
            public boolean getBuckOutCompatLink()
            ```

            [Returns:]{.returnLabel}
            :   whether to symlink the default output location
                (\`buck-out\`) to the user-provided override for
                compatibility.

        []{#getBuildVersions()}

        -   #### getBuildVersions

            ``` methodSignature
            @Lazy
            public boolean getBuildVersions()
            ```

            [Returns:]{.returnLabel}
            :   whether to enabled versions on build/test command.

        []{#getTargetsVersions()}

        -   #### getTargetsVersions

            ``` methodSignature
            @Lazy
            public boolean getTargetsVersions()
            ```

            [Returns:]{.returnLabel}
            :   whether to enabled versions on targets command.

        []{#getRuleKeyCaching()}

        -   #### getRuleKeyCaching

            ``` methodSignature
            @Lazy
            public boolean getRuleKeyCaching()
            ```

            [Returns:]{.returnLabel}
            :   whether to enable caching of rule key calculations
                between builds.

        []{#createBuildOutputSymLinksEnabled()}

        -   #### createBuildOutputSymLinksEnabled

            ``` methodSignature
            @Lazy
            public boolean createBuildOutputSymLinksEnabled()
            ```

            ::: block
            Whether to create symlinks of build output in buck-out/last.
            :::

        []{#isEmbeddedCellBuckOutEnabled()}

        -   #### isEmbeddedCellBuckOutEnabled

            ``` methodSignature
            @Lazy
            public boolean isEmbeddedCellBuckOutEnabled()
            ```

        []{#getPathToBuildPrehookScript()}

        -   #### getPathToBuildPrehookScript

            ``` methodSignature
            @Lazy
            public Optional<String> getPathToBuildPrehookScript()
            ```

        []{#getBuildPrehookScriptInterpreterAndArgs()}

        -   #### getBuildPrehookScriptInterpreterAndArgs

            ``` methodSignature
            @Lazy
            public Optional<com.google.common.collect.ImmutableList<String>> getBuildPrehookScriptInterpreterAndArgs()
            ```

        []{#getShouldDeleteTemporaries()}

        -   #### getShouldDeleteTemporaries

            ``` methodSignature
            @Lazy
            public boolean getShouldDeleteTemporaries()
            ```

            ::: block
            Whether to delete temporary files generated to run a build
            rule immediately after the rule is run.
            :::

        []{#getFileHashCacheMode()}

        -   #### getFileHashCacheMode

            ``` methodSignature
            @Lazy
            public FileHashCacheMode getFileHashCacheMode()
            ```

            [Returns:]{.returnLabel}
            :   whether to enable new file hash cache engine.

        []{#shouldBuckOutIncludeTargetConfigHash()}

        -   #### shouldBuckOutIncludeTargetConfigHash

            ``` methodSignature
            @Lazy
            public boolean shouldBuckOutIncludeTargetConfigHash()
            ```

        []{#getHashedBuckOutLinkMode()}

        -   #### getHashedBuckOutLinkMode

            ``` methodSignature
            @Lazy
            public HashedBuckOutLinkMode getHashedBuckOutLinkMode()
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

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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.parser](package-summary.html)
:::

## Class DaemonicParserState {#class-daemonicparserstate .title title="Class DaemonicParserState"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.parser.DaemonicParserState

::: description
-   

    ------------------------------------------------------------------------

        @ThreadSafe
        public class DaemonicParserState
        extends Object

    ::: block
    Persistent parsing data, that can exist between invocations of the
    [`Parser`](Parser.html "interface in com.facebook.buck.parser"). All
    public methods that cause build files to be read must be guarded by
    calls to
    [`invalidateIfProjectBuildFileParserStateChanged(Cell)`](#invalidateIfProjectBuildFileParserStateChanged(com.facebook.buck.core.cell.Cell))
    in order to ensure that state is maintained correctly.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                                                                                                 Field                          Description
          ----------------------------------------------------------------------------------------------------------------- ------------------------------ -------------
          `static com.facebook.buck.parser.DaemonicParserState.CacheType<UnconfiguredBuildTarget,​UnconfiguredTargetNode>`   `RAW_TARGET_NODE_CACHE_TYPE`    
          `static com.facebook.buck.parser.DaemonicParserState.CacheType<BuildTarget,​TargetNodeMaybeIncompatible>`          `TARGET_NODE_CACHE_TYPE`        

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                 Description
          ------------------------------------------- -------------
          `DaemonicParserState​(int parsingThreads)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.goo              | `getCounters()`       |                       |
        | gle.common.collect.Im |                       |                       |
        | mutableList<Counter>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `<K,​T>com.facebook    | `getOrCre             | ::: block             |
        | .buck.parser.Pipeline | ateNodeCache​(com.face | Retrieve the cache    |
        | NodeCache.Cache<K,​T>` | book.buck.parser.Daem | view for caching a    |
        |                       | onicParserState.Cache | particular type.      |
        |                       | Type<K,​T> cacheType)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.facebook.bu      | `g                    |                       |
        | ck.parser.PipelineNod | etPackageFileCache()` |                       |
        | eCache.Cache<AbsPath, |                       |                       |
        | ​PackageFileManifest>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.facebook.        | `getRawNodeCache()`   |                       |
        | buck.parser.PipelineN |                       |                       |
        | odeCache.Cache<AbsPat |                       |                       |
        | h,​BuildFileManifest>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `i                    |                       |
        |                       | nvalidateAllCaches()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `inval                |                       |
        |                       | idateBasedOn​(Watchman |                       |
        |                       | OverflowEvent event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `i                    |                       |
        |                       | nvalidateBasedOn​(Watc |                       |
        |                       | hmanPathEvent event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `invalidateC          |                       |
        |                       | ellCaches​(Cell cell)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `invalida             | ::: block             |
        |                       | tePath​(AbsPath path)` | Invalidate everything |
        |                       |                       | which depend on path. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `isPathCre            |                       |
        |                       | ateOrDeleteEvent​(Watc |                       |
        |                       | hmanPathEvent event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#TARGET_NODE_CACHE_TYPE}

        -   #### TARGET_NODE_CACHE_TYPE

                public static final com.facebook.buck.parser.DaemonicParserState.CacheType<BuildTarget,​TargetNodeMaybeIncompatible> TARGET_NODE_CACHE_TYPE

        []{#RAW_TARGET_NODE_CACHE_TYPE}

        -   #### RAW_TARGET_NODE_CACHE_TYPE

                public static final com.facebook.buck.parser.DaemonicParserState.CacheType<UnconfiguredBuildTarget,​UnconfiguredTargetNode> RAW_TARGET_NODE_CACHE_TYPE
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(int)}

        -   #### DaemonicParserState

                public DaemonicParserState​(int parsingThreads)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getOrCreateNodeCache(com.facebook.buck.parser.DaemonicParserState.CacheType)}

        -   #### getOrCreateNodeCache

            ``` methodSignature
            public <K,​T> com.facebook.buck.parser.PipelineNodeCache.Cache<K,​T> getOrCreateNodeCache​(com.facebook.buck.parser.DaemonicParserState.CacheType<K,​T> cacheType)
            ```

            ::: block
            Retrieve the cache view for caching a particular type.
            Note that the output type is not constrained to the type of
            the Class object to allow for types with generics. Care
            should be taken to ensure that the correct class object is
            passed in.
            :::

        []{#getRawNodeCache()}

        -   #### getRawNodeCache

            ``` methodSignature
            public com.facebook.buck.parser.PipelineNodeCache.Cache<AbsPath,​BuildFileManifest> getRawNodeCache()
            ```

        []{#getPackageFileCache()}

        -   #### getPackageFileCache

            ``` methodSignature
            public com.facebook.buck.parser.PipelineNodeCache.Cache<AbsPath,​PackageFileManifest> getPackageFileCache()
            ```

        []{#invalidateBasedOn(com.facebook.buck.io.watchman.WatchmanOverflowEvent)}

        -   #### invalidateBasedOn

            ``` methodSignature
            public void invalidateBasedOn​(WatchmanOverflowEvent event)
            ```

        []{#invalidateBasedOn(com.facebook.buck.io.watchman.WatchmanPathEvent)}

        -   #### invalidateBasedOn

            ``` methodSignature
            public void invalidateBasedOn​(WatchmanPathEvent event)
            ```

        []{#invalidatePath(com.facebook.buck.core.filesystems.AbsPath)}

        -   #### invalidatePath

            ``` methodSignature
            public void invalidatePath​(AbsPath path)
            ```

            ::: block
            Invalidate everything which depend on path.
            :::

        []{#isPathCreateOrDeleteEvent(com.facebook.buck.io.watchman.WatchmanPathEvent)}

        -   #### isPathCreateOrDeleteEvent

            ``` methodSignature
            public static boolean isPathCreateOrDeleteEvent​(WatchmanPathEvent event)
            ```

        []{#invalidateCellCaches(com.facebook.buck.core.cell.Cell)}

        -   #### invalidateCellCaches

            ``` methodSignature
            public boolean invalidateCellCaches​(Cell cell)
            ```

        []{#invalidateAllCaches()}

        -   #### invalidateAllCaches

            ``` methodSignature
            public boolean invalidateAllCaches()
            ```

        []{#getCounters()}

        -   #### getCounters

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Counter> getCounters()
            ```

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`
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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

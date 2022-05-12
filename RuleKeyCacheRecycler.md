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
[Package]{.packageLabelInType} [com.facebook.buck.rules.keys](package-summary.html)
:::

## Class RuleKeyCacheRecycler\<V\> {#class-rulekeycacherecyclerv .title title="Class RuleKeyCacheRecycler"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.keys.RuleKeyCacheRecycler\<V\>

::: description
-   

    ------------------------------------------------------------------------

        public class RuleKeyCacheRecycler<V>
        extends Object

    ::: block
    Class which encapsulates all effort to cache and reuse a
    [`RuleKeyCache`](RuleKeyCache.html "interface in com.facebook.buck.rules.keys")
    between builds.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `Ru                   | ::: block             |
        |                       | leKeyCacheRecycler.Se | Any external settings |
        |                       | ttingsAffectingCache` | which, if changed,    |
        |                       |                       | will cause the entire |
        |                       |                       | cache to be           |
        |                       |                       | invalidated.          |
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
        | `static <V> Rul       | `crea                 |                       |
        | eKeyCacheRecycler<V>` | te​(TrackableRuleKeyCa |                       |
        |                       | che<V> ruleKeyCache)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static <V> Rul       | `creat                |                       |
        | eKeyCacheRecycler<V>` | eAndRegister​(com.goog |                       |
        |                       | le.common.eventbus.Ev |                       |
        |                       | entBus eventBus,      |                       |
        |                       |              Trackabl |                       |
        |                       | eRuleKeyCache<V> rule |                       |
        |                       | KeyCache,             |                       |
        |                       |       com.google.comm |                       |
        |                       | on.collect.ImmutableS |                       |
        |                       | et<ProjectFilesystem> |                       |
        |                       |  watchedFilesystems)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `c                    | `g                    |                       |
        | om.google.common.coll | etCachedBuildRules()` |                       |
        | ect.ImmutableList<Map |                       |                       |
        | .Entry<BuildRule,​V>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `invalid              |                       |
        |                       | atePath​(ProjectFilesy |                       |
        |                       | stem filesystem,      |                       |
        |                       |           Path path)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `onFile               |                       |
        |                       | systemChange​(Watchman |                       |
        |                       | OverflowEvent event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `on                   |                       |
        |                       | FilesystemChange​(Watc |                       |
        |                       | hmanPathEvent event)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `withRecycledCache​(   | ::: block             |
        | RuleKeyCacheScope<V>` | BuckEventBus buckEven | Provides access to a  |
        |                       | tBus,                 | [`RuleKeyCache`]      |
        |                       |   RuleKeyCacheRecycle | (RuleKeyCache.html "i |
        |                       | r.SettingsAffectingCa | nterface in com.faceb |
        |                       | che currentSettings)` | ook.buck.rules.keys") |
        |                       |                       | via a                 |
        |                       |                       | [`Rule                |
        |                       |                       | KeyCacheScope`](RuleK |
        |                       |                       | eyCacheScope.html "in |
        |                       |                       | terface in com.facebo |
        |                       |                       | ok.buck.rules.keys"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
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
    -   []{#method.detail}

        ### Method Detail

        []{#createAndRegister(com.google.common.eventbus.EventBus,com.facebook.buck.rules.keys.TrackableRuleKeyCache,com.google.common.collect.ImmutableSet)}

        -   #### createAndRegister

            ``` methodSignature
            public static <V> RuleKeyCacheRecycler<V> createAndRegister​(com.google.common.eventbus.EventBus eventBus,
                                                                        TrackableRuleKeyCache<V> ruleKeyCache,
                                                                        com.google.common.collect.ImmutableSet<ProjectFilesystem> watchedFilesystems)
            ```

            [Parameters:]{.paramLabel}
            :   `eventBus` - `EventBus` which delivers watchman events.
            :   `watchedFilesystems` - all
                [`ProjectFilesystem`](../../io/filesystem/ProjectFilesystem.html "interface in com.facebook.buck.io.filesystem")s
                which use watchman to receive events when files are
                changed.

            [Returns:]{.returnLabel}
            :   a new
                [`RuleKeyCacheRecycler`](RuleKeyCacheRecycler.html "class in com.facebook.buck.rules.keys").

        []{#create(com.facebook.buck.rules.keys.TrackableRuleKeyCache)}

        -   #### create

            ``` methodSignature
            public static <V> RuleKeyCacheRecycler<V> create​(TrackableRuleKeyCache<V> ruleKeyCache)
            ```

        []{#onFilesystemChange(com.facebook.buck.io.watchman.WatchmanPathEvent)}

        -   #### onFilesystemChange

            ``` methodSignature
            public void onFilesystemChange​(WatchmanPathEvent event)
            ```

        []{#invalidatePath(com.facebook.buck.io.filesystem.ProjectFilesystem,java.nio.file.Path)}

        -   #### invalidatePath

            ``` methodSignature
            public void invalidatePath​(ProjectFilesystem filesystem,
                                       Path path)
            ```

        []{#onFilesystemChange(com.facebook.buck.io.watchman.WatchmanOverflowEvent)}

        -   #### onFilesystemChange

            ``` methodSignature
            public void onFilesystemChange​(WatchmanOverflowEvent event)
            ```

        []{#withRecycledCache(com.facebook.buck.event.BuckEventBus,com.facebook.buck.rules.keys.RuleKeyCacheRecycler.SettingsAffectingCache)}

        -   #### withRecycledCache

            ``` methodSignature
            public RuleKeyCacheScope<V> withRecycledCache​(BuckEventBus buckEventBus,
                                                          RuleKeyCacheRecycler.SettingsAffectingCache currentSettings)
            ```

            ::: block
            Provides access to a
            [`RuleKeyCache`](RuleKeyCache.html "interface in com.facebook.buck.rules.keys")
            via a
            [`RuleKeyCacheScope`](RuleKeyCacheScope.html "interface in com.facebook.buck.rules.keys").
            The
            [`RuleKeyCacheScope`](RuleKeyCacheScope.html "interface in com.facebook.buck.rules.keys")
            must be used with a try-resource block and does logging and
            cache invalidation both before and after being used.
            :::

            [Returns:]{.returnLabel}
            :   a
                [`RuleKeyCacheScope`](RuleKeyCacheScope.html "interface in com.facebook.buck.rules.keys")
                managing access to enclosed
                [`RuleKeyCache`](RuleKeyCache.html "interface in com.facebook.buck.rules.keys").

        []{#getCachedBuildRules()}

        -   #### getCachedBuildRules

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Map.Entry<BuildRule,​V>> getCachedBuildRules()
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

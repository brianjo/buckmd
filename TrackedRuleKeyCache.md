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
[Package]{.packageLabelInType} [com.facebook.buck.rules.keys](package-summary.html)
:::

## Class TrackedRuleKeyCache\<V\> {#class-trackedrulekeycachev .title title="Class TrackedRuleKeyCache"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.keys.TrackedRuleKeyCache\<V\>

::: description
-   

    [Type Parameters:]{.paramLabel}
    :   `V` -

    ```{=html}
    <!-- -->
    ```

    All Implemented Interfaces:
    :   `RuleKeyCache<V>`

    ------------------------------------------------------------------------

        public class TrackedRuleKeyCache<V>
        extends Object
        implements RuleKeyCache<V>

    ::: block
    A DefaultRuleKeyCache that records cache stats information in the
    corresponding CacheStatsTracker
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                Description
          ---------------------------------------------------------------------------------------------------------- -------------
          `TrackedRuleKeyCache​(TrackableRuleKeyCache<V> cache,                    CacheStatsTracker statsTracker)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `V`                   | `get​(Build            |                       |
        |                       | EngineAction action)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `V`                   | `get​(Buil             |                       |
        |                       | dEngineAction action, |                       |
        |                       |     java.util.functio |                       |
        |                       | n.Function<? super Bu |                       |
        |                       | ildEngineAction,​RuleK |                       |
        |                       | eyResult<V>> create)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `V`                   | `get​(                 |                       |
        |                       | AddsToRuleKey appenda |                       |
        |                       | ble,    java.util.fun |                       |
        |                       | ction.Function<? supe |                       |
        |                       | r AddsToRuleKey,​RuleK |                       |
        |                       | eyResult<V>> create)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `CacheStats`          | `getStats()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `invalidateAll()`     | ::: block             |
        |                       |                       | Invalidate everything |
        |                       |                       | in the cache.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `invalidateAllExcep   | ::: block             |
        |                       | tFilesystems​(com.goog | Invalidate all inputs |
        |                       | le.common.collect.Imm | \*not\* from the      |
        |                       | utableSet<ProjectFile | given                 |
        |                       | system> filesystems)` | [`Projec              |
        |                       |                       | tFilesystem`](../../i |
        |                       |                       | o/filesystem/ProjectF |
        |                       |                       | ilesystem.html "inter |
        |                       |                       | face in com.facebook. |
        |                       |                       | buck.io.filesystem")s |
        |                       |                       | and their transitive  |
        |                       |                       | dependents.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `invalidat            | ::: block             |
        |                       | eFilesystem​(ProjectFi | Invalidate all inputs |
        |                       | lesystem filesystem)` | from a given          |
        |                       |                       | [`Proje               |
        |                       |                       | ctFilesystem`](../../ |
        |                       |                       | io/filesystem/Project |
        |                       |                       | Filesystem.html "inte |
        |                       |                       | rface in com.facebook |
        |                       |                       | .buck.io.filesystem") |
        |                       |                       | and their transitive  |
        |                       |                       | dependents.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `invalidateInpu       | ::: block             |
        |                       | ts​(Iterable<com.faceb | Invalidate the given  |
        |                       | ook.buck.rules.keys.R | inputs and all their  |
        |                       | uleKeyInput> inputs)` | transitive            |
        |                       |                       | dependents.           |
        |                       |                       | :::                   |
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

        []{#<init>(com.facebook.buck.rules.keys.TrackableRuleKeyCache,com.facebook.buck.util.cache.CacheStatsTracker)}

        -   #### TrackedRuleKeyCache

                public TrackedRuleKeyCache​(TrackableRuleKeyCache<V> cache,
                                           CacheStatsTracker statsTracker)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#get(com.facebook.buck.core.build.action.BuildEngineAction)}

        -   #### get

            ``` methodSignature
            @Nullable
            public V get​(BuildEngineAction action)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `get` in interface `RuleKeyCache<V>`

            [Returns:]{.returnLabel}
            :   the rule key value for the given `action`, or null if it
                is not cached..

        []{#get(com.facebook.buck.core.build.action.BuildEngineAction,java.util.function.Function)}

        -   #### get

            ``` methodSignature
            public V get​(BuildEngineAction action,
                         java.util.function.Function<? super BuildEngineAction,​RuleKeyResult<V>> create)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `get` in interface `RuleKeyCache<V>`

            [Returns:]{.returnLabel}
            :   the rule key value for the given `rule`, either serving
                it form cache or by running the given function.

        []{#get(com.facebook.buck.core.rulekey.AddsToRuleKey,java.util.function.Function)}

        -   #### get

            ``` methodSignature
            public V get​(AddsToRuleKey appendable,
                         java.util.function.Function<? super AddsToRuleKey,​RuleKeyResult<V>> create)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `get` in interface `RuleKeyCache<V>`

            [Returns:]{.returnLabel}
            :   the rule key value for the given `appendable`, either
                serving it form cache or by running the given function.

        []{#invalidateInputs(java.lang.Iterable)}

        -   #### invalidateInputs

            ``` methodSignature
            public void invalidateInputs​(Iterable<com.facebook.buck.rules.keys.RuleKeyInput> inputs)
            ```

            ::: block
            [Description copied from
            interface: `RuleKeyCache`]{.descfrmTypeLabel}
            :::

            ::: block
            Invalidate the given inputs and all their transitive
            dependents.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `invalidateInputs` in interface `RuleKeyCache<V>`

        []{#invalidateAllExceptFilesystems(com.google.common.collect.ImmutableSet)}

        -   #### invalidateAllExceptFilesystems

            ``` methodSignature
            public void invalidateAllExceptFilesystems​(com.google.common.collect.ImmutableSet<ProjectFilesystem> filesystems)
            ```

            ::: block
            Invalidate all inputs \*not\* from the given
            [`ProjectFilesystem`](../../io/filesystem/ProjectFilesystem.html "interface in com.facebook.buck.io.filesystem")s
            and their transitive dependents.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `invalidateAllExceptFilesystems` in
                interface `RuleKeyCache<V>`

        []{#invalidateFilesystem(com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### invalidateFilesystem

            ``` methodSignature
            public void invalidateFilesystem​(ProjectFilesystem filesystem)
            ```

            ::: block
            Invalidate all inputs from a given
            [`ProjectFilesystem`](../../io/filesystem/ProjectFilesystem.html "interface in com.facebook.buck.io.filesystem")
            and their transitive dependents.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `invalidateFilesystem` in interface `RuleKeyCache<V>`

        []{#invalidateAll()}

        -   #### invalidateAll

            ``` methodSignature
            public void invalidateAll()
            ```

            ::: block
            Invalidate everything in the cache.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `invalidateAll` in interface `RuleKeyCache<V>`

        []{#getStats()}

        -   #### getStats

            ``` methodSignature
            public CacheStats getStats()
            ```

            [Returns:]{.returnLabel}
            :   the stats of the cache
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

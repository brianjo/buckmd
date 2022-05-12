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

## Class DefaultRuleKeyCache\<V\> {#class-defaultrulekeycachev .title title="Class DefaultRuleKeyCache"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.keys.DefaultRuleKeyCache\<V\>

::: description
-   

    [Type Parameters:]{.paramLabel}
    :   `V` - The rule key type.

    ```{=html}
    <!-- -->
    ```

    All Implemented Interfaces:
    :   `TrackableRuleKeyCache<V>`

    ------------------------------------------------------------------------

        public class DefaultRuleKeyCache<V>
        extends Object
        implements TrackableRuleKeyCache<V>

    ::: block
    A
    [`RuleKey`](../../core/rulekey/RuleKey.html "class in com.facebook.buck.core.rulekey")
    cache used by a
    [`RuleKeyFactory`](RuleKeyFactory.html "interface in com.facebook.buck.rules.keys").
    Inputs and dependencies of cached rule keys are tracked to allow for
    invalidations based on changed inputs. As such, this cache is usable
    between multiple build runs.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor               Description
          ------------------------- -------------
          `DefaultRuleKeyCache()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `V`                   | `ge                   |                       |
        |                       | t​(BuildEngineAction a |                       |
        |                       | ction,    CacheStatsT |                       |
        |                       | racker statsTracker)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `V`                   | `g                    |                       |
        |                       | et​(BuildEngineAction  |                       |
        |                       | action,    java.util. |                       |
        |                       | function.Function<? s |                       |
        |                       | uper BuildEngineActio |                       |
        |                       | n,​RuleKeyResult<V>> c |                       |
        |                       | reate,    CacheStatsT |                       |
        |                       | racker statsTracker)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `V`                   | `get​(AddsToRuleKey    |                       |
        |                       | appendable,    java.u |                       |
        |                       | til.function.Function |                       |
        |                       | <? super AddsToRuleKe |                       |
        |                       | y,​RuleKeyResult<V>> c |                       |
        |                       | reate,    CacheStatsT |                       |
        |                       | racker statsTracker)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `c                    | `g                    |                       |
        | om.google.common.coll | etCachedBuildRules()` |                       |
        | ect.ImmutableList<Map |                       |                       |
        | .Entry<BuildRule,​V>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `inva                 | ::: block             |
        |                       | lidateAll​(CacheStatsT | Invalidate everything |
        |                       | racker statsTracker)` | in the cache.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `invalidateAllExce    | ::: block             |
        |                       | ptFilesystems​(com.goo | Invalidate all inputs |
        |                       | gle.common.collect.Im | \*not\* from the      |
        |                       | mutableSet<ProjectFil | given                 |
        |                       | esystem> filesystems, | [`Projec              |
        |                       |                       | tFilesystem`](../../i |
        |                       |           CacheStatsT | o/filesystem/ProjectF |
        |                       | racker statsTracker)` | ilesystem.html "inter |
        |                       |                       | face in com.facebook. |
        |                       |                       | buck.io.filesystem")s |
        |                       |                       | and their transitive  |
        |                       |                       | dependents.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `invalidateFilesyste  | ::: block             |
        |                       | m​(ProjectFilesystem f | Invalidate all inputs |
        |                       | ilesystem,            | from a given          |
        |                       |           CacheStatsT | [`Proje               |
        |                       | racker statsTracker)` | ctFilesystem`](../../ |
        |                       |                       | io/filesystem/Project |
        |                       |                       | Filesystem.html "inte |
        |                       |                       | rface in com.facebook |
        |                       |                       | .buck.io.filesystem") |
        |                       |                       | and their transitive  |
        |                       |                       | dependents.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `invalidateInputs​(Ite | ::: block             |
        |                       | rable<com.facebook.bu | Invalidate the given  |
        |                       | ck.rules.keys.RuleKey | inputs and all their  |
        |                       | Input> inputs,        | transitive            |
        |                       |           CacheStatsT | dependents.           |
        |                       | racker statsTracker)` | :::                   |
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

        []{#<init>()}

        -   #### DefaultRuleKeyCache

                public DefaultRuleKeyCache()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#get(com.facebook.buck.core.build.action.BuildEngineAction,com.facebook.buck.util.cache.CacheStatsTracker)}

        -   #### get

            ``` methodSignature
            @Nullable
            public V get​(BuildEngineAction action,
                         CacheStatsTracker statsTracker)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `get` in interface `TrackableRuleKeyCache<V>`

        []{#get(com.facebook.buck.core.build.action.BuildEngineAction,java.util.function.Function,com.facebook.buck.util.cache.CacheStatsTracker)}

        -   #### get

            ``` methodSignature
            public V get​(BuildEngineAction action,
                         java.util.function.Function<? super BuildEngineAction,​RuleKeyResult<V>> create,
                         CacheStatsTracker statsTracker)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `get` in interface `TrackableRuleKeyCache<V>`

        []{#get(com.facebook.buck.core.rulekey.AddsToRuleKey,java.util.function.Function,com.facebook.buck.util.cache.CacheStatsTracker)}

        -   #### get

            ``` methodSignature
            public V get​(AddsToRuleKey appendable,
                         java.util.function.Function<? super AddsToRuleKey,​RuleKeyResult<V>> create,
                         CacheStatsTracker statsTracker)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `get` in interface `TrackableRuleKeyCache<V>`

        []{#invalidateInputs(java.lang.Iterable,com.facebook.buck.util.cache.CacheStatsTracker)}

        -   #### invalidateInputs

            ``` methodSignature
            public void invalidateInputs​(Iterable<com.facebook.buck.rules.keys.RuleKeyInput> inputs,
                                         CacheStatsTracker statsTracker)
            ```

            ::: block
            Invalidate the given inputs and all their transitive
            dependents.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `invalidateInputs` in
                interface `TrackableRuleKeyCache<V>`

        []{#invalidateAllExceptFilesystems(com.google.common.collect.ImmutableSet,com.facebook.buck.util.cache.CacheStatsTracker)}

        -   #### invalidateAllExceptFilesystems

            ``` methodSignature
            public void invalidateAllExceptFilesystems​(com.google.common.collect.ImmutableSet<ProjectFilesystem> filesystems,
                                                       CacheStatsTracker statsTracker)
            ```

            ::: block
            Invalidate all inputs \*not\* from the given
            [`ProjectFilesystem`](../../io/filesystem/ProjectFilesystem.html "interface in com.facebook.buck.io.filesystem")s
            and their transitive dependents.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `invalidateAllExceptFilesystems` in
                interface `TrackableRuleKeyCache<V>`

        []{#invalidateFilesystem(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.util.cache.CacheStatsTracker)}

        -   #### invalidateFilesystem

            ``` methodSignature
            public void invalidateFilesystem​(ProjectFilesystem filesystem,
                                             CacheStatsTracker statsTracker)
            ```

            ::: block
            Invalidate all inputs from a given
            [`ProjectFilesystem`](../../io/filesystem/ProjectFilesystem.html "interface in com.facebook.buck.io.filesystem")
            and their transitive dependents.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `invalidateFilesystem` in
                interface `TrackableRuleKeyCache<V>`

        []{#invalidateAll(com.facebook.buck.util.cache.CacheStatsTracker)}

        -   #### invalidateAll

            ``` methodSignature
            public void invalidateAll​(CacheStatsTracker statsTracker)
            ```

            ::: block
            Invalidate everything in the cache.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `invalidateAll` in interface `TrackableRuleKeyCache<V>`

        []{#getCachedBuildRules()}

        -   #### getCachedBuildRules

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Map.Entry<BuildRule,​V>> getCachedBuildRules()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCachedBuildRules` in
                interface `TrackableRuleKeyCache<V>`
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

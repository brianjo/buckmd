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

## Interface RuleKeyCache\<V\> {#interface-rulekeycachev .title title="Interface RuleKeyCache"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `TrackedRuleKeyCache`

    ------------------------------------------------------------------------

        public interface RuleKeyCache<V>

    ::: block
    Interface for caches for rule keys.
    :::
:::

::: summary
-   ::: {.section role="region"}
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
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#get(com.facebook.buck.core.build.action.BuildEngineAction)}

        -   #### get

            ``` methodSignature
            @Nullable
            V get​(BuildEngineAction action)
            ```

            [Returns:]{.returnLabel}
            :   the rule key value for the given `action`, or null if it
                is not cached..

        []{#get(com.facebook.buck.core.build.action.BuildEngineAction,java.util.function.Function)}

        -   #### get

            ``` methodSignature
            V get​(BuildEngineAction action,
                  java.util.function.Function<? super BuildEngineAction,​RuleKeyResult<V>> create)
            ```

            [Returns:]{.returnLabel}
            :   the rule key value for the given `rule`, either serving
                it form cache or by running the given function.

        []{#get(com.facebook.buck.core.rulekey.AddsToRuleKey,java.util.function.Function)}

        -   #### get

            ``` methodSignature
            V get​(AddsToRuleKey appendable,
                  java.util.function.Function<? super AddsToRuleKey,​RuleKeyResult<V>> create)
            ```

            [Returns:]{.returnLabel}
            :   the rule key value for the given `appendable`, either
                serving it form cache or by running the given function.

        []{#invalidateInputs(java.lang.Iterable)}

        -   #### invalidateInputs

            ``` methodSignature
            void invalidateInputs​(Iterable<com.facebook.buck.rules.keys.RuleKeyInput> inputs)
            ```

            ::: block
            Invalidate the given inputs and all their transitive
            dependents.
            :::

        []{#invalidateAllExceptFilesystems(com.google.common.collect.ImmutableSet)}

        -   #### invalidateAllExceptFilesystems

            ``` methodSignature
            void invalidateAllExceptFilesystems​(com.google.common.collect.ImmutableSet<ProjectFilesystem> filesystems)
            ```

            ::: block
            Invalidate all inputs \*not\* from the given
            [`ProjectFilesystem`](../../io/filesystem/ProjectFilesystem.html "interface in com.facebook.buck.io.filesystem")s
            and their transitive dependents.
            :::

        []{#invalidateFilesystem(com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### invalidateFilesystem

            ``` methodSignature
            void invalidateFilesystem​(ProjectFilesystem filesystem)
            ```

            ::: block
            Invalidate all inputs from a given
            [`ProjectFilesystem`](../../io/filesystem/ProjectFilesystem.html "interface in com.facebook.buck.io.filesystem")
            and their transitive dependents.
            :::

        []{#invalidateAll()}

        -   #### invalidateAll

            ``` methodSignature
            void invalidateAll()
            ```

            ::: block
            Invalidate everything in the cache.
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

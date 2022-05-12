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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.impl](package-summary.html)
:::

## Class AbstractBuildRuleResolver {#class-abstractbuildruleresolver .title title="Class AbstractBuildRuleResolver"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.rules.impl.AbstractBuildRuleResolver

::: description
-   

    All Implemented Interfaces:
    :   `BuildRuleResolver`, `SourcePathRuleFinder`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `AbstractActionGraphBuilder`

    ------------------------------------------------------------------------

        public abstract class AbstractBuildRuleResolver
        extends Object
        implements BuildRuleResolver

    ::: block
    An abstract implementation of BuildTargetResolver that simplifies
    concrete implementations.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                     Description
          -------------- ------------------------------- -------------
          `protected `   `AbstractBuildRuleResolver()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.goog             | `fil                  |                       |
        | le.common.collect.Imm | terBuildRuleInputs​(So |                       |
        | utableSet<BuildRule>` | urcePath... sources)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.goog             | `filterBuildRuleInput |                       |
        | le.common.collect.Imm | s​(Iterable<? extends  |                       |
        | utableSet<BuildRule>` | SourcePath> sources)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `java.util.stre       | `filterBuildRu        |                       |
        | am.Stream<BuildRule>` | leInputs​(Optional<Sou |                       |
        |                       | rcePath> sourcePath)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `java.util.stre       | `filt                 |                       |
        | am.Stream<BuildRule>` | erBuildRuleInputs​(jav |                       |
        |                       | a.util.stream.Stream< |                       |
        |                       | SourcePath> sources)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.com       | `g                    |                       |
        | mon.collect.Immutable | etAllRules​(Iterable<B |                       |
        | SortedSet<BuildRule>` | uildTarget> targets)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuildRule`           | `getRule​(Buil         | ::: block             |
        |                       | dTarget buildTarget)` | Returns the           |
        |                       |                       | `BuildRule`           |
        |                       |                       | associated with the   |
        |                       |                       | `buildTarget`.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `BuildRule`           | `                     |                       |
        |                       | getRule​(BuildTargetSo |                       |
        |                       | urcePath sourcePath)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<BuildRule>` | `getRule​(So           |                       |
        |                       | urcePath sourcePath)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `<T> Optional<T>`     | `ge                   | ::: block             |
        |                       | tRuleOptionalWithType | Returns the           |
        |                       | ​(BuildTarget buildTar | `BuildRule`           |
        |                       | get,                  | associated with the   |
        |                       |        Class<T> cls)` | given `BuildTarget`   |
        |                       |                       | if it is already      |
        |                       |                       | present, casting it   |
        |                       |                       | to an expected type.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `<T> T`               | `getRule              | ::: block             |
        |                       | WithType​(BuildTarget  | Returns the           |
        |                       | buildTarget,          | `BuildRule`           |
        |                       |        Class<T> cls)` | associated with the   |
        |                       |                       | `buildTarget`,        |
        |                       |                       | casting it to an      |
        |                       |                       | expected type.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Sourc                | `get                  |                       |
        | ePathResolverAdapter` | SourcePathResolver()` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.BuildRuleResolver}

            ### Methods inherited from interface com.facebook.buck.core.rules.[BuildRuleResolver](../BuildRuleResolver.html "interface in com.facebook.buck.core.rules")

            `getRuleOptional`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### AbstractBuildRuleResolver

                protected AbstractBuildRuleResolver()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getRuleOptionalWithType(com.facebook.buck.core.model.BuildTarget,java.lang.Class)}

        -   #### getRuleOptionalWithType

            ``` methodSignature
            public <T> Optional<T> getRuleOptionalWithType​(BuildTarget buildTarget,
                                                           Class<T> cls)
            ```

            ::: block
            [Description copied from
            interface: `BuildRuleResolver`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns the `BuildRule` associated with the given
            `BuildTarget` if it is already present, casting it to an
            expected type.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRuleOptionalWithType` in
                interface `BuildRuleResolver`

        []{#getRule(com.facebook.buck.core.model.BuildTarget)}

        -   #### getRule

            ``` methodSignature
            public BuildRule getRule​(BuildTarget buildTarget)
            ```

            ::: block
            [Description copied from
            interface: `BuildRuleResolver`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns the `BuildRule` associated with the `buildTarget`.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRule` in interface `BuildRuleResolver`

        []{#getRuleWithType(com.facebook.buck.core.model.BuildTarget,java.lang.Class)}

        -   #### getRuleWithType

            ``` methodSignature
            public <T> T getRuleWithType​(BuildTarget buildTarget,
                                         Class<T> cls)
            ```

            ::: block
            [Description copied from
            interface: `BuildRuleResolver`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns the `BuildRule` associated with the `buildTarget`,
            casting it to an expected type.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRuleWithType` in interface `BuildRuleResolver`

        []{#getAllRules(java.lang.Iterable)}

        -   #### getAllRules

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<BuildRule> getAllRules​(Iterable<BuildTarget> targets)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getAllRules` in interface `BuildRuleResolver`

        []{#filterBuildRuleInputs(java.lang.Iterable)}

        -   #### filterBuildRuleInputs

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<BuildRule> filterBuildRuleInputs​(Iterable<? extends SourcePath> sources)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `filterBuildRuleInputs` in
                interface `SourcePathRuleFinder`

        []{#filterBuildRuleInputs(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### filterBuildRuleInputs

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<BuildRule> filterBuildRuleInputs​(SourcePath... sources)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `filterBuildRuleInputs` in
                interface `SourcePathRuleFinder`

        []{#filterBuildRuleInputs(java.util.stream.Stream)}

        -   #### filterBuildRuleInputs

            ``` methodSignature
            public java.util.stream.Stream<BuildRule> filterBuildRuleInputs​(java.util.stream.Stream<SourcePath> sources)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `filterBuildRuleInputs` in
                interface `SourcePathRuleFinder`

        []{#filterBuildRuleInputs(java.util.Optional)}

        -   #### filterBuildRuleInputs

            ``` methodSignature
            public java.util.stream.Stream<BuildRule> filterBuildRuleInputs​(Optional<SourcePath> sourcePath)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `filterBuildRuleInputs` in
                interface `SourcePathRuleFinder`

        []{#getRule(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### getRule

            ``` methodSignature
            public Optional<BuildRule> getRule​(SourcePath sourcePath)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRule` in interface `SourcePathRuleFinder`

            [Returns:]{.returnLabel}
            :   An
                [`Optional`](http://docs.oracle.com/javase/7/docs/api/java/util/Optional.html?is-external=true "class or interface in java.util"){.externalLink}
                containing the
                [`BuildRule`](../BuildRule.html "interface in com.facebook.buck.core.rules")
                whose output `sourcePath` refers to, or `absent` if
                `sourcePath` doesn\'t refer to the output of a
                [`BuildRule`](../BuildRule.html "interface in com.facebook.buck.core.rules").

        []{#getRule(com.facebook.buck.core.sourcepath.BuildTargetSourcePath)}

        -   #### getRule

            ``` methodSignature
            public BuildRule getRule​(BuildTargetSourcePath sourcePath)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRule` in interface `SourcePathRuleFinder`

            [Returns:]{.returnLabel}
            :   The
                [`BuildRule`](../BuildRule.html "interface in com.facebook.buck.core.rules")
                whose output `sourcePath` refers to its output.

        []{#getSourcePathResolver()}

        -   #### getSourcePathResolver

            ``` methodSignature
            public SourcePathResolverAdapter getSourcePathResolver()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourcePathResolver` in
                interface `SourcePathRuleFinder`
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

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
-   [Enum Constants](#enum.constant.summary) \| 
-   Field \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Enum Constants](#enum.constant.detail) \| 
-   Field \| 
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

## Enum BuildRuleSuccessType {#enum-buildrulesuccesstype .title title="Enum BuildRuleSuccessType"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<[BuildRuleSuccessType](BuildRuleSuccessType.html "enum in com.facebook.buck.core.build.engine")\>

    -   -   com.facebook.buck.core.build.engine.BuildRuleSuccessType

::: description
-   

    All Implemented Interfaces:
    :   `Serializable`, `Comparable<BuildRuleSuccessType>`

    ------------------------------------------------------------------------

        public enum BuildRuleSuccessType
        extends Enum<BuildRuleSuccessType>

    ::: block
    Token provided by the result of
    [`BuildEngine.build(BuildEngineBuildContext,  ExecutionContext, BuildRule)`](BuildEngine.html#build(com.facebook.buck.core.build.engine.BuildEngineBuildContext,com.facebook.buck.core.build.execution.context.ExecutionContext,com.facebook.buck.core.rules.BuildRule)),
    demonstrating that the associated
    [`BuildRule`](../../rules/BuildRule.html "interface in com.facebook.buck.core.rules")
    was built successfully.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#enum.constant.summary}

        ### Enum Constant Summary

        +-----------------------------------+-----------------------------------+
        | Enum Constant                     | Description                       |
        +===================================+===================================+
        | `BUILT_LOCALLY`                   | ::: block                         |
        |                                   | Built by executing the            |
        |                                   | [`Step                            |
        |                                   | `](../../../step/Step.html "inter |
        |                                   | face in com.facebook.buck.step")s |
        |                                   | for the rule.                     |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `FETCHED_FROM_CACHE`              | ::: block                         |
        |                                   | Fetched via the                   |
        |                                   | [`ArtifactC                       |
        |                                   | ache`](../../../artifact_cache/Ar |
        |                                   | tifactCache.html "interface in co |
        |                                   | m.facebook.buck.artifact_cache"). |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `FETCHED_FROM_CACHE_INPUT_BASED`  | ::: block                         |
        |                                   | Fetched via the                   |
        |                                   | [`Artifact                        |
        |                                   | Cache`](../../../artifact_cache/A |
        |                                   | rtifactCache.html "interface in c |
        |                                   | om.facebook.buck.artifact_cache") |
        |                                   | using an input-based rule key.    |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `F                                | ::: block                         |
        | ETCHED_FROM_CACHE_MANIFEST_BASED` | Fetched via the                   |
        |                                   | [`Artifact                        |
        |                                   | Cache`](../../../artifact_cache/A |
        |                                   | rtifactCache.html "interface in c |
        |                                   | om.facebook.buck.artifact_cache") |
        |                                   | using an input-based rule key.    |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `MATCHING_DEP_FILE_RULE_KEY`      | ::: block                         |
        |                                   | Computed dep-file                 |
        |                                   | [`RuleKey`](../                   |
        |                                   | ../rulekey/RuleKey.html "class in |
        |                                   |  com.facebook.buck.core.rulekey") |
        |                                   | matches the one on disk           |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `MATCHING_INPUT_BASED_RULE_KEY`   | ::: block                         |
        |                                   | Computed input-based              |
        |                                   | [`RuleKey`](../                   |
        |                                   | ../rulekey/RuleKey.html "class in |
        |                                   |  com.facebook.buck.core.rulekey") |
        |                                   | matches the one on disk.          |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `MATCHING_RULE_KEY`               | ::: block                         |
        |                                   | Computed                          |
        |                                   | [`RuleKey`](../                   |
        |                                   | ../rulekey/RuleKey.html "class in |
        |                                   |  com.facebook.buck.core.rulekey") |
        |                                   | matches the one on disk.          |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+

        : Enum Constants[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `String`              | `g                    |                       |
        |                       | etShortDescription()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `                     |                       |
        |                       | outputsHaveChanged()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `shouldClearAndOverw  |                       |
        |                       | riteMetadataOnDisk()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `shouldUploa          |                       |
        |                       | dResultingArtifact()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `shouldW              |                       |
        |                       | riteRecordedMetadataT |                       |
        |                       | oDiskAfterBuilding()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `                     | ::: block             |
        | BuildRuleSuccessType` | valueOf​(String name)` | Returns the enum      |
        |                       |                       | constant of this type |
        |                       |                       | with the specified    |
        |                       |                       | name.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Bu            | `values()`            | ::: block             |
        | ildRuleSuccessType[]` |                       | Returns an array      |
        |                       |                       | containing the        |
        |                       |                       | constants of this     |
        |                       |                       | enum type, in the     |
        |                       |                       | order they are        |
        |                       |                       | declared.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Enum}

            ### Methods inherited from class java.lang.[Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, compareTo, equals, finalize, getDeclaringClass, hashCode, name, ordinal, toString, valueOf`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `getClass, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#enum.constant.detail}

        ### Enum Constant Detail

        []{#BUILT_LOCALLY}

        -   #### BUILT_LOCALLY

                public static final BuildRuleSuccessType BUILT_LOCALLY

            ::: block
            Built by executing the
            [`Step`](../../../step/Step.html "interface in com.facebook.buck.step")s
            for the rule.
            :::

        []{#FETCHED_FROM_CACHE}

        -   #### FETCHED_FROM_CACHE

                public static final BuildRuleSuccessType FETCHED_FROM_CACHE

            ::: block
            Fetched via the
            [`ArtifactCache`](../../../artifact_cache/ArtifactCache.html "interface in com.facebook.buck.artifact_cache").
            :::

        []{#FETCHED_FROM_CACHE_INPUT_BASED}

        -   #### FETCHED_FROM_CACHE_INPUT_BASED

                public static final BuildRuleSuccessType FETCHED_FROM_CACHE_INPUT_BASED

            ::: block
            Fetched via the
            [`ArtifactCache`](../../../artifact_cache/ArtifactCache.html "interface in com.facebook.buck.artifact_cache")
            using an input-based rule key.
            :::

        []{#FETCHED_FROM_CACHE_MANIFEST_BASED}

        -   #### FETCHED_FROM_CACHE_MANIFEST_BASED

                public static final BuildRuleSuccessType FETCHED_FROM_CACHE_MANIFEST_BASED

            ::: block
            Fetched via the
            [`ArtifactCache`](../../../artifact_cache/ArtifactCache.html "interface in com.facebook.buck.artifact_cache")
            using an input-based rule key.
            :::

        []{#MATCHING_RULE_KEY}

        -   #### MATCHING_RULE_KEY

                public static final BuildRuleSuccessType MATCHING_RULE_KEY

            ::: block
            Computed
            [`RuleKey`](../../rulekey/RuleKey.html "class in com.facebook.buck.core.rulekey")
            matches the one on disk.
            :::

        []{#MATCHING_INPUT_BASED_RULE_KEY}

        -   #### MATCHING_INPUT_BASED_RULE_KEY

                public static final BuildRuleSuccessType MATCHING_INPUT_BASED_RULE_KEY

            ::: block
            Computed input-based
            [`RuleKey`](../../rulekey/RuleKey.html "class in com.facebook.buck.core.rulekey")
            matches the one on disk.
            :::

        []{#MATCHING_DEP_FILE_RULE_KEY}

        -   #### MATCHING_DEP_FILE_RULE_KEY

                public static final BuildRuleSuccessType MATCHING_DEP_FILE_RULE_KEY

            ::: block
            Computed dep-file
            [`RuleKey`](../../rulekey/RuleKey.html "class in com.facebook.buck.core.rulekey")
            matches the one on disk
            :::
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#values()}

        -   #### values

            ``` methodSignature
            public static BuildRuleSuccessType[] values()
            ```

            ::: block
            Returns an array containing the constants of this enum type,
            in the order they are declared. This method may be used to
            iterate over the constants as follows:
                for (BuildRuleSuccessType c : BuildRuleSuccessType.values())
                    System.out.println(c);
            :::

            [Returns:]{.returnLabel}
            :   an array containing the constants of this enum type, in
                the order they are declared

        []{#valueOf(java.lang.String)}

        -   #### valueOf

            ``` methodSignature
            public static BuildRuleSuccessType valueOf​(String name)
            ```

            ::: block
            Returns the enum constant of this type with the specified
            name. The string must match *exactly* an identifier used to
            declare an enum constant in this type. (Extraneous
            whitespace characters are not permitted.)
            :::

            [Parameters:]{.paramLabel}
            :   `name` - the name of the enum constant to be returned.

            [Returns:]{.returnLabel}
            :   the enum constant with the specified name

            [Throws:]{.throwsLabel}
            :   `IllegalArgumentException` - if this enum type has no
                constant with the specified name
            :   `NullPointerException` - if the argument is null

        []{#shouldWriteRecordedMetadataToDiskAfterBuilding()}

        -   #### shouldWriteRecordedMetadataToDiskAfterBuilding

            ``` methodSignature
            public boolean shouldWriteRecordedMetadataToDiskAfterBuilding()
            ```

        []{#shouldClearAndOverwriteMetadataOnDisk()}

        -   #### shouldClearAndOverwriteMetadataOnDisk

            ``` methodSignature
            public boolean shouldClearAndOverwriteMetadataOnDisk()
            ```

        []{#shouldUploadResultingArtifact()}

        -   #### shouldUploadResultingArtifact

            ``` methodSignature
            public boolean shouldUploadResultingArtifact()
            ```

        []{#outputsHaveChanged()}

        -   #### outputsHaveChanged

            ``` methodSignature
            public boolean outputsHaveChanged()
            ```

        []{#getShortDescription()}

        -   #### getShortDescription

            ``` methodSignature
            public String getShortDescription()
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
-   [Enum Constants](#enum.constant.summary) \| 
-   Field \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Enum Constants](#enum.constant.detail) \| 
-   Field \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

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

## Class AbstractRuleKeyBuilder\<RULE_KEY\> {#class-abstractrulekeybuilderrule_key .title title="Class AbstractRuleKeyBuilder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.keys.AbstractRuleKeyBuilder\<RULE_KEY\>

::: description
-   

    Direct Known Subclasses:
    :   `RuleKeyBuilder`

    ------------------------------------------------------------------------

        public abstract class AbstractRuleKeyBuilder<RULE_KEY>
        extends Object

    ::: block
    Base class for rulekey builders. Implements much of the logic of
    computing keys from
    [`AddToRuleKey`](../../core/rulekey/AddToRuleKey.html "annotation in com.facebook.buck.core.rulekey")-annotated
    fields.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                                                  Description
          -------------- ------------------------------------------------------------ -------------
          `protected `   `AbstractRuleKeyBuilder​(RuleKeyScopedHasher scopedHasher)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `abstract RULE_KEY`   | `build()`             |                       |
        +-----------------------+-----------------------+-----------------------+
        | `<RESULT> RESULT`     | `build​(java.util.f    | ::: block             |
        |                       | unction.Function<RULE | A convenience method  |
        |                       | _KEY,​RESULT> mapper)` | that builds the rule  |
        |                       |                       | key hash and          |
        |                       |                       | transforms it with a  |
        |                       |                       | mapper.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `protected            | `setA                 |                       |
        | abstract AbstractRule | ction​(Action action)` |                       |
        | KeyBuilder<RULE_KEY>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected            | `s                    |                       |
        | abstract AbstractRule | etAddsToRuleKey​(AddsT |                       |
        | KeyBuilder<RULE_KEY>` | oRuleKey appendable)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected            | `setBuild             |                       |
        | abstract AbstractRule | Rule​(BuildRule rule)` |                       |
        | KeyBuilder<RULE_KEY>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected            | `setNo                |                       |
        | abstract AbstractRule | nHashingSourcePath​(So |                       |
        | KeyBuilder<RULE_KEY>` | urcePath sourcePath)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `p                    | `setRefl              | ::: block             |
        | rotected AbstractRule | ectively​(Object val)` | Recursively           |
        | KeyBuilder<RULE_KEY>` |                       | serializes the value. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AbstractRule         | `setReflective        | ::: block             |
        | KeyBuilder<RULE_KEY>` | ly​(String key,        | Adds the key-value    |
        |                       |          Object val)` | pair to the rulekey.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AbstractRule         | `setR                 | ::: block             |
        | KeyBuilder<RULE_KEY>` | eflectivelyPathKey​(Pa | Adds the key-value    |
        |                       | th key,               | pair to the rulekey.  |
        |                       |          Object val)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `protected            | `setSin               |                       |
        | abstract AbstractRule | gleValue​(Object val)` |                       |
        | KeyBuilder<RULE_KEY>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected            | `setSourcePath​(So     |                       |
        | abstract AbstractRule | urcePath sourcePath)` |                       |
        | KeyBuilder<RULE_KEY>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
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

        []{#<init>(com.facebook.buck.rules.keys.RuleKeyScopedHasher)}

        -   #### AbstractRuleKeyBuilder

                protected AbstractRuleKeyBuilder​(RuleKeyScopedHasher scopedHasher)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#setReflectively(java.lang.String,java.lang.Object)}

        -   #### setReflectively

            ``` methodSignature
            public final AbstractRuleKeyBuilder<RULE_KEY> setReflectively​(String key,
                                                                          @Nullable
                                                                          Object val)
            ```

            ::: block
            Adds the key-value pair to the rulekey. If the builder skips
            adding the value, the key will also be skipped.
            :::

        []{#setReflectivelyPathKey(java.nio.file.Path,java.lang.Object)}

        -   #### setReflectivelyPathKey

            ``` methodSignature
            public AbstractRuleKeyBuilder<RULE_KEY> setReflectivelyPathKey​(Path key,
                                                                           @Nullable
                                                                           Object val)
            ```

            ::: block
            Adds the key-value pair to the rulekey. If the builder skips
            adding the value, the key will also be skipped.
            :::

        []{#setReflectively(java.lang.Object)}

        -   #### setReflectively

            ``` methodSignature
            protected AbstractRuleKeyBuilder<RULE_KEY> setReflectively​(@Nullable
                                                                       Object val)
                                                                throws IOException
            ```

            ::: block
            Recursively serializes the value. Serialization of the key
            is handled outside.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#setSingleValue(java.lang.Object)}

        -   #### setSingleValue

            ``` methodSignature
            protected abstract AbstractRuleKeyBuilder<RULE_KEY> setSingleValue​(@Nullable
                                                                               Object val)
            ```

        []{#setAction(com.facebook.buck.core.rules.actions.Action)}

        -   #### setAction

            ``` methodSignature
            protected abstract AbstractRuleKeyBuilder<RULE_KEY> setAction​(Action action)
            ```

        []{#setBuildRule(com.facebook.buck.core.rules.BuildRule)}

        -   #### setBuildRule

            ``` methodSignature
            protected abstract AbstractRuleKeyBuilder<RULE_KEY> setBuildRule​(BuildRule rule)
            ```

        []{#setAddsToRuleKey(com.facebook.buck.core.rulekey.AddsToRuleKey)}

        -   #### setAddsToRuleKey

            ``` methodSignature
            protected abstract AbstractRuleKeyBuilder<RULE_KEY> setAddsToRuleKey​(AddsToRuleKey appendable)
            ```

        []{#setSourcePath(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setSourcePath

            ``` methodSignature
            protected abstract AbstractRuleKeyBuilder<RULE_KEY> setSourcePath​(SourcePath sourcePath)
                                                                       throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#setNonHashingSourcePath(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setNonHashingSourcePath

            ``` methodSignature
            protected abstract AbstractRuleKeyBuilder<RULE_KEY> setNonHashingSourcePath​(SourcePath sourcePath)
            ```

        []{#build()}

        -   #### build

            ``` methodSignature
            public abstract RULE_KEY build()
            ```

        []{#build(java.util.function.Function)}

        -   #### build

            ``` methodSignature
            public final <RESULT> RESULT build​(java.util.function.Function<RULE_KEY,​RESULT> mapper)
            ```

            ::: block
            A convenience method that builds the rule key hash and
            transforms it with a mapper.
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

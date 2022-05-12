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

## Class RuleKeyBuilder\<RULE_KEY\> {#class-rulekeybuilderrule_key .title title="Class RuleKeyBuilder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.rules.keys.AbstractRuleKeyBuilder](AbstractRuleKeyBuilder.html "class in com.facebook.buck.rules.keys")\<RULE_KEY\>

    -   -   com.facebook.buck.rules.keys.RuleKeyBuilder\<RULE_KEY\>

::: description
-   

    [Type Parameters:]{.paramLabel}
    :   `RULE_KEY` - - the actual type that the builder produces (e.g.
        `HashCode`).

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `ContentAgnosticRuleKeyFactory.Builder`,
        `DefaultRuleKeyFactory.Builder`

    ------------------------------------------------------------------------

        public abstract class RuleKeyBuilder<RULE_KEY>
        extends AbstractRuleKeyBuilder<RULE_KEY>

    ::: block
    A base implementation for rule key builders.
    [`RuleKeyFactory`](RuleKeyFactory.html "interface in com.facebook.buck.rules.keys")
    classes create concrete instances of this class and use them to
    produce rule keys. Concrete implementations may tweak behavior of
    the builder, and at the very minimum should implement
    [`AbstractRuleKeyBuilder.setAddsToRuleKey(AddsToRuleKey)`](AbstractRuleKeyBuilder.html#setAddsToRuleKey(com.facebook.buck.core.rulekey.AddsToRuleKey)),
    and
    [`AbstractRuleKeyBuilder.setBuildRule(BuildRule)`](AbstractRuleKeyBuilder.html#setBuildRule(com.facebook.buck.core.rules.BuildRule)).

    This class implements
    [`AbstractRuleKeyBuilder`](AbstractRuleKeyBuilder.html "class in com.facebook.buck.rules.keys")
    interface which is the primary mechanism of how
    [`RuleKeyFactory`](RuleKeyFactory.html "interface in com.facebook.buck.rules.keys")
    and
    [`AddsToRuleKey`](../../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey")
    classes feed the builder.

    Each element fed to the builder is a (key, value) pair. Keys are
    always simple strings, typically the name of a field annotated with
    [`AddToRuleKey`](../../core/rulekey/AddToRuleKey.html "annotation in com.facebook.buck.core.rulekey").
    Values on the other hand may be complex types that are resolved
    recursively. For instance, a list of elements gets serialized by
    serializing each element of the list in order, and finally
    serializing the list token along with the length of the list.
    Similarly for other containers and wrappers.

    There is an exception to the above rule of how containers and
    wrappers get serialized. Namely, they only get serialized if at
    least one of their elements gets serialized. This is to support
    concrete rule key builders that ignore some elements, or handle them
    differently. For example, several concrete builders handle
    [`SourcePath`](../../core/sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")
    elements in a special way.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                        Description
          -------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `RuleKeyBuilder​(SourcePathRuleFinder ruleFinder,               FileHashLoader hashLoader,               CountingRuleKeyHasher<RULE_KEY> hasher)`    
          `RuleKeyBuilder​(SourcePathRuleFinder ruleFinder,               FileHashLoader hashLoader,               RuleKeyHasher<RULE_KEY> hasher)`            

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `RULE_KEY`            | `build()`             | ::: block             |
        |                       |                       | Builds the rule key   |
        |                       |                       | hash.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `protected Rule       | `s                    |                       |
        | KeyBuilder<RULE_KEY>` | etPath​(ProjectFilesys |                       |
        |                       | tem filesystem,       |                       |
        |                       |   Path relativePath)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Rule                 | `setPath​(Path a       |                       |
        | KeyBuilder<RULE_KEY>` | bsolutePath,        P |                       |
        |                       | ath ideallyRelative)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected Rule       | `setSin               |                       |
        | KeyBuilder<RULE_KEY>` | gleValue​(Object val)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.rules.keys.AbstractRuleKeyBuilder}

            ### Methods inherited from class com.facebook.buck.rules.keys.[AbstractRuleKeyBuilder](AbstractRuleKeyBuilder.html "class in com.facebook.buck.rules.keys")

            `build, setAction, setAddsToRuleKey, setBuildRule, setNonHashingSourcePath, setReflectively, setReflectively, setReflectivelyPathKey, setSourcePath`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.rules.SourcePathRuleFinder,com.facebook.buck.util.hashing.FileHashLoader,com.facebook.buck.rules.keys.hasher.CountingRuleKeyHasher)}

        -   #### RuleKeyBuilder

                public RuleKeyBuilder​(SourcePathRuleFinder ruleFinder,
                                      FileHashLoader hashLoader,
                                      CountingRuleKeyHasher<RULE_KEY> hasher)

        []{#<init>(com.facebook.buck.core.rules.SourcePathRuleFinder,com.facebook.buck.util.hashing.FileHashLoader,com.facebook.buck.rules.keys.hasher.RuleKeyHasher)}

        -   #### RuleKeyBuilder

                public RuleKeyBuilder​(SourcePathRuleFinder ruleFinder,
                                      FileHashLoader hashLoader,
                                      RuleKeyHasher<RULE_KEY> hasher)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#setPath(java.nio.file.Path,java.nio.file.Path)}

        -   #### setPath

            ``` methodSignature
            public RuleKeyBuilder<RULE_KEY> setPath​(Path absolutePath,
                                                    Path ideallyRelative)
                                             throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#setPath(com.facebook.buck.io.filesystem.ProjectFilesystem,java.nio.file.Path)}

        -   #### setPath

            ``` methodSignature
            protected RuleKeyBuilder<RULE_KEY> setPath​(ProjectFilesystem filesystem,
                                                       Path relativePath)
                                                throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#setSingleValue(java.lang.Object)}

        -   #### setSingleValue

            ``` methodSignature
            protected final RuleKeyBuilder<RULE_KEY> setSingleValue​(@Nullable
                                                                    Object val)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `setSingleValue` in
                class `AbstractRuleKeyBuilder<RULE_KEY>`

        []{#build()}

        -   #### build

            ``` methodSignature
            public final RULE_KEY build()
            ```

            ::: block
            Builds the rule key hash.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `build` in class `AbstractRuleKeyBuilder<RULE_KEY>`
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

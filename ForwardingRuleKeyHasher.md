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
-   [Nested](#nested.class.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.rules.keys.hasher](package-summary.html)
:::

## Class ForwardingRuleKeyHasher\<HASH,​HASH2\> {#class-forwardingrulekeyhasherhashhash2 .title title="Class ForwardingRuleKeyHasher"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.keys.hasher.ForwardingRuleKeyHasher\<HASH,​HASH2\>

::: description
-   

    All Implemented Interfaces:
    :   `RuleKeyHasher<HASH>`

    ------------------------------------------------------------------------

        public abstract class ForwardingRuleKeyHasher<HASH,​HASH2>
        extends Object
        implements RuleKeyHasher<HASH>

    ::: block
    A
    [`RuleKeyHasher`](RuleKeyHasher.html "interface in com.facebook.buck.rules.keys.hasher")
    that forwards all the methods to the two underlying hashers.
    [`hash()`](#hash()) invokes the method of the both underlying
    hashers and returns the hash of the first one.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.rules.keys.hasher.RuleKeyHasher}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.rules.keys.hasher.[RuleKeyHasher](RuleKeyHasher.html "interface in com.facebook.buck.rules.keys.hasher")

            `RuleKeyHasher.Container, RuleKeyHasher.Wrapper`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                                                                                                            Description
          -------------- ---------------------------------------------------------------------------------------------------------------------- -------------
          `protected `   `ForwardingRuleKeyHasher​(RuleKeyHasher<HASH> firstHasher,                        RuleKeyHasher<HASH2> secondHasher)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `HASH`                | `hash()`              | ::: block             |
        |                       |                       | Computes the final    |
        |                       |                       | hash.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `pro                  | `onHas                |                       |
        | tected abstract void` | h​(HASH firstHash,     |                       |
        |                       |    HASH2 secondHash)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ForwardingRuleK      | `pu                   |                       |
        | eyHasher<HASH,​HASH2>` | tArchiveMemberPath​(Pa |                       |
        |                       | th relativeArchivePat |                       |
        |                       | h,                    |                       |
        |                       |   Path archiveMemberP |                       |
        |                       | ath,                  |                       |
        |                       |     com.google.common |                       |
        |                       | .hash.HashCode hash)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ForwardingRuleK      | `put                  |                       |
        | eyHasher<HASH,​HASH2>` | Boolean​(boolean val)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ForwardingRuleK      | `putBuildTarget​(Buil  |                       |
        | eyHasher<HASH,​HASH2>` | dTarget buildTarget)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ForwardingRuleK      | `putBuil              |                       |
        | eyHasher<HASH,​HASH2>` | dTargetSourcePath​(Bui |                       |
        |                       | ldTargetSourcePath bu |                       |
        |                       | ildTargetSourcePath)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ForwardingRuleK      | `pu                   |                       |
        | eyHasher<HASH,​HASH2>` | tBytes​(byte[] bytes)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ForwardingRuleK      | `pu                   |                       |
        | eyHasher<HASH,​HASH2>` | tCharacter​(char val)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ForwardingRuleK      | `putContai            | ::: block             |
        | eyHasher<HASH,​HASH2>` | ner​(RuleKeyHasher.Con | Puts the container    |
        |                       | tainer container,     | signature             |
        |                       |          int length)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ForwardingRuleK      | `putKey​(String key)`  | ::: block             |
        | eyHasher<HASH,​HASH2>` |                       | Puts the field\'s key |
        |                       |                       | (i.e.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RuleKeyHasher<HASH>` | `                     | ::: block             |
        |                       | putKeyPath​(Path key)` | Puts the stringified  |
        |                       |                       | path as a key.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ForwardingRuleK      | `putNonHa             |                       |
        | eyHasher<HASH,​HASH2>` | shingPath​(Path path)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ForwardingRuleK      | `putNull()`           | ::: block             |
        | eyHasher<HASH,​HASH2>` |                       | Puts the field\'s     |
        |                       |                       | value, Java types     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ForwardingRuleK      | `p                    |                       |
        | eyHasher<HASH,​HASH2>` | utNumber​(Number val)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ForwardingRuleK      | `p                    |                       |
        | eyHasher<HASH,​HASH2>` | utPath​(Path path,     |                       |
        |                       |     com.google.common |                       |
        |                       | .hash.HashCode hash)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ForwardingRuleK      | `putPatt              |                       |
        | eyHasher<HASH,​HASH2>` | ern​(Pattern pattern)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ForwardingRuleK      | `putRule              |                       |
        | eyHasher<HASH,​HASH2>` | Key​(RuleKey ruleKey)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ForwardingRuleK      | `putRuleTyp           |                       |
        | eyHasher<HASH,​HASH2>` | e​(RuleType ruleType)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ForwardingRuleK      | `putSha               | ::: block             |
        | eyHasher<HASH,​HASH2>` | 1​(Sha1HashCode sha1)` | Puts the field\'s     |
        |                       |                       | value, Buck specific  |
        |                       |                       | types                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ForwardingRuleK      | `p                    |                       |
        | eyHasher<HASH,​HASH2>` | utString​(String val)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ForwardingRuleK      | `                     |                       |
        | eyHasher<HASH,​HASH2>` | putWrapper​(RuleKeyHas |                       |
        |                       | her.Wrapper wrapper)` |                       |
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

        []{#<init>(com.facebook.buck.rules.keys.hasher.RuleKeyHasher,com.facebook.buck.rules.keys.hasher.RuleKeyHasher)}

        -   #### ForwardingRuleKeyHasher

                protected ForwardingRuleKeyHasher​(RuleKeyHasher<HASH> firstHasher,
                                                  RuleKeyHasher<HASH2> secondHasher)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#putKey(java.lang.String)}

        -   #### putKey

            ``` methodSignature
            public ForwardingRuleKeyHasher<HASH,​HASH2> putKey​(String key)
            ```

            ::: block
            [Description copied from
            interface: `RuleKeyHasher`]{.descfrmTypeLabel}
            :::

            ::: block
            Puts the field\'s key (i.e. the name of the field)
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `putKey` in interface `RuleKeyHasher<HASH>`

        []{#putKeyPath(java.nio.file.Path)}

        -   #### putKeyPath

            ``` methodSignature
            public RuleKeyHasher<HASH> putKeyPath​(Path key)
            ```

            ::: block
            [Description copied from
            interface: `RuleKeyHasher`]{.descfrmTypeLabel}
            :::

            ::: block
            Puts the stringified path as a key.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `putKeyPath` in interface `RuleKeyHasher<HASH>`

        []{#putNull()}

        -   #### putNull

            ``` methodSignature
            public ForwardingRuleKeyHasher<HASH,​HASH2> putNull()
            ```

            ::: block
            [Description copied from
            interface: `RuleKeyHasher`]{.descfrmTypeLabel}
            :::

            ::: block
            Puts the field\'s value, Java types
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `putNull` in interface `RuleKeyHasher<HASH>`

        []{#putCharacter(char)}

        -   #### putCharacter

            ``` methodSignature
            public ForwardingRuleKeyHasher<HASH,​HASH2> putCharacter​(char val)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putCharacter` in interface `RuleKeyHasher<HASH>`

        []{#putBoolean(boolean)}

        -   #### putBoolean

            ``` methodSignature
            public ForwardingRuleKeyHasher<HASH,​HASH2> putBoolean​(boolean val)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putBoolean` in interface `RuleKeyHasher<HASH>`

        []{#putNumber(java.lang.Number)}

        -   #### putNumber

            ``` methodSignature
            public ForwardingRuleKeyHasher<HASH,​HASH2> putNumber​(Number val)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putNumber` in interface `RuleKeyHasher<HASH>`

        []{#putString(java.lang.String)}

        -   #### putString

            ``` methodSignature
            public ForwardingRuleKeyHasher<HASH,​HASH2> putString​(String val)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putString` in interface `RuleKeyHasher<HASH>`

        []{#putBytes(byte[])}

        -   #### putBytes

            ``` methodSignature
            public ForwardingRuleKeyHasher<HASH,​HASH2> putBytes​(byte[] bytes)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putBytes` in interface `RuleKeyHasher<HASH>`

        []{#putPattern(java.util.regex.Pattern)}

        -   #### putPattern

            ``` methodSignature
            public ForwardingRuleKeyHasher<HASH,​HASH2> putPattern​(Pattern pattern)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putPattern` in interface `RuleKeyHasher<HASH>`

        []{#putSha1(com.facebook.buck.util.sha1.Sha1HashCode)}

        -   #### putSha1

            ``` methodSignature
            public ForwardingRuleKeyHasher<HASH,​HASH2> putSha1​(Sha1HashCode sha1)
            ```

            ::: block
            [Description copied from
            interface: `RuleKeyHasher`]{.descfrmTypeLabel}
            :::

            ::: block
            Puts the field\'s value, Buck specific types
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `putSha1` in interface `RuleKeyHasher<HASH>`

        []{#putPath(java.nio.file.Path,com.google.common.hash.HashCode)}

        -   #### putPath

            ``` methodSignature
            public ForwardingRuleKeyHasher<HASH,​HASH2> putPath​(Path path,
                                                                     com.google.common.hash.HashCode hash)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putPath` in interface `RuleKeyHasher<HASH>`

        []{#putArchiveMemberPath(java.nio.file.Path,java.nio.file.Path,com.google.common.hash.HashCode)}

        -   #### putArchiveMemberPath

            ``` methodSignature
            public ForwardingRuleKeyHasher<HASH,​HASH2> putArchiveMemberPath​(Path relativeArchivePath,
                                                                                  Path archiveMemberPath,
                                                                                  com.google.common.hash.HashCode hash)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putArchiveMemberPath` in
                interface `RuleKeyHasher<HASH>`

            [Parameters:]{.paramLabel}
            :   `relativeArchivePath` - relative path to archive.
            :   `archiveMemberPath` - path to archive member.

        []{#putNonHashingPath(java.nio.file.Path)}

        -   #### putNonHashingPath

            ``` methodSignature
            public ForwardingRuleKeyHasher<HASH,​HASH2> putNonHashingPath​(Path path)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putNonHashingPath` in interface `RuleKeyHasher<HASH>`

        []{#putRuleKey(com.facebook.buck.core.rulekey.RuleKey)}

        -   #### putRuleKey

            ``` methodSignature
            public ForwardingRuleKeyHasher<HASH,​HASH2> putRuleKey​(RuleKey ruleKey)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putRuleKey` in interface `RuleKeyHasher<HASH>`

        []{#putRuleType(com.facebook.buck.core.model.RuleType)}

        -   #### putRuleType

            ``` methodSignature
            public ForwardingRuleKeyHasher<HASH,​HASH2> putRuleType​(RuleType ruleType)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putRuleType` in interface `RuleKeyHasher<HASH>`

        []{#putBuildTarget(com.facebook.buck.core.model.BuildTarget)}

        -   #### putBuildTarget

            ``` methodSignature
            public ForwardingRuleKeyHasher<HASH,​HASH2> putBuildTarget​(BuildTarget buildTarget)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putBuildTarget` in interface `RuleKeyHasher<HASH>`

        []{#putBuildTargetSourcePath(com.facebook.buck.core.sourcepath.BuildTargetSourcePath)}

        -   #### putBuildTargetSourcePath

            ``` methodSignature
            public ForwardingRuleKeyHasher<HASH,​HASH2> putBuildTargetSourcePath​(BuildTargetSourcePath buildTargetSourcePath)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putBuildTargetSourcePath` in
                interface `RuleKeyHasher<HASH>`

        []{#putContainer(com.facebook.buck.rules.keys.hasher.RuleKeyHasher.Container,int)}

        -   #### putContainer

            ``` methodSignature
            public ForwardingRuleKeyHasher<HASH,​HASH2> putContainer​(RuleKeyHasher.Container container,
                                                                          int length)
            ```

            ::: block
            [Description copied from
            interface: `RuleKeyHasher`]{.descfrmTypeLabel}
            :::

            ::: block
            Puts the container signature
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `putContainer` in interface `RuleKeyHasher<HASH>`

        []{#putWrapper(com.facebook.buck.rules.keys.hasher.RuleKeyHasher.Wrapper)}

        -   #### putWrapper

            ``` methodSignature
            public ForwardingRuleKeyHasher<HASH,​HASH2> putWrapper​(RuleKeyHasher.Wrapper wrapper)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putWrapper` in interface `RuleKeyHasher<HASH>`

        []{#hash()}

        -   #### hash

            ``` methodSignature
            public HASH hash()
            ```

            ::: block
            [Description copied from
            interface: `RuleKeyHasher`]{.descfrmTypeLabel}
            :::

            ::: block
            Computes the final hash.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `hash` in interface `RuleKeyHasher<HASH>`

        []{#onHash(java.lang.Object,java.lang.Object)}
        []{#onHash(HASH,HASH2)}

        -   #### onHash

            ``` methodSignature
            protected abstract void onHash​(HASH firstHash,
                                           HASH2 secondHash)
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
-   [Nested](#nested.class.summary) \| 
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

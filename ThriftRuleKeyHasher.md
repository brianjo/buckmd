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

## Class ThriftRuleKeyHasher {#class-thriftrulekeyhasher .title title="Class ThriftRuleKeyHasher"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.keys.hasher.ThriftRuleKeyHasher

::: description
-   

    All Implemented Interfaces:
    :   `RuleKeyHasher<com.facebook.buck.log.thrift.rulekeys.FullRuleKey>`

    ------------------------------------------------------------------------

        public class ThriftRuleKeyHasher
        extends Object
        implements RuleKeyHasher<com.facebook.buck.log.thrift.rulekeys.FullRuleKey>

    ::: block
    A rule key hasher that attempts to create thrift structures
    representing rule keys as hashing occurs, and writes out the
    serialized data once the rule key is \"complete\"
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

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `ThriftRuleKeyHasher​(Th           | ::: block                         |
        | riftRuleKeyLogger ruleKeyLogger)` | Creates a                         |
        |                                   | [`ThriftRuleKeyHasher`](Thrift    |
        |                                   | RuleKeyHasher.html "class in com. |
        |                                   | facebook.buck.rules.keys.hasher") |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+

        : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `flushToLogger()`     | ::: block             |
        |                       |                       | Writes the object out |
        |                       |                       | to the logger         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.face             | `hash()`              | ::: block             |
        | book.buck.log.thrift. |                       | Finishes populating   |
        | rulekeys.FullRuleKey` |                       | the ruleKey with      |
        |                       |                       | remaining key/value   |
        |                       |                       | pairs and returns it  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Ru                   | `pu                   |                       |
        | leKeyHasher<com.faceb | tArchiveMemberPath​(Pa |                       |
        | ook.buck.log.thrift.r | th relativeArchivePat |                       |
        | ulekeys.FullRuleKey>` | h,                    |                       |
        |                       |   Path archiveMemberP |                       |
        |                       | ath,                  |                       |
        |                       |     com.google.common |                       |
        |                       | .hash.HashCode hash)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Ru                   | `put                  |                       |
        | leKeyHasher<com.faceb | Boolean​(boolean val)` |                       |
        | ook.buck.log.thrift.r |                       |                       |
        | ulekeys.FullRuleKey>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Ru                   | `putBuildTarget​(Buil  |                       |
        | leKeyHasher<com.faceb | dTarget buildTarget)` |                       |
        | ook.buck.log.thrift.r |                       |                       |
        | ulekeys.FullRuleKey>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Ru                   | `putBuil              |                       |
        | leKeyHasher<com.faceb | dTargetSourcePath​(Bui |                       |
        | ook.buck.log.thrift.r | ldTargetSourcePath bu |                       |
        | ulekeys.FullRuleKey>` | ildTargetSourcePath)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Ru                   | `pu                   |                       |
        | leKeyHasher<com.faceb | tBytes​(byte[] bytes)` |                       |
        | ook.buck.log.thrift.r |                       |                       |
        | ulekeys.FullRuleKey>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Ru                   | `pu                   |                       |
        | leKeyHasher<com.faceb | tCharacter​(char val)` |                       |
        | ook.buck.log.thrift.r |                       |                       |
        | ulekeys.FullRuleKey>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Ru                   | `putContai            | ::: block             |
        | leKeyHasher<com.faceb | ner​(RuleKeyHasher.Con | Adds a container to   |
        | ook.buck.log.thrift.r | tainer container,     | the stack.            |
        | ulekeys.FullRuleKey>` |          int length)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Ru                   | `putKey​(String key)`  | ::: block             |
        | leKeyHasher<com.faceb |                       | Puts the field\'s key |
        | ook.buck.log.thrift.r |                       | (i.e.                 |
        | ulekeys.FullRuleKey>` |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Ru                   | `                     | ::: block             |
        | leKeyHasher<com.faceb | putKeyPath​(Path key)` | Puts the stringified  |
        | ook.buck.log.thrift.r |                       | path as a key.        |
        | ulekeys.FullRuleKey>` |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Ru                   | `putNonHa             |                       |
        | leKeyHasher<com.faceb | shingPath​(Path path)` |                       |
        | ook.buck.log.thrift.r |                       |                       |
        | ulekeys.FullRuleKey>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Ru                   | `putNull()`           | ::: block             |
        | leKeyHasher<com.faceb |                       | Puts the field\'s     |
        | ook.buck.log.thrift.r |                       | value, Java types     |
        | ulekeys.FullRuleKey>` |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Ru                   | `p                    |                       |
        | leKeyHasher<com.faceb | utNumber​(Number val)` |                       |
        | ook.buck.log.thrift.r |                       |                       |
        | ulekeys.FullRuleKey>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Ru                   | `p                    |                       |
        | leKeyHasher<com.faceb | utPath​(Path path,     |                       |
        | ook.buck.log.thrift.r |     com.google.common |                       |
        | ulekeys.FullRuleKey>` | .hash.HashCode hash)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Ru                   | `putPatt              |                       |
        | leKeyHasher<com.faceb | ern​(Pattern pattern)` |                       |
        | ook.buck.log.thrift.r |                       |                       |
        | ulekeys.FullRuleKey>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Ru                   | `putRule              |                       |
        | leKeyHasher<com.faceb | Key​(RuleKey ruleKey)` |                       |
        | ook.buck.log.thrift.r |                       |                       |
        | ulekeys.FullRuleKey>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Ru                   | `putRuleTyp           |                       |
        | leKeyHasher<com.faceb | e​(RuleType ruleType)` |                       |
        | ook.buck.log.thrift.r |                       |                       |
        | ulekeys.FullRuleKey>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Ru                   | `putSha               | ::: block             |
        | leKeyHasher<com.faceb | 1​(Sha1HashCode sha1)` | Puts the field\'s     |
        | ook.buck.log.thrift.r |                       | value, Buck specific  |
        | ulekeys.FullRuleKey>` |                       | types                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Ru                   | `p                    |                       |
        | leKeyHasher<com.faceb | utString​(String val)` |                       |
        | ook.buck.log.thrift.r |                       |                       |
        | ulekeys.FullRuleKey>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Ru                   | `                     |                       |
        | leKeyHasher<com.faceb | putWrapper​(RuleKeyHas |                       |
        | ook.buck.log.thrift.r | her.Wrapper wrapper)` |                       |
        | ulekeys.FullRuleKey>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `setHash              | ::: block             |
        |                       | Key​(com.google.common | Sets the hash key on  |
        |                       | .hash.HashCode code)` | the ruleKey object    |
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

        []{#<init>(com.facebook.buck.log.thrift.ThriftRuleKeyLogger)}

        -   #### ThriftRuleKeyHasher

                public ThriftRuleKeyHasher​(ThriftRuleKeyLogger ruleKeyLogger)

            ::: block
            Creates a
            [`ThriftRuleKeyHasher`](ThriftRuleKeyHasher.html "class in com.facebook.buck.rules.keys.hasher")
            :::

            [Parameters:]{.paramLabel}
            :   `ruleKeyLogger` - The ruleKeyLogger used to write
                serialized thrift structures out
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#putKey(java.lang.String)}

        -   #### putKey

            ``` methodSignature
            public RuleKeyHasher<com.facebook.buck.log.thrift.rulekeys.FullRuleKey> putKey​(String key)
            ```

            ::: block
            [Description copied from
            interface: `RuleKeyHasher`]{.descfrmTypeLabel}
            :::

            ::: block
            Puts the field\'s key (i.e. the name of the field)
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `putKey` in
                interface `RuleKeyHasher<com.facebook.buck.log.thrift.rulekeys.FullRuleKey>`

        []{#putKeyPath(java.nio.file.Path)}

        -   #### putKeyPath

            ``` methodSignature
            public RuleKeyHasher<com.facebook.buck.log.thrift.rulekeys.FullRuleKey> putKeyPath​(Path key)
            ```

            ::: block
            [Description copied from
            interface: `RuleKeyHasher`]{.descfrmTypeLabel}
            :::

            ::: block
            Puts the stringified path as a key.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `putKeyPath` in
                interface `RuleKeyHasher<com.facebook.buck.log.thrift.rulekeys.FullRuleKey>`

        []{#putNull()}

        -   #### putNull

            ``` methodSignature
            public RuleKeyHasher<com.facebook.buck.log.thrift.rulekeys.FullRuleKey> putNull()
            ```

            ::: block
            [Description copied from
            interface: `RuleKeyHasher`]{.descfrmTypeLabel}
            :::

            ::: block
            Puts the field\'s value, Java types
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `putNull` in
                interface `RuleKeyHasher<com.facebook.buck.log.thrift.rulekeys.FullRuleKey>`

        []{#putCharacter(char)}

        -   #### putCharacter

            ``` methodSignature
            public RuleKeyHasher<com.facebook.buck.log.thrift.rulekeys.FullRuleKey> putCharacter​(char val)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putCharacter` in
                interface `RuleKeyHasher<com.facebook.buck.log.thrift.rulekeys.FullRuleKey>`

        []{#putBoolean(boolean)}

        -   #### putBoolean

            ``` methodSignature
            public RuleKeyHasher<com.facebook.buck.log.thrift.rulekeys.FullRuleKey> putBoolean​(boolean val)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putBoolean` in
                interface `RuleKeyHasher<com.facebook.buck.log.thrift.rulekeys.FullRuleKey>`

        []{#putNumber(java.lang.Number)}

        -   #### putNumber

            ``` methodSignature
            public RuleKeyHasher<com.facebook.buck.log.thrift.rulekeys.FullRuleKey> putNumber​(Number val)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putNumber` in
                interface `RuleKeyHasher<com.facebook.buck.log.thrift.rulekeys.FullRuleKey>`

        []{#putString(java.lang.String)}

        -   #### putString

            ``` methodSignature
            public RuleKeyHasher<com.facebook.buck.log.thrift.rulekeys.FullRuleKey> putString​(String val)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putString` in
                interface `RuleKeyHasher<com.facebook.buck.log.thrift.rulekeys.FullRuleKey>`

        []{#putBytes(byte[])}

        -   #### putBytes

            ``` methodSignature
            public RuleKeyHasher<com.facebook.buck.log.thrift.rulekeys.FullRuleKey> putBytes​(byte[] bytes)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putBytes` in
                interface `RuleKeyHasher<com.facebook.buck.log.thrift.rulekeys.FullRuleKey>`

        []{#putPattern(java.util.regex.Pattern)}

        -   #### putPattern

            ``` methodSignature
            public RuleKeyHasher<com.facebook.buck.log.thrift.rulekeys.FullRuleKey> putPattern​(Pattern pattern)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putPattern` in
                interface `RuleKeyHasher<com.facebook.buck.log.thrift.rulekeys.FullRuleKey>`

        []{#putSha1(com.facebook.buck.util.sha1.Sha1HashCode)}

        -   #### putSha1

            ``` methodSignature
            public RuleKeyHasher<com.facebook.buck.log.thrift.rulekeys.FullRuleKey> putSha1​(Sha1HashCode sha1)
            ```

            ::: block
            [Description copied from
            interface: `RuleKeyHasher`]{.descfrmTypeLabel}
            :::

            ::: block
            Puts the field\'s value, Buck specific types
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `putSha1` in
                interface `RuleKeyHasher<com.facebook.buck.log.thrift.rulekeys.FullRuleKey>`

        []{#putPath(java.nio.file.Path,com.google.common.hash.HashCode)}

        -   #### putPath

            ``` methodSignature
            public RuleKeyHasher<com.facebook.buck.log.thrift.rulekeys.FullRuleKey> putPath​(Path path,
                                                                                            com.google.common.hash.HashCode hash)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putPath` in
                interface `RuleKeyHasher<com.facebook.buck.log.thrift.rulekeys.FullRuleKey>`

        []{#putArchiveMemberPath(java.nio.file.Path,java.nio.file.Path,com.google.common.hash.HashCode)}

        -   #### putArchiveMemberPath

            ``` methodSignature
            public RuleKeyHasher<com.facebook.buck.log.thrift.rulekeys.FullRuleKey> putArchiveMemberPath​(Path relativeArchivePath,
                                                                                                         Path archiveMemberPath,
                                                                                                         com.google.common.hash.HashCode hash)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putArchiveMemberPath` in
                interface `RuleKeyHasher<com.facebook.buck.log.thrift.rulekeys.FullRuleKey>`

            [Parameters:]{.paramLabel}
            :   `relativeArchivePath` - relative path to archive.
            :   `archiveMemberPath` - path to archive member.

        []{#putNonHashingPath(java.nio.file.Path)}

        -   #### putNonHashingPath

            ``` methodSignature
            public RuleKeyHasher<com.facebook.buck.log.thrift.rulekeys.FullRuleKey> putNonHashingPath​(Path path)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putNonHashingPath` in
                interface `RuleKeyHasher<com.facebook.buck.log.thrift.rulekeys.FullRuleKey>`

        []{#putRuleKey(com.facebook.buck.core.rulekey.RuleKey)}

        -   #### putRuleKey

            ``` methodSignature
            public RuleKeyHasher<com.facebook.buck.log.thrift.rulekeys.FullRuleKey> putRuleKey​(RuleKey ruleKey)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putRuleKey` in
                interface `RuleKeyHasher<com.facebook.buck.log.thrift.rulekeys.FullRuleKey>`

        []{#putRuleType(com.facebook.buck.core.model.RuleType)}

        -   #### putRuleType

            ``` methodSignature
            public RuleKeyHasher<com.facebook.buck.log.thrift.rulekeys.FullRuleKey> putRuleType​(RuleType ruleType)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putRuleType` in
                interface `RuleKeyHasher<com.facebook.buck.log.thrift.rulekeys.FullRuleKey>`

        []{#putBuildTarget(com.facebook.buck.core.model.BuildTarget)}

        -   #### putBuildTarget

            ``` methodSignature
            public RuleKeyHasher<com.facebook.buck.log.thrift.rulekeys.FullRuleKey> putBuildTarget​(BuildTarget buildTarget)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putBuildTarget` in
                interface `RuleKeyHasher<com.facebook.buck.log.thrift.rulekeys.FullRuleKey>`

        []{#putBuildTargetSourcePath(com.facebook.buck.core.sourcepath.BuildTargetSourcePath)}

        -   #### putBuildTargetSourcePath

            ``` methodSignature
            public RuleKeyHasher<com.facebook.buck.log.thrift.rulekeys.FullRuleKey> putBuildTargetSourcePath​(BuildTargetSourcePath buildTargetSourcePath)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putBuildTargetSourcePath` in
                interface `RuleKeyHasher<com.facebook.buck.log.thrift.rulekeys.FullRuleKey>`

        []{#putContainer(com.facebook.buck.rules.keys.hasher.RuleKeyHasher.Container,int)}

        -   #### putContainer

            ``` methodSignature
            public RuleKeyHasher<com.facebook.buck.log.thrift.rulekeys.FullRuleKey> putContainer​(RuleKeyHasher.Container container,
                                                                                                 int length)
            ```

            ::: block
            Adds a container to the stack. This will pop down the stack
            of already hashed values in order to populate the container.
            The container Value is then put back on the stack
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `putContainer` in
                interface `RuleKeyHasher<com.facebook.buck.log.thrift.rulekeys.FullRuleKey>`

            [Parameters:]{.paramLabel}
            :   `container` - The container type
            :   `length` - The number of elements in the container. This
                can vary slightly by container type

            [Returns:]{.returnLabel}
            :   The original RuleKeyHasher object

        []{#putWrapper(com.facebook.buck.rules.keys.hasher.RuleKeyHasher.Wrapper)}

        -   #### putWrapper

            ``` methodSignature
            public RuleKeyHasher<com.facebook.buck.log.thrift.rulekeys.FullRuleKey> putWrapper​(RuleKeyHasher.Wrapper wrapper)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putWrapper` in
                interface `RuleKeyHasher<com.facebook.buck.log.thrift.rulekeys.FullRuleKey>`

        []{#hash()}

        -   #### hash

            ``` methodSignature
            public com.facebook.buck.log.thrift.rulekeys.FullRuleKey hash()
            ```

            ::: block
            Finishes populating the ruleKey with remaining key/value
            pairs and returns it
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `hash` in
                interface `RuleKeyHasher<com.facebook.buck.log.thrift.rulekeys.FullRuleKey>`

            [Returns:]{.returnLabel}
            :   The fully populated ruleKey

        []{#setHashKey(com.google.common.hash.HashCode)}

        -   #### setHashKey

            ``` methodSignature
            public void setHashKey​(com.google.common.hash.HashCode code)
            ```

            ::: block
            Sets the hash key on the ruleKey object
            :::

            [Parameters:]{.paramLabel}
            :   `code` - The hash code to use

        []{#flushToLogger()}

        -   #### flushToLogger

            ``` methodSignature
            public void flushToLogger()
            ```

            ::: block
            Writes the object out to the logger
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

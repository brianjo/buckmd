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

## Class GuavaRuleKeyHasher {#class-guavarulekeyhasher .title title="Class GuavaRuleKeyHasher"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.keys.hasher.GuavaRuleKeyHasher

::: description
-   

    All Implemented Interfaces:
    :   `RuleKeyHasher<com.google.common.hash.HashCode>`

    ------------------------------------------------------------------------

        public class GuavaRuleKeyHasher
        extends Object
        implements RuleKeyHasher<com.google.common.hash.HashCode>

    ::: block
    An implementation of
    [`RuleKeyHasher`](RuleKeyHasher.html "interface in com.facebook.buck.rules.keys.hasher")
    that wraps Guava\'s `Hasher`.
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

          Constructor                                                  Description
          ------------------------------------------------------------ -------------
          `GuavaRuleKeyHasher​(com.google.common.hash.Hasher hasher)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.google.          | `hash()`              | ::: block             |
        | common.hash.HashCode` |                       | Computes the final    |
        |                       |                       | hash.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GuavaRuleKeyHasher`  | `pu                   |                       |
        |                       | tArchiveMemberPath​(Pa |                       |
        |                       | th relativeArchivePat |                       |
        |                       | h,                    |                       |
        |                       |   Path archiveMemberP |                       |
        |                       | ath,                  |                       |
        |                       |     com.google.common |                       |
        |                       | .hash.HashCode hash)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `GuavaRuleKeyHasher`  | `put                  |                       |
        |                       | Boolean​(boolean val)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `GuavaRuleKeyHasher`  | `putBuildTarget​(Buil  |                       |
        |                       | dTarget buildTarget)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `RuleK                | `pu                   |                       |
        | eyHasher<com.google.c | tBuildTargetSourcePat |                       |
        | ommon.hash.HashCode>` | h​(BuildTargetSourcePa |                       |
        |                       | th targetSourcePath)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `GuavaRuleKeyHasher`  | `pu                   |                       |
        |                       | tBytes​(byte[] bytes)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `GuavaRuleKeyHasher`  | `pu                   |                       |
        |                       | tCharacter​(char val)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `GuavaRuleKeyHasher`  | `putContai            | ::: block             |
        |                       | ner​(RuleKeyHasher.Con | Puts the container    |
        |                       | tainer container,     | signature             |
        |                       |          int length)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GuavaRuleKeyHasher`  | `putKey​(String key)`  | ::: block             |
        |                       |                       | Puts the field\'s key |
        |                       |                       | (i.e.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RuleK                | `                     | ::: block             |
        | eyHasher<com.google.c | putKeyPath​(Path key)` | Puts the stringified  |
        | ommon.hash.HashCode>` |                       | path as a key.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GuavaRuleKeyHasher`  | `putNonHa             |                       |
        |                       | shingPath​(Path path)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `GuavaRuleKeyHasher`  | `putNull()`           | ::: block             |
        |                       |                       | Puts the field\'s     |
        |                       |                       | value, Java types     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GuavaRuleKeyHasher`  | `p                    |                       |
        |                       | utNumber​(Number val)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `GuavaRuleKeyHasher`  | `p                    |                       |
        |                       | utPath​(Path path,     |                       |
        |                       |     com.google.common |                       |
        |                       | .hash.HashCode hash)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `GuavaRuleKeyHasher`  | `putPatt              |                       |
        |                       | ern​(Pattern pattern)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `GuavaRuleKeyHasher`  | `putRule              |                       |
        |                       | Key​(RuleKey ruleKey)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `GuavaRuleKeyHasher`  | `putRuleTyp           |                       |
        |                       | e​(RuleType ruleType)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `GuavaRuleKeyHasher`  | `putSha               | ::: block             |
        |                       | 1​(Sha1HashCode sha1)` | Puts the field\'s     |
        |                       |                       | value, Buck specific  |
        |                       |                       | types                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GuavaRuleKeyHasher`  | `p                    |                       |
        |                       | utString​(String val)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `GuavaRuleKeyHasher`  | `                     |                       |
        |                       | putWrapper​(RuleKeyHas |                       |
        |                       | her.Wrapper wrapper)` |                       |
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

        []{#<init>(com.google.common.hash.Hasher)}

        -   #### GuavaRuleKeyHasher

                public GuavaRuleKeyHasher​(com.google.common.hash.Hasher hasher)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#putKey(java.lang.String)}

        -   #### putKey

            ``` methodSignature
            public GuavaRuleKeyHasher putKey​(String key)
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
                interface `RuleKeyHasher<com.google.common.hash.HashCode>`

        []{#putKeyPath(java.nio.file.Path)}

        -   #### putKeyPath

            ``` methodSignature
            public RuleKeyHasher<com.google.common.hash.HashCode> putKeyPath​(Path key)
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
                interface `RuleKeyHasher<com.google.common.hash.HashCode>`

        []{#putNull()}

        -   #### putNull

            ``` methodSignature
            public GuavaRuleKeyHasher putNull()
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
                interface `RuleKeyHasher<com.google.common.hash.HashCode>`

        []{#putCharacter(char)}

        -   #### putCharacter

            ``` methodSignature
            public GuavaRuleKeyHasher putCharacter​(char val)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putCharacter` in
                interface `RuleKeyHasher<com.google.common.hash.HashCode>`

        []{#putBoolean(boolean)}

        -   #### putBoolean

            ``` methodSignature
            public GuavaRuleKeyHasher putBoolean​(boolean val)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putBoolean` in
                interface `RuleKeyHasher<com.google.common.hash.HashCode>`

        []{#putNumber(java.lang.Number)}

        -   #### putNumber

            ``` methodSignature
            public GuavaRuleKeyHasher putNumber​(Number val)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putNumber` in
                interface `RuleKeyHasher<com.google.common.hash.HashCode>`

        []{#putString(java.lang.String)}

        -   #### putString

            ``` methodSignature
            public GuavaRuleKeyHasher putString​(String val)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putString` in
                interface `RuleKeyHasher<com.google.common.hash.HashCode>`

        []{#putBytes(byte[])}

        -   #### putBytes

            ``` methodSignature
            public GuavaRuleKeyHasher putBytes​(byte[] bytes)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putBytes` in
                interface `RuleKeyHasher<com.google.common.hash.HashCode>`

        []{#putPattern(java.util.regex.Pattern)}

        -   #### putPattern

            ``` methodSignature
            public GuavaRuleKeyHasher putPattern​(Pattern pattern)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putPattern` in
                interface `RuleKeyHasher<com.google.common.hash.HashCode>`

        []{#putSha1(com.facebook.buck.util.sha1.Sha1HashCode)}

        -   #### putSha1

            ``` methodSignature
            public GuavaRuleKeyHasher putSha1​(Sha1HashCode sha1)
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
                interface `RuleKeyHasher<com.google.common.hash.HashCode>`

        []{#putPath(java.nio.file.Path,com.google.common.hash.HashCode)}

        -   #### putPath

            ``` methodSignature
            public GuavaRuleKeyHasher putPath​(Path path,
                                              com.google.common.hash.HashCode hash)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putPath` in
                interface `RuleKeyHasher<com.google.common.hash.HashCode>`

        []{#putArchiveMemberPath(java.nio.file.Path,java.nio.file.Path,com.google.common.hash.HashCode)}

        -   #### putArchiveMemberPath

            ``` methodSignature
            public GuavaRuleKeyHasher putArchiveMemberPath​(Path relativeArchivePath,
                                                           Path archiveMemberPath,
                                                           com.google.common.hash.HashCode hash)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putArchiveMemberPath` in
                interface `RuleKeyHasher<com.google.common.hash.HashCode>`

            [Parameters:]{.paramLabel}
            :   `relativeArchivePath` - relative path to archive.
            :   `archiveMemberPath` - path to archive member.

        []{#putNonHashingPath(java.nio.file.Path)}

        -   #### putNonHashingPath

            ``` methodSignature
            public GuavaRuleKeyHasher putNonHashingPath​(Path path)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putNonHashingPath` in
                interface `RuleKeyHasher<com.google.common.hash.HashCode>`

        []{#putRuleKey(com.facebook.buck.core.rulekey.RuleKey)}

        -   #### putRuleKey

            ``` methodSignature
            public GuavaRuleKeyHasher putRuleKey​(RuleKey ruleKey)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putRuleKey` in
                interface `RuleKeyHasher<com.google.common.hash.HashCode>`

        []{#putRuleType(com.facebook.buck.core.model.RuleType)}

        -   #### putRuleType

            ``` methodSignature
            public GuavaRuleKeyHasher putRuleType​(RuleType ruleType)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putRuleType` in
                interface `RuleKeyHasher<com.google.common.hash.HashCode>`

        []{#putBuildTarget(com.facebook.buck.core.model.BuildTarget)}

        -   #### putBuildTarget

            ``` methodSignature
            public GuavaRuleKeyHasher putBuildTarget​(BuildTarget buildTarget)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putBuildTarget` in
                interface `RuleKeyHasher<com.google.common.hash.HashCode>`

        []{#putBuildTargetSourcePath(com.facebook.buck.core.sourcepath.BuildTargetSourcePath)}

        -   #### putBuildTargetSourcePath

            ``` methodSignature
            public RuleKeyHasher<com.google.common.hash.HashCode> putBuildTargetSourcePath​(BuildTargetSourcePath targetSourcePath)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putBuildTargetSourcePath` in
                interface `RuleKeyHasher<com.google.common.hash.HashCode>`

        []{#putContainer(com.facebook.buck.rules.keys.hasher.RuleKeyHasher.Container,int)}

        -   #### putContainer

            ``` methodSignature
            public GuavaRuleKeyHasher putContainer​(RuleKeyHasher.Container container,
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
            :   `putContainer` in
                interface `RuleKeyHasher<com.google.common.hash.HashCode>`

        []{#putWrapper(com.facebook.buck.rules.keys.hasher.RuleKeyHasher.Wrapper)}

        -   #### putWrapper

            ``` methodSignature
            public GuavaRuleKeyHasher putWrapper​(RuleKeyHasher.Wrapper wrapper)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putWrapper` in
                interface `RuleKeyHasher<com.google.common.hash.HashCode>`

        []{#hash()}

        -   #### hash

            ``` methodSignature
            public com.google.common.hash.HashCode hash()
            ```

            ::: block
            [Description copied from
            interface: `RuleKeyHasher`]{.descfrmTypeLabel}
            :::

            ::: block
            Computes the final hash.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `hash` in
                interface `RuleKeyHasher<com.google.common.hash.HashCode>`
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

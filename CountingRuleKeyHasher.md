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

## Class CountingRuleKeyHasher\<HASH\> {#class-countingrulekeyhasherhash .title title="Class CountingRuleKeyHasher"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.keys.hasher.CountingRuleKeyHasher\<HASH\>

::: description
-   

    All Implemented Interfaces:
    :   `RuleKeyHasher<HASH>`

    ------------------------------------------------------------------------

        public class CountingRuleKeyHasher<HASH>
        extends Object
        implements RuleKeyHasher<HASH>

    ::: block
    A delegating
    [`RuleKeyHasher`](RuleKeyHasher.html "interface in com.facebook.buck.rules.keys.hasher")
    that counts the number of values put in it.
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

          Constructor                                             Description
          ------------------------------------------------------- -------------
          `CountingRuleKeyHasher​(RuleKeyHasher<HASH> delegate)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `long`                | `getCount()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `HASH`                | `hash()`              | ::: block             |
        |                       |                       | Computes the final    |
        |                       |                       | hash.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Countin              | `pu                   |                       |
        | gRuleKeyHasher<HASH>` | tArchiveMemberPath​(Pa |                       |
        |                       | th relativeArchivePat |                       |
        |                       | h,                    |                       |
        |                       |   Path archiveMemberP |                       |
        |                       | ath,                  |                       |
        |                       |     com.google.common |                       |
        |                       | .hash.HashCode hash)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Countin              | `put                  |                       |
        | gRuleKeyHasher<HASH>` | Boolean​(boolean val)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Countin              | `putBuildTarget​(Buil  |                       |
        | gRuleKeyHasher<HASH>` | dTarget buildTarget)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Countin              | `putBuil              |                       |
        | gRuleKeyHasher<HASH>` | dTargetSourcePath​(Bui |                       |
        |                       | ldTargetSourcePath bu |                       |
        |                       | ildTargetSourcePath)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Countin              | `pu                   |                       |
        | gRuleKeyHasher<HASH>` | tBytes​(byte[] bytes)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Countin              | `pu                   |                       |
        | gRuleKeyHasher<HASH>` | tCharacter​(char val)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Countin              | `putContai            | ::: block             |
        | gRuleKeyHasher<HASH>` | ner​(RuleKeyHasher.Con | Puts the container    |
        |                       | tainer container,     | signature             |
        |                       |          int length)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Countin              | `putKey​(String key)`  | ::: block             |
        | gRuleKeyHasher<HASH>` |                       | Puts the field\'s key |
        |                       |                       | (i.e.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Countin              | `                     | ::: block             |
        | gRuleKeyHasher<HASH>` | putKeyPath​(Path key)` | Puts the stringified  |
        |                       |                       | path as a key.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Countin              | `putNonHa             |                       |
        | gRuleKeyHasher<HASH>` | shingPath​(Path path)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Countin              | `putNull()`           | ::: block             |
        | gRuleKeyHasher<HASH>` |                       | Puts the field\'s     |
        |                       |                       | value, Java types     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Countin              | `p                    |                       |
        | gRuleKeyHasher<HASH>` | utNumber​(Number val)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Countin              | `p                    |                       |
        | gRuleKeyHasher<HASH>` | utPath​(Path path,     |                       |
        |                       |     com.google.common |                       |
        |                       | .hash.HashCode hash)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Countin              | `putPatt              |                       |
        | gRuleKeyHasher<HASH>` | ern​(Pattern pattern)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Countin              | `putRule              |                       |
        | gRuleKeyHasher<HASH>` | Key​(RuleKey ruleKey)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Countin              | `putRuleTyp           |                       |
        | gRuleKeyHasher<HASH>` | e​(RuleType ruleType)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Countin              | `putSha               | ::: block             |
        | gRuleKeyHasher<HASH>` | 1​(Sha1HashCode sha1)` | Puts the field\'s     |
        |                       |                       | value, Buck specific  |
        |                       |                       | types                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Countin              | `p                    |                       |
        | gRuleKeyHasher<HASH>` | utString​(String val)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Countin              | `                     |                       |
        | gRuleKeyHasher<HASH>` | putWrapper​(RuleKeyHas |                       |
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

        []{#<init>(com.facebook.buck.rules.keys.hasher.RuleKeyHasher)}

        -   #### CountingRuleKeyHasher

                public CountingRuleKeyHasher​(RuleKeyHasher<HASH> delegate)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getCount()}

        -   #### getCount

            ``` methodSignature
            public long getCount()
            ```

        []{#putKey(java.lang.String)}

        -   #### putKey

            ``` methodSignature
            public CountingRuleKeyHasher<HASH> putKey​(String key)
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
            public CountingRuleKeyHasher<HASH> putKeyPath​(Path key)
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
            public CountingRuleKeyHasher<HASH> putNull()
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
            public CountingRuleKeyHasher<HASH> putCharacter​(char val)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putCharacter` in interface `RuleKeyHasher<HASH>`

        []{#putBoolean(boolean)}

        -   #### putBoolean

            ``` methodSignature
            public CountingRuleKeyHasher<HASH> putBoolean​(boolean val)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putBoolean` in interface `RuleKeyHasher<HASH>`

        []{#putNumber(java.lang.Number)}

        -   #### putNumber

            ``` methodSignature
            public CountingRuleKeyHasher<HASH> putNumber​(Number val)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putNumber` in interface `RuleKeyHasher<HASH>`

        []{#putString(java.lang.String)}

        -   #### putString

            ``` methodSignature
            public CountingRuleKeyHasher<HASH> putString​(String val)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putString` in interface `RuleKeyHasher<HASH>`

        []{#putBytes(byte[])}

        -   #### putBytes

            ``` methodSignature
            public CountingRuleKeyHasher<HASH> putBytes​(byte[] bytes)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putBytes` in interface `RuleKeyHasher<HASH>`

        []{#putPattern(java.util.regex.Pattern)}

        -   #### putPattern

            ``` methodSignature
            public CountingRuleKeyHasher<HASH> putPattern​(Pattern pattern)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putPattern` in interface `RuleKeyHasher<HASH>`

        []{#putSha1(com.facebook.buck.util.sha1.Sha1HashCode)}

        -   #### putSha1

            ``` methodSignature
            public CountingRuleKeyHasher<HASH> putSha1​(Sha1HashCode sha1)
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
            public CountingRuleKeyHasher<HASH> putPath​(Path path,
                                                       com.google.common.hash.HashCode hash)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putPath` in interface `RuleKeyHasher<HASH>`

        []{#putArchiveMemberPath(java.nio.file.Path,java.nio.file.Path,com.google.common.hash.HashCode)}

        -   #### putArchiveMemberPath

            ``` methodSignature
            public CountingRuleKeyHasher<HASH> putArchiveMemberPath​(Path relativeArchivePath,
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
            public CountingRuleKeyHasher<HASH> putNonHashingPath​(Path path)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putNonHashingPath` in interface `RuleKeyHasher<HASH>`

        []{#putRuleKey(com.facebook.buck.core.rulekey.RuleKey)}

        -   #### putRuleKey

            ``` methodSignature
            public CountingRuleKeyHasher<HASH> putRuleKey​(RuleKey ruleKey)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putRuleKey` in interface `RuleKeyHasher<HASH>`

        []{#putRuleType(com.facebook.buck.core.model.RuleType)}

        -   #### putRuleType

            ``` methodSignature
            public CountingRuleKeyHasher<HASH> putRuleType​(RuleType ruleType)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putRuleType` in interface `RuleKeyHasher<HASH>`

        []{#putBuildTarget(com.facebook.buck.core.model.BuildTarget)}

        -   #### putBuildTarget

            ``` methodSignature
            public CountingRuleKeyHasher<HASH> putBuildTarget​(BuildTarget buildTarget)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putBuildTarget` in interface `RuleKeyHasher<HASH>`

        []{#putBuildTargetSourcePath(com.facebook.buck.core.sourcepath.BuildTargetSourcePath)}

        -   #### putBuildTargetSourcePath

            ``` methodSignature
            public CountingRuleKeyHasher<HASH> putBuildTargetSourcePath​(BuildTargetSourcePath buildTargetSourcePath)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putBuildTargetSourcePath` in
                interface `RuleKeyHasher<HASH>`

        []{#putContainer(com.facebook.buck.rules.keys.hasher.RuleKeyHasher.Container,int)}

        -   #### putContainer

            ``` methodSignature
            public CountingRuleKeyHasher<HASH> putContainer​(RuleKeyHasher.Container container,
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
            public CountingRuleKeyHasher<HASH> putWrapper​(RuleKeyHasher.Wrapper wrapper)
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

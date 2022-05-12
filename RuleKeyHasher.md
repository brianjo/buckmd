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
[Package]{.packageLabelInType} [com.facebook.buck.rules.keys.hasher](package-summary.html)
:::

## Interface RuleKeyHasher\<HASH\> {#interface-rulekeyhasherhash .title title="Interface RuleKeyHasher"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `CountingRuleKeyHasher`, `ForwardingRuleKeyHasher`,
        `GuavaRuleKeyHasher`, `StringRuleKeyHasher`,
        `ThriftRuleKeyHasher`

    ------------------------------------------------------------------------

        public interface RuleKeyHasher<HASH>

    ::: block
    A hasher used for the rule key construction.
    **Warning:** The result of calling any methods after calling
    [`hash()`](#hash()) is undefined.

    Chunks of data that are put into the
    [`RuleKeyHasher`](RuleKeyHasher.html "interface in com.facebook.buck.rules.keys.hasher")
    are delimited. Delimiting details are implementation dependent, but
    one common way is to hash the size of the data along with the data
    itself, for each operation performed. For example, the following
    three expressions should ideally all generate different hash codes:

         newHasher().putByte(b1).putByte(b2).putByte(b3).hash()
         newHasher().putByte(b1).putBytes(new byte[] { b2, b3 }).hash()
         newHasher().putBytes(new byte[] { b1, b2, b3 }).hash()
         

    Note, Buck hashes both field values and field names (keys) when
    constructing rule keys. E.g.:
        {@code
         public class myRule implements BuildRule {












        Nested Class Summary

        Nested Classes 

        Modifier and Type
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
    | `RuleKeyHasher<HASH>` | `pu                   |                       |
    |                       | tArchiveMemberPath​(Pa |                       |
    |                       | th relativeArchivePat |                       |
    |                       | h,                    |                       |
    |                       |   Path archiveMemberP |                       |
    |                       | ath,                  |                       |
    |                       |     com.google.common |                       |
    |                       | .hash.HashCode hash)` |                       |
    +-----------------------+-----------------------+-----------------------+
    | `RuleKeyHasher<HASH>` | `put                  |                       |
    |                       | Boolean​(boolean val)` |                       |
    +-----------------------+-----------------------+-----------------------+
    | `RuleKeyHasher<HASH>` | `putBuildTarget​(Buil  |                       |
    |                       | dTarget buildTarget)` |                       |
    +-----------------------+-----------------------+-----------------------+
    | `RuleKeyHasher<HASH>` | `putBuil              |                       |
    |                       | dTargetSourcePath​(Bui |                       |
    |                       | ldTargetSourcePath bu |                       |
    |                       | ildTargetSourcePath)` |                       |
    +-----------------------+-----------------------+-----------------------+
    | `RuleKeyHasher<HASH>` | `pu                   |                       |
    |                       | tBytes​(byte[] bytes)` |                       |
    +-----------------------+-----------------------+-----------------------+
    | `RuleKeyHasher<HASH>` | `pu                   |                       |
    |                       | tCharacter​(char val)` |                       |
    +-----------------------+-----------------------+-----------------------+
    | `RuleKeyHasher<HASH>` | `putContai            | ::: block             |
    |                       | ner​(RuleKeyHasher.Con | Puts the container    |
    |                       | tainer container,     | signature             |
    |                       |          int length)` | :::                   |
    +-----------------------+-----------------------+-----------------------+
    | `RuleKeyHasher<HASH>` | `putKey​(String key)`  | ::: block             |
    |                       |                       | Puts the field\'s key |
    |                       |                       | (i.e.                 |
    |                       |                       | :::                   |
    +-----------------------+-----------------------+-----------------------+
    | `RuleKeyHasher<HASH>` | `                     | ::: block             |
    |                       | putKeyPath​(Path key)` | Puts the stringified  |
    |                       |                       | path as a key.        |
    |                       |                       | :::                   |
    +-----------------------+-----------------------+-----------------------+
    | `RuleKeyHasher<HASH>` | `putNonHa             |                       |
    |                       | shingPath​(Path path)` |                       |
    +-----------------------+-----------------------+-----------------------+
    | `RuleKeyHasher<HASH>` | `putNull()`           | ::: block             |
    |                       |                       | Puts the field\'s     |
    |                       |                       | value, Java types     |
    |                       |                       | :::                   |
    +-----------------------+-----------------------+-----------------------+
    | `RuleKeyHasher<HASH>` | `p                    |                       |
    |                       | utNumber​(Number val)` |                       |
    +-----------------------+-----------------------+-----------------------+
    | `RuleKeyHasher<HASH>` | `p                    |                       |
    |                       | utPath​(Path path,     |                       |
    |                       |     com.google.common |                       |
    |                       | .hash.HashCode hash)` |                       |
    +-----------------------+-----------------------+-----------------------+
    | `RuleKeyHasher<HASH>` | `putPatt              |                       |
    |                       | ern​(Pattern pattern)` |                       |
    +-----------------------+-----------------------+-----------------------+
    | `RuleKeyHasher<HASH>` | `putRule              |                       |
    |                       | Key​(RuleKey ruleKey)` |                       |
    +-----------------------+-----------------------+-----------------------+
    | `RuleKeyHasher<HASH>` | `putRuleTyp           |                       |
    |                       | e​(RuleType ruleType)` |                       |
    +-----------------------+-----------------------+-----------------------+
    | `RuleKeyHasher<HASH>` | `putSha               | ::: block             |
    |                       | 1​(Sha1HashCode sha1)` | Puts the field\'s     |
    |                       |                       | value, Buck specific  |
    |                       |                       | types                 |
    |                       |                       | :::                   |
    +-----------------------+-----------------------+-----------------------+
    | `RuleKeyHasher<HASH>` | `p                    |                       |
    |                       | utString​(String val)` |                       |
    +-----------------------+-----------------------+-----------------------+
    | `RuleKeyHasher<HASH>` | `                     |                       |
    |                       | putWrapper​(RuleKeyHas |                       |
    |                       | her.Wrapper wrapper)` |                       |
    +-----------------------+-----------------------+-----------------------+

    : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
    Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2 .tableTab}[[Abstract
    Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
:::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#putKey(java.lang.String)}

        -   #### putKey

            ``` methodSignature
            RuleKeyHasher<HASH> putKey​(String key)
            ```

            ::: block
            Puts the field\'s key (i.e. the name of the field)
            :::

        []{#putKeyPath(java.nio.file.Path)}

        -   #### putKeyPath

            ``` methodSignature
            RuleKeyHasher<HASH> putKeyPath​(Path key)
            ```

            ::: block
            Puts the stringified path as a key.
            :::

        []{#putNull()}

        -   #### putNull

            ``` methodSignature
            RuleKeyHasher<HASH> putNull()
            ```

            ::: block
            Puts the field\'s value, Java types
            :::

        []{#putCharacter(char)}

        -   #### putCharacter

            ``` methodSignature
            RuleKeyHasher<HASH> putCharacter​(char val)
            ```

        []{#putBoolean(boolean)}

        -   #### putBoolean

            ``` methodSignature
            RuleKeyHasher<HASH> putBoolean​(boolean val)
            ```

        []{#putNumber(java.lang.Number)}

        -   #### putNumber

            ``` methodSignature
            RuleKeyHasher<HASH> putNumber​(Number val)
            ```

        []{#putString(java.lang.String)}

        -   #### putString

            ``` methodSignature
            RuleKeyHasher<HASH> putString​(String val)
            ```

        []{#putBytes(byte[])}

        -   #### putBytes

            ``` methodSignature
            RuleKeyHasher<HASH> putBytes​(byte[] bytes)
            ```

        []{#putPattern(java.util.regex.Pattern)}

        -   #### putPattern

            ``` methodSignature
            RuleKeyHasher<HASH> putPattern​(Pattern pattern)
            ```

        []{#putSha1(com.facebook.buck.util.sha1.Sha1HashCode)}

        -   #### putSha1

            ``` methodSignature
            RuleKeyHasher<HASH> putSha1​(Sha1HashCode sha1)
            ```

            ::: block
            Puts the field\'s value, Buck specific types
            :::

        []{#putPath(java.nio.file.Path,com.google.common.hash.HashCode)}

        -   #### putPath

            ``` methodSignature
            RuleKeyHasher<HASH> putPath​(Path path,
                                        com.google.common.hash.HashCode hash)
            ```

        []{#putArchiveMemberPath(java.nio.file.Path,java.nio.file.Path,com.google.common.hash.HashCode)}

        -   #### putArchiveMemberPath

            ``` methodSignature
            RuleKeyHasher<HASH> putArchiveMemberPath​(Path relativeArchivePath,
                                                     Path archiveMemberPath,
                                                     com.google.common.hash.HashCode hash)
            ```

            [Parameters:]{.paramLabel}
            :   `relativeArchivePath` - relative path to archive.
            :   `archiveMemberPath` - path to archive member.

        []{#putNonHashingPath(java.nio.file.Path)}

        -   #### putNonHashingPath

            ``` methodSignature
            RuleKeyHasher<HASH> putNonHashingPath​(Path path)
            ```

        []{#putRuleKey(com.facebook.buck.core.rulekey.RuleKey)}

        -   #### putRuleKey

            ``` methodSignature
            RuleKeyHasher<HASH> putRuleKey​(RuleKey ruleKey)
            ```

        []{#putRuleType(com.facebook.buck.core.model.RuleType)}

        -   #### putRuleType

            ``` methodSignature
            RuleKeyHasher<HASH> putRuleType​(RuleType ruleType)
            ```

        []{#putBuildTarget(com.facebook.buck.core.model.BuildTarget)}

        -   #### putBuildTarget

            ``` methodSignature
            RuleKeyHasher<HASH> putBuildTarget​(BuildTarget buildTarget)
            ```

        []{#putBuildTargetSourcePath(com.facebook.buck.core.sourcepath.BuildTargetSourcePath)}

        -   #### putBuildTargetSourcePath

            ``` methodSignature
            RuleKeyHasher<HASH> putBuildTargetSourcePath​(BuildTargetSourcePath buildTargetSourcePath)
            ```

        []{#putContainer(com.facebook.buck.rules.keys.hasher.RuleKeyHasher.Container,int)}

        -   #### putContainer

            ``` methodSignature
            RuleKeyHasher<HASH> putContainer​(RuleKeyHasher.Container container,
                                             int length)
            ```

            ::: block
            Puts the container signature
            :::

        []{#putWrapper(com.facebook.buck.rules.keys.hasher.RuleKeyHasher.Wrapper)}

        -   #### putWrapper

            ``` methodSignature
            RuleKeyHasher<HASH> putWrapper​(RuleKeyHasher.Wrapper wrapper)
            ```

        []{#hash()}

        -   #### hash

            ``` methodSignature
            HASH hash()
            ```

            ::: block
            Computes the final hash.
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

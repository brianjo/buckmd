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

## Class StringRuleKeyHasher {#class-stringrulekeyhasher .title title="Class StringRuleKeyHasher"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.keys.hasher.StringRuleKeyHasher

::: description
-   

    All Implemented Interfaces:
    :   `RuleKeyHasher<String>`

    ------------------------------------------------------------------------

        public class StringRuleKeyHasher
        extends Object
        implements RuleKeyHasher<String>

    ::: block
    An implementation of
    [`RuleKeyHasher`](RuleKeyHasher.html "interface in com.facebook.buck.rules.keys.hasher")
    that serializes to
    [`String`](http://docs.oracle.com/javase/7/docs/api/java/lang/String.html?is-external=true "class or interface in java.lang"){.externalLink}.
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

          Constructor               Description
          ------------------------- -------------
          `StringRuleKeyHasher()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `String`              | `hash()`              | ::: block             |
        |                       |                       | Computes the final    |
        |                       |                       | hash.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `StringRuleKeyHasher` | `pu                   |                       |
        |                       | tArchiveMemberPath​(Pa |                       |
        |                       | th relativeArchivePat |                       |
        |                       | h,                    |                       |
        |                       |   Path archiveMemberP |                       |
        |                       | ath,                  |                       |
        |                       |     com.google.common |                       |
        |                       | .hash.HashCode hash)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `StringRuleKeyHasher` | `put                  |                       |
        |                       | Boolean​(boolean val)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `StringRuleKeyHasher` | `putBuildTarget​(Buil  |                       |
        |                       | dTarget buildTarget)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `R                    | `pu                   |                       |
        | uleKeyHasher<String>` | tBuildTargetSourcePat |                       |
        |                       | h​(BuildTargetSourcePa |                       |
        |                       | th targetSourcePath)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `StringRuleKeyHasher` | `pu                   |                       |
        |                       | tBytes​(byte[] bytes)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `StringRuleKeyHasher` | `pu                   |                       |
        |                       | tCharacter​(char val)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `StringRuleKeyHasher` | `putContai            | ::: block             |
        |                       | ner​(RuleKeyHasher.Con | Puts the container    |
        |                       | tainer container,     | signature             |
        |                       |          int length)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `StringRuleKeyHasher` | `putKey​(String key)`  | ::: block             |
        |                       |                       | Puts the field\'s key |
        |                       |                       | (i.e.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `R                    | `                     | ::: block             |
        | uleKeyHasher<String>` | putKeyPath​(Path key)` | Puts the stringified  |
        |                       |                       | path as a key.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `StringRuleKeyHasher` | `putNonHa             |                       |
        |                       | shingPath​(Path path)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `StringRuleKeyHasher` | `putNull()`           | ::: block             |
        |                       |                       | Puts the field\'s     |
        |                       |                       | value, Java types     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `StringRuleKeyHasher` | `p                    |                       |
        |                       | utNumber​(Number val)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `StringRuleKeyHasher` | `p                    |                       |
        |                       | utPath​(Path path,     |                       |
        |                       |     com.google.common |                       |
        |                       | .hash.HashCode hash)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `StringRuleKeyHasher` | `putPatt              |                       |
        |                       | ern​(Pattern pattern)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `StringRuleKeyHasher` | `putRule              |                       |
        |                       | Key​(RuleKey ruleKey)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `StringRuleKeyHasher` | `putRuleTyp           |                       |
        |                       | e​(RuleType ruleType)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `StringRuleKeyHasher` | `putSha               | ::: block             |
        |                       | 1​(Sha1HashCode sha1)` | Puts the field\'s     |
        |                       |                       | value, Buck specific  |
        |                       |                       | types                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `StringRuleKeyHasher` | `p                    |                       |
        |                       | utString​(String val)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `StringRuleKeyHasher` | `                     |                       |
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

        []{#<init>()}

        -   #### StringRuleKeyHasher

                public StringRuleKeyHasher()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#putKey(java.lang.String)}

        -   #### putKey

            ``` methodSignature
            public StringRuleKeyHasher putKey​(String key)
            ```

            ::: block
            [Description copied from
            interface: `RuleKeyHasher`]{.descfrmTypeLabel}
            :::

            ::: block
            Puts the field\'s key (i.e. the name of the field)
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `putKey` in interface `RuleKeyHasher<String>`

        []{#putKeyPath(java.nio.file.Path)}

        -   #### putKeyPath

            ``` methodSignature
            public RuleKeyHasher<String> putKeyPath​(Path key)
            ```

            ::: block
            [Description copied from
            interface: `RuleKeyHasher`]{.descfrmTypeLabel}
            :::

            ::: block
            Puts the stringified path as a key.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `putKeyPath` in interface `RuleKeyHasher<String>`

        []{#putNull()}

        -   #### putNull

            ``` methodSignature
            public StringRuleKeyHasher putNull()
            ```

            ::: block
            [Description copied from
            interface: `RuleKeyHasher`]{.descfrmTypeLabel}
            :::

            ::: block
            Puts the field\'s value, Java types
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `putNull` in interface `RuleKeyHasher<String>`

        []{#putCharacter(char)}

        -   #### putCharacter

            ``` methodSignature
            public StringRuleKeyHasher putCharacter​(char val)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putCharacter` in interface `RuleKeyHasher<String>`

        []{#putBoolean(boolean)}

        -   #### putBoolean

            ``` methodSignature
            public StringRuleKeyHasher putBoolean​(boolean val)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putBoolean` in interface `RuleKeyHasher<String>`

        []{#putNumber(java.lang.Number)}

        -   #### putNumber

            ``` methodSignature
            public StringRuleKeyHasher putNumber​(Number val)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putNumber` in interface `RuleKeyHasher<String>`

        []{#putString(java.lang.String)}

        -   #### putString

            ``` methodSignature
            public StringRuleKeyHasher putString​(String val)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putString` in interface `RuleKeyHasher<String>`

        []{#putPattern(java.util.regex.Pattern)}

        -   #### putPattern

            ``` methodSignature
            public StringRuleKeyHasher putPattern​(Pattern pattern)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putPattern` in interface `RuleKeyHasher<String>`

        []{#putBytes(byte[])}

        -   #### putBytes

            ``` methodSignature
            public StringRuleKeyHasher putBytes​(byte[] bytes)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putBytes` in interface `RuleKeyHasher<String>`

        []{#putSha1(com.facebook.buck.util.sha1.Sha1HashCode)}

        -   #### putSha1

            ``` methodSignature
            public StringRuleKeyHasher putSha1​(Sha1HashCode sha1)
            ```

            ::: block
            [Description copied from
            interface: `RuleKeyHasher`]{.descfrmTypeLabel}
            :::

            ::: block
            Puts the field\'s value, Buck specific types
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `putSha1` in interface `RuleKeyHasher<String>`

        []{#putArchiveMemberPath(java.nio.file.Path,java.nio.file.Path,com.google.common.hash.HashCode)}

        -   #### putArchiveMemberPath

            ``` methodSignature
            public StringRuleKeyHasher putArchiveMemberPath​(Path relativeArchivePath,
                                                            Path archiveMemberPath,
                                                            com.google.common.hash.HashCode hash)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putArchiveMemberPath` in
                interface `RuleKeyHasher<String>`

            [Parameters:]{.paramLabel}
            :   `relativeArchivePath` - relative path to archive.
            :   `archiveMemberPath` - path to archive member.

        []{#putPath(java.nio.file.Path,com.google.common.hash.HashCode)}

        -   #### putPath

            ``` methodSignature
            public StringRuleKeyHasher putPath​(Path path,
                                               com.google.common.hash.HashCode hash)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putPath` in interface `RuleKeyHasher<String>`

        []{#putNonHashingPath(java.nio.file.Path)}

        -   #### putNonHashingPath

            ``` methodSignature
            public StringRuleKeyHasher putNonHashingPath​(Path path)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putNonHashingPath` in interface `RuleKeyHasher<String>`

        []{#putRuleKey(com.facebook.buck.core.rulekey.RuleKey)}

        -   #### putRuleKey

            ``` methodSignature
            public StringRuleKeyHasher putRuleKey​(RuleKey ruleKey)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putRuleKey` in interface `RuleKeyHasher<String>`

        []{#putRuleType(com.facebook.buck.core.model.RuleType)}

        -   #### putRuleType

            ``` methodSignature
            public StringRuleKeyHasher putRuleType​(RuleType ruleType)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putRuleType` in interface `RuleKeyHasher<String>`

        []{#putBuildTarget(com.facebook.buck.core.model.BuildTarget)}

        -   #### putBuildTarget

            ``` methodSignature
            public StringRuleKeyHasher putBuildTarget​(BuildTarget buildTarget)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putBuildTarget` in interface `RuleKeyHasher<String>`

        []{#putBuildTargetSourcePath(com.facebook.buck.core.sourcepath.BuildTargetSourcePath)}

        -   #### putBuildTargetSourcePath

            ``` methodSignature
            public RuleKeyHasher<String> putBuildTargetSourcePath​(BuildTargetSourcePath targetSourcePath)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putBuildTargetSourcePath` in
                interface `RuleKeyHasher<String>`

        []{#putContainer(com.facebook.buck.rules.keys.hasher.RuleKeyHasher.Container,int)}

        -   #### putContainer

            ``` methodSignature
            public StringRuleKeyHasher putContainer​(RuleKeyHasher.Container container,
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
            :   `putContainer` in interface `RuleKeyHasher<String>`

        []{#putWrapper(com.facebook.buck.rules.keys.hasher.RuleKeyHasher.Wrapper)}

        -   #### putWrapper

            ``` methodSignature
            public StringRuleKeyHasher putWrapper​(RuleKeyHasher.Wrapper wrapper)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `putWrapper` in interface `RuleKeyHasher<String>`

        []{#hash()}

        -   #### hash

            ``` methodSignature
            public String hash()
            ```

            ::: block
            [Description copied from
            interface: `RuleKeyHasher`]{.descfrmTypeLabel}
            :::

            ::: block
            Computes the final hash.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `hash` in interface `RuleKeyHasher<String>`
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

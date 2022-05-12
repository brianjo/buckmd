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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.build.engine.manifest](package-summary.html)
:::

## Class Manifest {#class-manifest .title title="Class Manifest"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.build.engine.manifest.Manifest

::: description
-   

    ------------------------------------------------------------------------

        public class Manifest
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `Manifest​(RuleKey key)`           | ::: block                         |
        |                                   | Create an empty manifest.         |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `Manifest​(InputStream rawInput)`  | ::: block                         |
        |                                   | Deserialize an existing manifest  |
        |                                   | from the given                    |
        |                                   | [`InputStream`]                   |
        |                                   | (http://docs.oracle.com/javase/7/ |
        |                                   | docs/api/java/io/InputStream.html |
        |                                   | ?is-external=true "class or inter |
        |                                   | face in java.io"){.externalLink}. |
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
        | `void`                | `addEntry​(F           | ::: block             |
        |                       | ileHashLoader fileHas | Adds a new output     |
        |                       | hLoader,         Rule | file to the manifest. |
        |                       | Key key,         Sour | :::                   |
        |                       | cePathResolverAdapter |                       |
        |                       |  resolver,         co |                       |
        |                       | m.google.common.colle |                       |
        |                       | ct.ImmutableSet<Sourc |                       |
        |                       | ePath> universe,      |                       |
        |                       |     com.google.common |                       |
        |                       | .collect.ImmutableSet |                       |
        |                       | <SourcePath> inputs)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `RuleKey`             | `getKey()`            |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ManifestStats`       | `getStats()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<RuleKey>`   | `                     |                       |
        |                       | lookup​(FileHashLoader |                       |
        |                       |  fileHashLoader,      |                       |
        |                       |   SourcePathResolverA |                       |
        |                       | dapter resolver,      |                       |
        |                       |   com.google.common.c |                       |
        |                       | ollect.ImmutableSet<S |                       |
        |                       | ourcePath> universe)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `serialize​(Out        | ::: block             |
        |                       | putStream rawOutput)` | Serializes the        |
        |                       |                       | manifest to the given |
        |                       |                       | [`                    |
        |                       |                       | OutputStream`](http:/ |
        |                       |                       | /docs.oracle.com/java |
        |                       |                       | se/7/docs/api/java/io |
        |                       |                       | /OutputStream.html?is |
        |                       |                       | -external=true "class |
        |                       |                       |  or interface in java |
        |                       |                       | .io"){.externalLink}. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `size()`              |                       |
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

        []{#<init>(com.facebook.buck.core.rulekey.RuleKey)}

        -   #### Manifest

                public Manifest​(RuleKey key)

            ::: block
            Create an empty manifest.
            :::

        []{#<init>(java.io.InputStream)}

        -   #### Manifest

                public Manifest​(InputStream rawInput)
                         throws IOException

            ::: block
            Deserialize an existing manifest from the given
            [`InputStream`](http://docs.oracle.com/javase/7/docs/api/java/io/InputStream.html?is-external=true "class or interface in java.io"){.externalLink}.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getKey()}

        -   #### getKey

            ``` methodSignature
            public RuleKey getKey()
            ```

        []{#lookup(com.facebook.buck.util.hashing.FileHashLoader,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,com.google.common.collect.ImmutableSet)}

        -   #### lookup

            ``` methodSignature
            public Optional<RuleKey> lookup​(FileHashLoader fileHashLoader,
                                            SourcePathResolverAdapter resolver,
                                            com.google.common.collect.ImmutableSet<SourcePath> universe)
                                     throws IOException
            ```

            [Returns:]{.returnLabel}
            :   the
                [`RuleKey`](../../../rulekey/RuleKey.html "class in com.facebook.buck.core.rulekey")
                of the entry that matches the on disk hashes provided by
                `      fileHashLoader`.

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#addEntry(com.facebook.buck.util.hashing.FileHashLoader,com.facebook.buck.core.rulekey.RuleKey,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,com.google.common.collect.ImmutableSet,com.google.common.collect.ImmutableSet)}

        -   #### addEntry

            ``` methodSignature
            public void addEntry​(FileHashLoader fileHashLoader,
                                 RuleKey key,
                                 SourcePathResolverAdapter resolver,
                                 com.google.common.collect.ImmutableSet<SourcePath> universe,
                                 com.google.common.collect.ImmutableSet<SourcePath> inputs)
                          throws IOException
            ```

            ::: block
            Adds a new output file to the manifest.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#serialize(java.io.OutputStream)}

        -   #### serialize

            ``` methodSignature
            public void serialize​(OutputStream rawOutput)
                           throws IOException
            ```

            ::: block
            Serializes the manifest to the given
            [`OutputStream`](http://docs.oracle.com/javase/7/docs/api/java/io/OutputStream.html?is-external=true "class or interface in java.io"){.externalLink}.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#size()}

        -   #### size

            ``` methodSignature
            public int size()
            ```

        []{#getStats()}

        -   #### getStats

            ``` methodSignature
            public ManifestStats getStats()
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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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

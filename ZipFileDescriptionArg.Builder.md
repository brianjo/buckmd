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
[Package]{.packageLabelInType} [com.facebook.buck.features.zip.rules](package-summary.html)
:::

## Class ZipFileDescriptionArg.Builder {#class-zipfiledescriptionarg.builder .title title="Class ZipFileDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.zip.rules.ZipFileDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [ZipFileDescriptionArg](ZipFileDescriptionArg.html "class in com.facebook.buck.features.zip.rules")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class ZipFileDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`ZipFileDescriptionArg`](ZipFileDescriptionArg.html "class in com.facebook.buck.features.zip.rules").
    Initialize attributes and then invoke the [`build()`](#build())
    method to create an immutable instance.
    *`Builder` is not thread-safe and generally should not be stored in
    a field or collection, but instead used immediately to create
    instances.*
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `ZipFileDe            | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`c                   |
        |                       | ildTarget> elements)` | ompatibleWith`](ZipFi |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ZipFileDe            | `addAllEntriesToExcl  | ::: block             |
        | scriptionArg.Builder` | ude​(Iterable<? extend | Adds elements to      |
        |                       | s Pattern> elements)` | [`entri               |
        |                       |                       | esToExclude`](ZipFile |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etEntriesToExclude()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ZipFileDe            | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels              |
        |                       |                       | `](ZipFileDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ZipFileDe            | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`licenses`]          |
        |                       |                       | (ZipFileDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ZipFileDe            | `addAllSrcs           | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`sr                  |
        |                       |                       | cs`](ZipFileDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ZipFileDe            | `addAllZipSrcs        | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`zipSrcs`            |
        |                       |                       | ](ZipFileDescriptionA |
        |                       |                       | rg.html#getZipSrcs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ZipFileDe            | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`c                   |
        |                       |                       | ompatibleWith`](ZipFi |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ZipFileDe            | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`c                   |
        |                       |                       | ompatibleWith`](ZipFi |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ZipFileDe            | `addEntriesToExcl     | ::: block             |
        | scriptionArg.Builder` | ude​(Pattern element)` | Adds one element to   |
        |                       |                       | [`entri               |
        |                       |                       | esToExclude`](ZipFile |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etEntriesToExclude()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ZipFileDe            | `addEntriesToExclude​( | ::: block             |
        | scriptionArg.Builder` | Pattern... elements)` | Adds elements to      |
        |                       |                       | [`entri               |
        |                       |                       | esToExclude`](ZipFile |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etEntriesToExclude()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ZipFileDe            | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels              |
        |                       |                       | `](ZipFileDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ZipFileDe            | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels              |
        |                       |                       | `](ZipFileDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ZipFileDe            | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`licenses`]          |
        |                       |                       | (ZipFileDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ZipFileDe            | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`licenses`]          |
        |                       |                       | (ZipFileDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ZipFileDe            | `addSrcs              | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`sr                  |
        |                       |                       | cs`](ZipFileDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ZipFileDe            | `addSrcs​(Sou          | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`sr                  |
        |                       |                       | cs`](ZipFileDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ZipFileDe            | `addZipSrcs           | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`zipSrcs`            |
        |                       |                       | ](ZipFileDescriptionA |
        |                       |                       | rg.html#getZipSrcs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ZipFileDe            | `addZipSrcs​(Sou       | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`zipSrcs`            |
        |                       |                       | ](ZipFileDescriptionA |
        |                       |                       | rg.html#getZipSrcs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Z                    | `build()`             | ::: block             |
        | ipFileDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`ZipFileDescripti    |
        |                       |                       | onArg`](ZipFileDescri |
        |                       |                       | ptionArg.html "class  |
        |                       |                       | in com.facebook.buck. |
        |                       |                       | features.zip.rules"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ZipFileDe            | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ZipFileDe            | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ZipFileDe            | `from​(com.facebook    | ::: block             |
        | scriptionArg.Builder` | .buck.features.zip.ru | Copy abstract value   |
        |                       | les.ZipFileDescriptio | type                  |
        |                       | n.AbstractZipFileDesc | `AbstractZ            |
        |                       | riptionArg instance)` | ipFileDescriptionArg` |
        |                       |                       | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ZipFileDe            | `from​(ZipFileDesc     | ::: block             |
        | scriptionArg.Builder` | riptionArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `Z                    |
        |                       |                       | ipFileDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ZipFileDe            | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`c                   |
        |                       |                       | ompatibleWith`](ZipFi |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ZipFileDe            | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`defaultTargetPl     |
        |                       |                       | atform`](ZipFileDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ZipFileDe            | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`defaultTargetPl     |
        |                       | faultTargetPlatform)` | atform`](ZipFileDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ZipFileDe            | `setEntriesToExcl     | ::: block             |
        | scriptionArg.Builder` | ude​(Iterable<? extend | Sets or replaces all  |
        |                       | s Pattern> elements)` | elements for          |
        |                       |                       | [`entri               |
        |                       |                       | esToExclude`](ZipFile |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etEntriesToExclude()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ZipFileDe            | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels              |
        |                       |                       | `](ZipFileDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ZipFileDe            | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`licenses`]          |
        |                       |                       | (ZipFileDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ZipFileDe            | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`na                  |
        |                       |                       | me`](ZipFileDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ZipFileDe            | `setOnDuplicat        | ::: block             |
        | scriptionArg.Builder` | eEntry​(OnDuplicateEnt | Initializes the value |
        |                       | ry onDuplicateEntry)` | for the               |
        |                       |                       | [`onDup               |
        |                       |                       | licateEntry`](ZipFile |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etOnDuplicateEntry()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ZipFileDe            | `setOut​(String out)`  | ::: block             |
        | scriptionArg.Builder` |                       | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`                    |
        |                       |                       | out`](ZipFileDescript |
        |                       |                       | ionArg.html#getOut()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ZipFileDe            | `setSrcs              | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`sr                  |
        |                       |                       | cs`](ZipFileDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ZipFileDe            | `setZipSrcs           | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`zipSrcs`            |
        |                       |                       | ](ZipFileDescriptionA |
        |                       |                       | rg.html#getZipSrcs()) |
        |                       |                       | list.                 |
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
    -   []{#method.detail}

        ### Method Detail

        []{#from(com.facebook.buck.features.zip.rules.ZipFileDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final ZipFileDescriptionArg.Builder from​(ZipFileDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `ZipFileDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.features.zip.rules.ZipFileDescription.AbstractZipFileDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final ZipFileDescriptionArg.Builder from​(com.facebook.buck.features.zip.rules.ZipFileDescription.AbstractZipFileDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type `AbstractZipFileDescriptionArg`
            instance into builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.BuildRuleArg)}

        -   #### from

            ``` methodSignature
            public final ZipFileDescriptionArg.Builder from​(BuildRuleArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.core.description.arg.BuildRuleArg`
            instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.ConstructorArg)}

        -   #### from

            ``` methodSignature
            public final ZipFileDescriptionArg.Builder from​(ConstructorArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.core.description.arg.ConstructorArg`
            instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setOut(java.lang.String)}

        -   #### setOut

            ``` methodSignature
            public final ZipFileDescriptionArg.Builder setOut​(String out)
            ```

            ::: block
            Initializes the value for the
            [`out`](ZipFileDescriptionArg.html#getOut()) attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`out`](ZipFileDescriptionArg.html#getOut()).*
            :::

            [Parameters:]{.paramLabel}
            :   `out` - The value for out

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSrcs(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addSrcs

            ``` methodSignature
            public final ZipFileDescriptionArg.Builder addSrcs​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`srcs`](ZipFileDescriptionArg.html#getSrcs()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A srcs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSrcs(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addSrcs

            ``` methodSignature
            public final ZipFileDescriptionArg.Builder addSrcs​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`srcs`](ZipFileDescriptionArg.html#getSrcs()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSrcs(java.lang.Iterable)}

        -   #### setSrcs

            ``` methodSignature
            public final ZipFileDescriptionArg.Builder setSrcs​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`srcs`](ZipFileDescriptionArg.html#getSrcs()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllSrcs(java.lang.Iterable)}

        -   #### addAllSrcs

            ``` methodSignature
            public final ZipFileDescriptionArg.Builder addAllSrcs​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`srcs`](ZipFileDescriptionArg.html#getSrcs()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addEntriesToExclude(java.util.regex.Pattern)}

        -   #### addEntriesToExclude

            ``` methodSignature
            public final ZipFileDescriptionArg.Builder addEntriesToExclude​(Pattern element)
            ```

            ::: block
            Adds one element to
            [`entriesToExclude`](ZipFileDescriptionArg.html#getEntriesToExclude())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A entriesToExclude element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addEntriesToExclude(java.util.regex.Pattern...)}

        -   #### addEntriesToExclude

            ``` methodSignature
            public final ZipFileDescriptionArg.Builder addEntriesToExclude​(Pattern... elements)
            ```

            ::: block
            Adds elements to
            [`entriesToExclude`](ZipFileDescriptionArg.html#getEntriesToExclude())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of entriesToExclude elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setEntriesToExclude(java.lang.Iterable)}

        -   #### setEntriesToExclude

            ``` methodSignature
            public final ZipFileDescriptionArg.Builder setEntriesToExclude​(Iterable<? extends Pattern> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`entriesToExclude`](ZipFileDescriptionArg.html#getEntriesToExclude())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of entriesToExclude elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllEntriesToExclude(java.lang.Iterable)}

        -   #### addAllEntriesToExclude

            ``` methodSignature
            public final ZipFileDescriptionArg.Builder addAllEntriesToExclude​(Iterable<? extends Pattern> elements)
            ```

            ::: block
            Adds elements to
            [`entriesToExclude`](ZipFileDescriptionArg.html#getEntriesToExclude())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of entriesToExclude elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addZipSrcs(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addZipSrcs

            ``` methodSignature
            public final ZipFileDescriptionArg.Builder addZipSrcs​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`zipSrcs`](ZipFileDescriptionArg.html#getZipSrcs()) list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A zipSrcs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addZipSrcs(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addZipSrcs

            ``` methodSignature
            public final ZipFileDescriptionArg.Builder addZipSrcs​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`zipSrcs`](ZipFileDescriptionArg.html#getZipSrcs()) list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of zipSrcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setZipSrcs(java.lang.Iterable)}

        -   #### setZipSrcs

            ``` methodSignature
            public final ZipFileDescriptionArg.Builder setZipSrcs​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`zipSrcs`](ZipFileDescriptionArg.html#getZipSrcs()) list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of zipSrcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllZipSrcs(java.lang.Iterable)}

        -   #### addAllZipSrcs

            ``` methodSignature
            public final ZipFileDescriptionArg.Builder addAllZipSrcs​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`zipSrcs`](ZipFileDescriptionArg.html#getZipSrcs()) list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of zipSrcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setOnDuplicateEntry(com.facebook.buck.util.zip.collect.OnDuplicateEntry)}

        -   #### setOnDuplicateEntry

            ``` methodSignature
            public final ZipFileDescriptionArg.Builder setOnDuplicateEntry​(OnDuplicateEntry onDuplicateEntry)
            ```

            ::: block
            Initializes the value for the
            [`onDuplicateEntry`](ZipFileDescriptionArg.html#getOnDuplicateEntry())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`onDuplicateEntry`](ZipFileDescriptionArg.html#getOnDuplicateEntry()).*
            :::

            [Parameters:]{.paramLabel}
            :   `onDuplicateEntry` - The value for onDuplicateEntry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final ZipFileDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](ZipFileDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final ZipFileDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](ZipFileDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final ZipFileDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](ZipFileDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final ZipFileDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](ZipFileDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final ZipFileDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](ZipFileDescriptionArg.html#getDefaultTargetPlatform())
            to defaultTargetPlatform.
            :::

            [Parameters:]{.paramLabel}
            :   `defaultTargetPlatform` - The value for
                defaultTargetPlatform

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setDefaultTargetPlatform(java.util.Optional)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final ZipFileDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](ZipFileDescriptionArg.html#getDefaultTargetPlatform())
            to defaultTargetPlatform.
            :::

            [Parameters:]{.paramLabel}
            :   `defaultTargetPlatform` - The value for
                defaultTargetPlatform

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String)}

        -   #### addLabels

            ``` methodSignature
            public final ZipFileDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](ZipFileDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final ZipFileDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](ZipFileDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final ZipFileDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](ZipFileDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final ZipFileDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](ZipFileDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final ZipFileDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](ZipFileDescriptionArg.html#getLicenses()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final ZipFileDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](ZipFileDescriptionArg.html#getLicenses()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final ZipFileDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](ZipFileDescriptionArg.html#getLicenses()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final ZipFileDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](ZipFileDescriptionArg.html#getLicenses()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final ZipFileDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](ZipFileDescriptionArg.html#getName()) attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public ZipFileDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`ZipFileDescriptionArg`](ZipFileDescriptionArg.html "class in com.facebook.buck.features.zip.rules").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of ZipFileDescriptionArg

            [Throws:]{.throwsLabel}
            :   `IllegalStateException` - if any required attributes are
                missing
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

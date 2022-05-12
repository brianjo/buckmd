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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.file](package-summary.html)
:::

## Class HttpArchiveDescriptionArg.Builder {#class-httparchivedescriptionarg.builder .title title="Class HttpArchiveDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.file.HttpArchiveDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [HttpArchiveDescriptionArg](HttpArchiveDescriptionArg.html "class in com.facebook.buck.file")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class HttpArchiveDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`HttpArchiveDescriptionArg`](HttpArchiveDescriptionArg.html "class in com.facebook.buck.file").
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
        | `HttpArchiveDe        | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`compa               |
        |                       | ildTarget> elements)` | tibleWith`](HttpArchi |
        |                       |                       | veDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpArchiveDe        | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels`](H          |
        |                       |                       | ttpArchiveDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpArchiveDe        | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`licenses`](Htt      |
        |                       |                       | pArchiveDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpArchiveDe        | `add                  | ::: block             |
        | scriptionArg.Builder` | AllUrls​(Iterable<? ex | Adds elements to      |
        |                       | tends URI> elements)` | [`urls`]              |
        |                       |                       | (HttpArchiveDescripti |
        |                       |                       | onArg.html#getUrls()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpArchiveDe        | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`compa               |
        |                       |                       | tibleWith`](HttpArchi |
        |                       |                       | veDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpArchiveDe        | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`compa               |
        |                       |                       | tibleWith`](HttpArchi |
        |                       |                       | veDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpArchiveDe        | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels`](H          |
        |                       |                       | ttpArchiveDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpArchiveDe        | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels`](H          |
        |                       |                       | ttpArchiveDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpArchiveDe        | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`licenses`](Htt      |
        |                       |                       | pArchiveDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpArchiveDe        | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`licenses`](Htt      |
        |                       |                       | pArchiveDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpArchiveDe        | `                     | ::: block             |
        | scriptionArg.Builder` | addUrls​(URI element)` | Adds one element to   |
        |                       |                       | [`urls`]              |
        |                       |                       | (HttpArchiveDescripti |
        |                       |                       | onArg.html#getUrls()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpArchiveDe        | `addU                 | ::: block             |
        | scriptionArg.Builder` | rls​(URI... elements)` | Adds elements to      |
        |                       |                       | [`urls`]              |
        |                       |                       | (HttpArchiveDescripti |
        |                       |                       | onArg.html#getUrls()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpA                | `build()`             | ::: block             |
        | rchiveDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`HttpArchiv          |
        |                       |                       | eDescriptionArg`](Htt |
        |                       |                       | pArchiveDescriptionAr |
        |                       |                       | g.html "class in com. |
        |                       |                       | facebook.buck.file"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpArchiveDe        | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpArchiveDe        | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpArchiveDe        | `from​(com.fa          | ::: block             |
        | scriptionArg.Builder` | cebook.buck.file.Http | Copy abstract value   |
        |                       | ArchiveDescription.Ab | type                  |
        |                       | stractHttpArchiveDesc | `AbstractHttpA        |
        |                       | riptionArg instance)` | rchiveDescriptionArg` |
        |                       |                       | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpArchiveDe        | `from​(HttpArchiveDesc | ::: block             |
        | scriptionArg.Builder` | riptionArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `HttpA                |
        |                       |                       | rchiveDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpArchiveDe        | `                     | ::: block             |
        | scriptionArg.Builder` | from​(com.facebook.buc | Fill a builder with   |
        |                       | k.file.HttpCommonDesc | attribute values from |
        |                       | riptionArg instance)` | the provided          |
        |                       |                       | `com.fa               |
        |                       |                       | cebook.buck.file.Http |
        |                       |                       | CommonDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpArchiveDe        | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`compa               |
        |                       |                       | tibleWith`](HttpArchi |
        |                       |                       | veDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpArchiveDe        | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`defaultTargetPlatfo |
        |                       |                       | rm`](HttpArchiveDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpArchiveDe        | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`defaultTargetPlatfo |
        |                       | faultTargetPlatform)` | rm`](HttpArchiveDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpArchiveDe        | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels`](H          |
        |                       |                       | ttpArchiveDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpArchiveDe        | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`licenses`](Htt      |
        |                       |                       | pArchiveDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpArchiveDe        | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`name`]              |
        |                       |                       | (HttpArchiveDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpArchiveDe        | `setOut​(String out)`  | ::: block             |
        | scriptionArg.Builder` |                       | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`out`                |
        |                       |                       | ](HttpArchiveDescript |
        |                       |                       | ionArg.html#getOut()) |
        |                       |                       | to out.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpArchiveDe        | `setOut​(O             | ::: block             |
        | scriptionArg.Builder` | ptional<String> out)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`out`                |
        |                       |                       | ](HttpArchiveDescript |
        |                       |                       | ionArg.html#getOut()) |
        |                       |                       | to out.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpArchiveDe        | `setS                 | ::: block             |
        | scriptionArg.Builder` | ha256​(String sha256)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`sha256`](H          |
        |                       |                       | ttpArchiveDescription |
        |                       |                       | Arg.html#getSha256()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpArchiveDe        | `setStripPrefix       | ::: block             |
        | scriptionArg.Builder` | ​(String stripPrefix)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [                     |
        |                       |                       | `stripPrefix`](HttpAr |
        |                       |                       | chiveDescriptionArg.h |
        |                       |                       | tml#getStripPrefix()) |
        |                       |                       | to stripPrefix.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpArchiveDe        | `set                  | ::: block             |
        | scriptionArg.Builder` | StripPrefix​(Optional< | Initializes the       |
        |                       | String> stripPrefix)` | optional value        |
        |                       |                       | [                     |
        |                       |                       | `stripPrefix`](HttpAr |
        |                       |                       | chiveDescriptionArg.h |
        |                       |                       | tml#getStripPrefix()) |
        |                       |                       | to stripPrefix.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpArchiveDe        | `                     | ::: block             |
        | scriptionArg.Builder` | setType​(String type)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`type`]              |
        |                       |                       | (HttpArchiveDescripti |
        |                       |                       | onArg.html#getType()) |
        |                       |                       | to type.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpArchiveDe        | `setType​(Op           | ::: block             |
        | scriptionArg.Builder` | tional<String> type)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`type`]              |
        |                       |                       | (HttpArchiveDescripti |
        |                       |                       | onArg.html#getType()) |
        |                       |                       | to type.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpArchiveDe        | `                     | ::: block             |
        | scriptionArg.Builder` | setUrls​(Iterable<? ex | Sets or replaces all  |
        |                       | tends URI> elements)` | elements for          |
        |                       |                       | [`urls`]              |
        |                       |                       | (HttpArchiveDescripti |
        |                       |                       | onArg.html#getUrls()) |
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

        []{#from(com.facebook.buck.file.HttpCommonDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final HttpArchiveDescriptionArg.Builder from​(com.facebook.buck.file.HttpCommonDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.file.HttpCommonDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.BuildRuleArg)}

        -   #### from

            ``` methodSignature
            public final HttpArchiveDescriptionArg.Builder from​(BuildRuleArg instance)
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
            public final HttpArchiveDescriptionArg.Builder from​(ConstructorArg instance)
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

        []{#from(com.facebook.buck.file.HttpArchiveDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final HttpArchiveDescriptionArg.Builder from​(HttpArchiveDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `HttpArchiveDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.file.HttpArchiveDescription.AbstractHttpArchiveDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final HttpArchiveDescriptionArg.Builder from​(com.facebook.buck.file.HttpArchiveDescription.AbstractHttpArchiveDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type `AbstractHttpArchiveDescriptionArg`
            instance into builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setStripPrefix(java.lang.String)}

        -   #### setStripPrefix

            ``` methodSignature
            public final HttpArchiveDescriptionArg.Builder setStripPrefix​(String stripPrefix)
            ```

            ::: block
            Initializes the optional value
            [`stripPrefix`](HttpArchiveDescriptionArg.html#getStripPrefix())
            to stripPrefix.
            :::

            [Parameters:]{.paramLabel}
            :   `stripPrefix` - The value for stripPrefix

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setStripPrefix(java.util.Optional)}

        -   #### setStripPrefix

            ``` methodSignature
            public final HttpArchiveDescriptionArg.Builder setStripPrefix​(Optional<String> stripPrefix)
            ```

            ::: block
            Initializes the optional value
            [`stripPrefix`](HttpArchiveDescriptionArg.html#getStripPrefix())
            to stripPrefix.
            :::

            [Parameters:]{.paramLabel}
            :   `stripPrefix` - The value for stripPrefix

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setType(java.lang.String)}

        -   #### setType

            ``` methodSignature
            public final HttpArchiveDescriptionArg.Builder setType​(String type)
            ```

            ::: block
            Initializes the optional value
            [`type`](HttpArchiveDescriptionArg.html#getType()) to type.
            :::

            [Parameters:]{.paramLabel}
            :   `type` - The value for type

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setType(java.util.Optional)}

        -   #### setType

            ``` methodSignature
            public final HttpArchiveDescriptionArg.Builder setType​(Optional<String> type)
            ```

            ::: block
            Initializes the optional value
            [`type`](HttpArchiveDescriptionArg.html#getType()) to type.
            :::

            [Parameters:]{.paramLabel}
            :   `type` - The value for type

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSha256(java.lang.String)}

        -   #### setSha256

            ``` methodSignature
            public final HttpArchiveDescriptionArg.Builder setSha256​(String sha256)
            ```

            ::: block
            Initializes the value for the
            [`sha256`](HttpArchiveDescriptionArg.html#getSha256())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `sha256` - The value for sha256

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addUrls(java.net.URI)}

        -   #### addUrls

            ``` methodSignature
            public final HttpArchiveDescriptionArg.Builder addUrls​(URI element)
            ```

            ::: block
            Adds one element to
            [`urls`](HttpArchiveDescriptionArg.html#getUrls()) list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A urls element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addUrls(java.net.URI...)}

        -   #### addUrls

            ``` methodSignature
            public final HttpArchiveDescriptionArg.Builder addUrls​(URI... elements)
            ```

            ::: block
            Adds elements to
            [`urls`](HttpArchiveDescriptionArg.html#getUrls()) list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of urls elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setUrls(java.lang.Iterable)}

        -   #### setUrls

            ``` methodSignature
            public final HttpArchiveDescriptionArg.Builder setUrls​(Iterable<? extends URI> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`urls`](HttpArchiveDescriptionArg.html#getUrls()) list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of urls elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllUrls(java.lang.Iterable)}

        -   #### addAllUrls

            ``` methodSignature
            public final HttpArchiveDescriptionArg.Builder addAllUrls​(Iterable<? extends URI> elements)
            ```

            ::: block
            Adds elements to
            [`urls`](HttpArchiveDescriptionArg.html#getUrls()) list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of urls elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setOut(java.lang.String)}

        -   #### setOut

            ``` methodSignature
            public final HttpArchiveDescriptionArg.Builder setOut​(String out)
            ```

            ::: block
            Initializes the optional value
            [`out`](HttpArchiveDescriptionArg.html#getOut()) to out.
            :::

            [Parameters:]{.paramLabel}
            :   `out` - The value for out

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setOut(java.util.Optional)}

        -   #### setOut

            ``` methodSignature
            public final HttpArchiveDescriptionArg.Builder setOut​(Optional<String> out)
            ```

            ::: block
            Initializes the optional value
            [`out`](HttpArchiveDescriptionArg.html#getOut()) to out.
            :::

            [Parameters:]{.paramLabel}
            :   `out` - The value for out

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final HttpArchiveDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](HttpArchiveDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final HttpArchiveDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](HttpArchiveDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final HttpArchiveDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](HttpArchiveDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final HttpArchiveDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](HttpArchiveDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String)}

        -   #### addLabels

            ``` methodSignature
            public final HttpArchiveDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](HttpArchiveDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final HttpArchiveDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](HttpArchiveDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final HttpArchiveDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](HttpArchiveDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final HttpArchiveDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](HttpArchiveDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final HttpArchiveDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](HttpArchiveDescriptionArg.html#getDefaultTargetPlatform())
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
            public final HttpArchiveDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](HttpArchiveDescriptionArg.html#getDefaultTargetPlatform())
            to defaultTargetPlatform.
            :::

            [Parameters:]{.paramLabel}
            :   `defaultTargetPlatform` - The value for
                defaultTargetPlatform

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final HttpArchiveDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](HttpArchiveDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final HttpArchiveDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](HttpArchiveDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final HttpArchiveDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](HttpArchiveDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final HttpArchiveDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](HttpArchiveDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final HttpArchiveDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](HttpArchiveDescriptionArg.html#getName())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public HttpArchiveDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`HttpArchiveDescriptionArg`](HttpArchiveDescriptionArg.html "class in com.facebook.buck.file").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of HttpArchiveDescriptionArg

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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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

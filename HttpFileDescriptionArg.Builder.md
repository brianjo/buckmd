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

## Class HttpFileDescriptionArg.Builder {#class-httpfiledescriptionarg.builder .title title="Class HttpFileDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.file.HttpFileDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [HttpFileDescriptionArg](HttpFileDescriptionArg.html "class in com.facebook.buck.file")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class HttpFileDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`HttpFileDescriptionArg`](HttpFileDescriptionArg.html "class in com.facebook.buck.file").
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
        | `HttpFileDe           | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`co                  |
        |                       | ildTarget> elements)` | mpatibleWith`](HttpFi |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpFileDe           | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels`             |
        |                       |                       | ](HttpFileDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpFileDe           | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`licenses`](         |
        |                       |                       | HttpFileDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpFileDe           | `add                  | ::: block             |
        | scriptionArg.Builder` | AllUrls​(Iterable<? ex | Adds elements to      |
        |                       | tends URI> elements)` | [`url                 |
        |                       |                       | s`](HttpFileDescripti |
        |                       |                       | onArg.html#getUrls()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpFileDe           | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`co                  |
        |                       |                       | mpatibleWith`](HttpFi |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpFileDe           | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`co                  |
        |                       |                       | mpatibleWith`](HttpFi |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpFileDe           | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels`             |
        |                       |                       | ](HttpFileDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpFileDe           | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels`             |
        |                       |                       | ](HttpFileDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpFileDe           | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`licenses`](         |
        |                       |                       | HttpFileDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpFileDe           | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`licenses`](         |
        |                       |                       | HttpFileDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpFileDe           | `                     | ::: block             |
        | scriptionArg.Builder` | addUrls​(URI element)` | Adds one element to   |
        |                       |                       | [`url                 |
        |                       |                       | s`](HttpFileDescripti |
        |                       |                       | onArg.html#getUrls()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpFileDe           | `addU                 | ::: block             |
        | scriptionArg.Builder` | rls​(URI... elements)` | Adds elements to      |
        |                       |                       | [`url                 |
        |                       |                       | s`](HttpFileDescripti |
        |                       |                       | onArg.html#getUrls()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Ht                   | `build()`             | ::: block             |
        | tpFileDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`Http                |
        |                       |                       | FileDescriptionArg`]( |
        |                       |                       | HttpFileDescriptionAr |
        |                       |                       | g.html "class in com. |
        |                       |                       | facebook.buck.file"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpFileDe           | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpFileDe           | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpFileDe           | `                     | ::: block             |
        | scriptionArg.Builder` | from​(com.facebook.buc | Fill a builder with   |
        |                       | k.file.HttpCommonDesc | attribute values from |
        |                       | riptionArg instance)` | the provided          |
        |                       |                       | `com.fa               |
        |                       |                       | cebook.buck.file.Http |
        |                       |                       | CommonDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpFileDe           | `from​(                | ::: block             |
        | scriptionArg.Builder` | com.facebook.buck.fil | Copy abstract value   |
        |                       | e.HttpFileDescription | type                  |
        |                       | .AbstractHttpFileDesc | `AbstractHt           |
        |                       | riptionArg instance)` | tpFileDescriptionArg` |
        |                       |                       | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpFileDe           | `from​(HttpFileDesc    | ::: block             |
        | scriptionArg.Builder` | riptionArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `Ht                   |
        |                       |                       | tpFileDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpFileDe           | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`co                  |
        |                       |                       | mpatibleWith`](HttpFi |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpFileDe           | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`defaultTargetPla    |
        |                       |                       | tform`](HttpFileDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpFileDe           | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`defaultTargetPla    |
        |                       | faultTargetPlatform)` | tform`](HttpFileDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpFileDe           | `setExecutable        | ::: block             |
        | scriptionArg.Builder` | ​(boolean executable)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`executable`](Ht     |
        |                       |                       | tpFileDescriptionArg. |
        |                       |                       | html#getExecutable()) |
        |                       |                       | to executable.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpFileDe           | `se                   | ::: block             |
        | scriptionArg.Builder` | tExecutable​(Optional< | Initializes the       |
        |                       | Boolean> executable)` | optional value        |
        |                       |                       | [`executable`](Ht     |
        |                       |                       | tpFileDescriptionArg. |
        |                       |                       | html#getExecutable()) |
        |                       |                       | to executable.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpFileDe           | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels`             |
        |                       |                       | ](HttpFileDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpFileDe           | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`licenses`](         |
        |                       |                       | HttpFileDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpFileDe           | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`nam                 |
        |                       |                       | e`](HttpFileDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpFileDe           | `setOut​(String out)`  | ::: block             |
        | scriptionArg.Builder` |                       | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`o                   |
        |                       |                       | ut`](HttpFileDescript |
        |                       |                       | ionArg.html#getOut()) |
        |                       |                       | to out.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpFileDe           | `setOut​(O             | ::: block             |
        | scriptionArg.Builder` | ptional<String> out)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`o                   |
        |                       |                       | ut`](HttpFileDescript |
        |                       |                       | ionArg.html#getOut()) |
        |                       |                       | to out.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpFileDe           | `setS                 | ::: block             |
        | scriptionArg.Builder` | ha256​(String sha256)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`sha256`             |
        |                       |                       | ](HttpFileDescription |
        |                       |                       | Arg.html#getSha256()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HttpFileDe           | `                     | ::: block             |
        | scriptionArg.Builder` | setUrls​(Iterable<? ex | Sets or replaces all  |
        |                       | tends URI> elements)` | elements for          |
        |                       |                       | [`url                 |
        |                       |                       | s`](HttpFileDescripti |
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
            public final HttpFileDescriptionArg.Builder from​(com.facebook.buck.file.HttpCommonDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.file.HttpCommonDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.file.HttpFileDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final HttpFileDescriptionArg.Builder from​(HttpFileDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `HttpFileDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.file.HttpFileDescription.AbstractHttpFileDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final HttpFileDescriptionArg.Builder from​(com.facebook.buck.file.HttpFileDescription.AbstractHttpFileDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type `AbstractHttpFileDescriptionArg`
            instance into builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.BuildRuleArg)}

        -   #### from

            ``` methodSignature
            public final HttpFileDescriptionArg.Builder from​(BuildRuleArg instance)
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
            public final HttpFileDescriptionArg.Builder from​(ConstructorArg instance)
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

        []{#setExecutable(boolean)}

        -   #### setExecutable

            ``` methodSignature
            public final HttpFileDescriptionArg.Builder setExecutable​(boolean executable)
            ```

            ::: block
            Initializes the optional value
            [`executable`](HttpFileDescriptionArg.html#getExecutable())
            to executable.
            :::

            [Parameters:]{.paramLabel}
            :   `executable` - The value for executable

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setExecutable(java.util.Optional)}

        -   #### setExecutable

            ``` methodSignature
            public final HttpFileDescriptionArg.Builder setExecutable​(Optional<Boolean> executable)
            ```

            ::: block
            Initializes the optional value
            [`executable`](HttpFileDescriptionArg.html#getExecutable())
            to executable.
            :::

            [Parameters:]{.paramLabel}
            :   `executable` - The value for executable

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSha256(java.lang.String)}

        -   #### setSha256

            ``` methodSignature
            public final HttpFileDescriptionArg.Builder setSha256​(String sha256)
            ```

            ::: block
            Initializes the value for the
            [`sha256`](HttpFileDescriptionArg.html#getSha256())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `sha256` - The value for sha256

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addUrls(java.net.URI)}

        -   #### addUrls

            ``` methodSignature
            public final HttpFileDescriptionArg.Builder addUrls​(URI element)
            ```

            ::: block
            Adds one element to
            [`urls`](HttpFileDescriptionArg.html#getUrls()) list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A urls element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addUrls(java.net.URI...)}

        -   #### addUrls

            ``` methodSignature
            public final HttpFileDescriptionArg.Builder addUrls​(URI... elements)
            ```

            ::: block
            Adds elements to
            [`urls`](HttpFileDescriptionArg.html#getUrls()) list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of urls elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setUrls(java.lang.Iterable)}

        -   #### setUrls

            ``` methodSignature
            public final HttpFileDescriptionArg.Builder setUrls​(Iterable<? extends URI> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`urls`](HttpFileDescriptionArg.html#getUrls()) list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of urls elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllUrls(java.lang.Iterable)}

        -   #### addAllUrls

            ``` methodSignature
            public final HttpFileDescriptionArg.Builder addAllUrls​(Iterable<? extends URI> elements)
            ```

            ::: block
            Adds elements to
            [`urls`](HttpFileDescriptionArg.html#getUrls()) list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of urls elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setOut(java.lang.String)}

        -   #### setOut

            ``` methodSignature
            public final HttpFileDescriptionArg.Builder setOut​(String out)
            ```

            ::: block
            Initializes the optional value
            [`out`](HttpFileDescriptionArg.html#getOut()) to out.
            :::

            [Parameters:]{.paramLabel}
            :   `out` - The value for out

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setOut(java.util.Optional)}

        -   #### setOut

            ``` methodSignature
            public final HttpFileDescriptionArg.Builder setOut​(Optional<String> out)
            ```

            ::: block
            Initializes the optional value
            [`out`](HttpFileDescriptionArg.html#getOut()) to out.
            :::

            [Parameters:]{.paramLabel}
            :   `out` - The value for out

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final HttpFileDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](HttpFileDescriptionArg.html#getLicenses()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final HttpFileDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](HttpFileDescriptionArg.html#getLicenses()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final HttpFileDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](HttpFileDescriptionArg.html#getLicenses()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final HttpFileDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](HttpFileDescriptionArg.html#getLicenses()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String)}

        -   #### addLabels

            ``` methodSignature
            public final HttpFileDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](HttpFileDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final HttpFileDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](HttpFileDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final HttpFileDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](HttpFileDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final HttpFileDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](HttpFileDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final HttpFileDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](HttpFileDescriptionArg.html#getDefaultTargetPlatform())
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
            public final HttpFileDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](HttpFileDescriptionArg.html#getDefaultTargetPlatform())
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
            public final HttpFileDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](HttpFileDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final HttpFileDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](HttpFileDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final HttpFileDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](HttpFileDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final HttpFileDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](HttpFileDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final HttpFileDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](HttpFileDescriptionArg.html#getName()) attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public HttpFileDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`HttpFileDescriptionArg`](HttpFileDescriptionArg.html "class in com.facebook.buck.file").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of HttpFileDescriptionArg

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

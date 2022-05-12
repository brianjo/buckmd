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
[Package]{.packageLabelInType} [com.facebook.buck.apple](package-summary.html)
:::

## Class AppleToolchainSetDescriptionArg.Builder {#class-appletoolchainsetdescriptionarg.builder .title title="Class AppleToolchainSetDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.AppleToolchainSetDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [AppleToolchainSetDescriptionArg](AppleToolchainSetDescriptionArg.html "class in com.facebook.buck.apple")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class AppleToolchainSetDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`AppleToolchainSetDescriptionArg`](AppleToolchainSetDescriptionArg.html "class in com.facebook.buck.apple").
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
        | `AppleToolchainSetDe  | `a                    | ::: block             |
        | scriptionArg.Builder` | ddAllAppleToolchains​( | Adds elements to      |
        |                       | Iterable<? extends Bu | [`appleToolchai       |
        |                       | ildTarget> elements)` | ns`](AppleToolchainSe |
        |                       |                       | tDescriptionArg.html# |
        |                       |                       | getAppleToolchains()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainSetDe  | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`compatibleW         |
        |                       | ildTarget> elements)` | ith`](AppleToolchainS |
        |                       |                       | etDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainSetDe  | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels`](AppleTo    |
        |                       |                       | olchainSetDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainSetDe  | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [                     |
        |                       |                       | `licenses`](AppleTool |
        |                       |                       | chainSetDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainSetDe  | `addAppleToolchains​(  | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`appleToolchai       |
        |                       |                       | ns`](AppleToolchainSe |
        |                       |                       | tDescriptionArg.html# |
        |                       |                       | getAppleToolchains()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainSetDe  | `ad                   | ::: block             |
        | scriptionArg.Builder` | dAppleToolchains​(Buil | Adds elements to      |
        |                       | dTarget... elements)` | [`appleToolchai       |
        |                       |                       | ns`](AppleToolchainSe |
        |                       |                       | tDescriptionArg.html# |
        |                       |                       | getAppleToolchains()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainSetDe  | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`compatibleW         |
        |                       |                       | ith`](AppleToolchainS |
        |                       |                       | etDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainSetDe  | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`compatibleW         |
        |                       |                       | ith`](AppleToolchainS |
        |                       |                       | etDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainSetDe  | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels`](AppleTo    |
        |                       |                       | olchainSetDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainSetDe  | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels`](AppleTo    |
        |                       |                       | olchainSetDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainSetDe  | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [                     |
        |                       |                       | `licenses`](AppleTool |
        |                       |                       | chainSetDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainSetDe  | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [                     |
        |                       |                       | `licenses`](AppleTool |
        |                       |                       | chainSetDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolch          | `build()`             | ::: block             |
        | ainSetDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`Ap                  |
        |                       |                       | pleToolchainSetDescri |
        |                       |                       | ptionArg`](AppleToolc |
        |                       |                       | hainSetDescriptionArg |
        |                       |                       | .html "class in com.f |
        |                       |                       | acebook.buck.apple"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainSetDe  | `fro                  | ::: block             |
        | scriptionArg.Builder` | m​(com.facebook.buck.a | Copy abstract value   |
        |                       | pple.AppleToolchainSe | type                  |
        |                       | tDescription.Abstract | `AbstractAppleToolch  |
        |                       | AppleToolchainSetDesc | ainSetDescriptionArg` |
        |                       | riptionArg instance)` | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainSetDe  | `from​(                | ::: block             |
        | scriptionArg.Builder` | AppleToolchainSetDesc | Fill a builder with   |
        |                       | riptionArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `AppleToolch          |
        |                       |                       | ainSetDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainSetDe  | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainSetDe  | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainSetDe  | `setAppleToolchains​(  | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`appleToolchai       |
        |                       |                       | ns`](AppleToolchainSe |
        |                       |                       | tDescriptionArg.html# |
        |                       |                       | getAppleToolchains()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainSetDe  | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`compatibleW         |
        |                       |                       | ith`](AppleToolchainS |
        |                       |                       | etDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainSetDe  | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`defa                |
        |                       |                       | ultTargetPlatform`](A |
        |                       |                       | ppleToolchainSetDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainSetDe  | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`defa                |
        |                       | faultTargetPlatform)` | ultTargetPlatform`](A |
        |                       |                       | ppleToolchainSetDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainSetDe  | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels`](AppleTo    |
        |                       |                       | olchainSetDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainSetDe  | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [                     |
        |                       |                       | `licenses`](AppleTool |
        |                       |                       | chainSetDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleToolchainSetDe  | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`name`](Apple        |
        |                       |                       | ToolchainSetDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
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

        []{#from(com.facebook.buck.apple.AppleToolchainSetDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final AppleToolchainSetDescriptionArg.Builder from​(AppleToolchainSetDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `AppleToolchainSetDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.apple.AppleToolchainSetDescription.AbstractAppleToolchainSetDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final AppleToolchainSetDescriptionArg.Builder from​(com.facebook.buck.apple.AppleToolchainSetDescription.AbstractAppleToolchainSetDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type
            `AbstractAppleToolchainSetDescriptionArg` instance into
            builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.BuildRuleArg)}

        -   #### from

            ``` methodSignature
            public final AppleToolchainSetDescriptionArg.Builder from​(BuildRuleArg instance)
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
            public final AppleToolchainSetDescriptionArg.Builder from​(ConstructorArg instance)
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

        []{#addAppleToolchains(com.facebook.buck.core.model.BuildTarget)}

        -   #### addAppleToolchains

            ``` methodSignature
            public final AppleToolchainSetDescriptionArg.Builder addAppleToolchains​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`appleToolchains`](AppleToolchainSetDescriptionArg.html#getAppleToolchains())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A appleToolchains element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAppleToolchains(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addAppleToolchains

            ``` methodSignature
            public final AppleToolchainSetDescriptionArg.Builder addAppleToolchains​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`appleToolchains`](AppleToolchainSetDescriptionArg.html#getAppleToolchains())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of appleToolchains elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAppleToolchains(java.lang.Iterable)}

        -   #### setAppleToolchains

            ``` methodSignature
            public final AppleToolchainSetDescriptionArg.Builder setAppleToolchains​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`appleToolchains`](AppleToolchainSetDescriptionArg.html#getAppleToolchains())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of appleToolchains elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllAppleToolchains(java.lang.Iterable)}

        -   #### addAllAppleToolchains

            ``` methodSignature
            public final AppleToolchainSetDescriptionArg.Builder addAllAppleToolchains​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`appleToolchains`](AppleToolchainSetDescriptionArg.html#getAppleToolchains())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of appleToolchains elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final AppleToolchainSetDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](AppleToolchainSetDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final AppleToolchainSetDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](AppleToolchainSetDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final AppleToolchainSetDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](AppleToolchainSetDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final AppleToolchainSetDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](AppleToolchainSetDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String)}

        -   #### addLabels

            ``` methodSignature
            public final AppleToolchainSetDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](AppleToolchainSetDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final AppleToolchainSetDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](AppleToolchainSetDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final AppleToolchainSetDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](AppleToolchainSetDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final AppleToolchainSetDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](AppleToolchainSetDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final AppleToolchainSetDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](AppleToolchainSetDescriptionArg.html#getDefaultTargetPlatform())
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
            public final AppleToolchainSetDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](AppleToolchainSetDescriptionArg.html#getDefaultTargetPlatform())
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
            public final AppleToolchainSetDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](AppleToolchainSetDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final AppleToolchainSetDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](AppleToolchainSetDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final AppleToolchainSetDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](AppleToolchainSetDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final AppleToolchainSetDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](AppleToolchainSetDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final AppleToolchainSetDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](AppleToolchainSetDescriptionArg.html#getName())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public AppleToolchainSetDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`AppleToolchainSetDescriptionArg`](AppleToolchainSetDescriptionArg.html "class in com.facebook.buck.apple").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of AppleToolchainSetDescriptionArg

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
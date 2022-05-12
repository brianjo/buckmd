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
[Package]{.packageLabelInType} [com.facebook.buck.android](package-summary.html)
:::

## Class NdkToolchainDescriptionArg.Builder {#class-ndktoolchaindescriptionarg.builder .title title="Class NdkToolchainDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.NdkToolchainDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [NdkToolchainDescriptionArg](NdkToolchainDescriptionArg.html "class in com.facebook.buck.android")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class NdkToolchainDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`NdkToolchainDescriptionArg`](NdkToolchainDescriptionArg.html "class in com.facebook.buck.android").
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
        | `NdkToolchainDe       | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`compat              |
        |                       | ildTarget> elements)` | ibleWith`](NdkToolcha |
        |                       |                       | inDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `NdkToolchainDe       | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels`](Nd         |
        |                       |                       | kToolchainDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `NdkToolchainDe       | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`licenses`](NdkT     |
        |                       |                       | oolchainDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `NdkToolchainDe       | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`compat              |
        |                       |                       | ibleWith`](NdkToolcha |
        |                       |                       | inDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `NdkToolchainDe       | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`compat              |
        |                       |                       | ibleWith`](NdkToolcha |
        |                       |                       | inDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `NdkToolchainDe       | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels`](Nd         |
        |                       |                       | kToolchainDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `NdkToolchainDe       | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels`](Nd         |
        |                       |                       | kToolchainDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `NdkToolchainDe       | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`licenses`](NdkT     |
        |                       |                       | oolchainDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `NdkToolchainDe       | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`licenses`](NdkT     |
        |                       |                       | oolchainDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `NdkToo               | `build()`             | ::: block             |
        | lchainDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`NdkToolchainDes     |
        |                       |                       | criptionArg`](NdkTool |
        |                       |                       | chainDescriptionArg.h |
        |                       |                       | tml "class in com.fac |
        |                       |                       | ebook.buck.android"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `NdkToolchainDe       | `from​(com.faceboo     | ::: block             |
        | scriptionArg.Builder` | k.buck.android.NdkToo | Copy abstract value   |
        |                       | lchainDescription.Abs | type                  |
        |                       | tractNdkToolchainDesc | `AbstractNdkToo       |
        |                       | riptionArg instance)` | lchainDescriptionArg` |
        |                       |                       | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `NdkToolchainDe       | `                     | ::: block             |
        | scriptionArg.Builder` | from​(NdkToolchainDesc | Fill a builder with   |
        |                       | riptionArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `NdkToo               |
        |                       |                       | lchainDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `NdkToolchainDe       | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `NdkToolchainDe       | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `NdkToolchainDe       | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`compat              |
        |                       |                       | ibleWith`](NdkToolcha |
        |                       |                       | inDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `NdkToolchainDe       | `setCxxRuntime​(NdkCx  | ::: block             |
        | scriptionArg.Builder` | xRuntime cxxRuntime)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`cxxRuntime`](NdkToo |
        |                       |                       | lchainDescriptionArg. |
        |                       |                       | html#getCxxRuntime()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `NdkToolchainDe       | `                     | ::: block             |
        | scriptionArg.Builder` | setCxxToolchain​(Build | Initializes the value |
        |                       | Target cxxToolchain)` | for the               |
        |                       |                       | [`cx                  |
        |                       |                       | xToolchain`](NdkToolc |
        |                       |                       | hainDescriptionArg.ht |
        |                       |                       | ml#getCxxToolchain()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `NdkToolchainDe       | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [                     |
        |                       |                       | `defaultTargetPlatfor |
        |                       |                       | m`](NdkToolchainDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `NdkToolchainDe       | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [                     |
        |                       | faultTargetPlatform)` | `defaultTargetPlatfor |
        |                       |                       | m`](NdkToolchainDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `NdkToolchainDe       | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels`](Nd         |
        |                       |                       | kToolchainDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `NdkToolchainDe       | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`licenses`](NdkT     |
        |                       |                       | oolchainDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `NdkToolchainDe       | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`name`](             |
        |                       |                       | NdkToolchainDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `NdkToolchainDe       | `setNdkPath           | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath ndkPath)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`ndkPath`](Ndk       |
        |                       |                       | ToolchainDescriptionA |
        |                       |                       | rg.html#getNdkPath()) |
        |                       |                       | to ndkPath.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `NdkToolchainDe       | `setNdkPat            | ::: block             |
        | scriptionArg.Builder` | h​(Optional<? extends  | Initializes the       |
        |                       | SourcePath> ndkPath)` | optional value        |
        |                       |                       | [`ndkPath`](Ndk       |
        |                       |                       | ToolchainDescriptionA |
        |                       |                       | rg.html#getNdkPath()) |
        |                       |                       | to ndkPath.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `NdkToolchainDe       | `setObjdump           | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath objdump)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`objdump`](Ndk       |
        |                       |                       | ToolchainDescriptionA |
        |                       |                       | rg.html#getObjdump()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `NdkToolchainDe       | `setShared            | ::: block             |
        | scriptionArg.Builder` | RuntimePath​(SourcePat | Initializes the       |
        |                       | h sharedRuntimePath)` | optional value        |
        |                       |                       | [`sharedRuntim        |
        |                       |                       | ePath`](NdkToolchainD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tSharedRuntimePath()) |
        |                       |                       | to sharedRuntimePath. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `NdkToolchainDe       | `setShare             | ::: block             |
        | scriptionArg.Builder` | dRuntimePath​(Optional | Initializes the       |
        |                       | <? extends SourcePath | optional value        |
        |                       | > sharedRuntimePath)` | [`sharedRuntim        |
        |                       |                       | ePath`](NdkToolchainD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tSharedRuntimePath()) |
        |                       |                       | to sharedRuntimePath. |
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

        []{#from(com.facebook.buck.android.NdkToolchainDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final NdkToolchainDescriptionArg.Builder from​(NdkToolchainDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `NdkToolchainDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.android.NdkToolchainDescription.AbstractNdkToolchainDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final NdkToolchainDescriptionArg.Builder from​(com.facebook.buck.android.NdkToolchainDescription.AbstractNdkToolchainDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type
            `AbstractNdkToolchainDescriptionArg` instance into builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.BuildRuleArg)}

        -   #### from

            ``` methodSignature
            public final NdkToolchainDescriptionArg.Builder from​(BuildRuleArg instance)
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
            public final NdkToolchainDescriptionArg.Builder from​(ConstructorArg instance)
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

        []{#setCxxToolchain(com.facebook.buck.core.model.BuildTarget)}

        -   #### setCxxToolchain

            ``` methodSignature
            public final NdkToolchainDescriptionArg.Builder setCxxToolchain​(BuildTarget cxxToolchain)
            ```

            ::: block
            Initializes the value for the
            [`cxxToolchain`](NdkToolchainDescriptionArg.html#getCxxToolchain())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `cxxToolchain` - The value for cxxToolchain

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSharedRuntimePath(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setSharedRuntimePath

            ``` methodSignature
            public final NdkToolchainDescriptionArg.Builder setSharedRuntimePath​(SourcePath sharedRuntimePath)
            ```

            ::: block
            Initializes the optional value
            [`sharedRuntimePath`](NdkToolchainDescriptionArg.html#getSharedRuntimePath())
            to sharedRuntimePath.
            :::

            [Parameters:]{.paramLabel}
            :   `sharedRuntimePath` - The value for sharedRuntimePath

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setSharedRuntimePath(java.util.Optional)}

        -   #### setSharedRuntimePath

            ``` methodSignature
            public final NdkToolchainDescriptionArg.Builder setSharedRuntimePath​(Optional<? extends SourcePath> sharedRuntimePath)
            ```

            ::: block
            Initializes the optional value
            [`sharedRuntimePath`](NdkToolchainDescriptionArg.html#getSharedRuntimePath())
            to sharedRuntimePath.
            :::

            [Parameters:]{.paramLabel}
            :   `sharedRuntimePath` - The value for sharedRuntimePath

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setObjdump(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setObjdump

            ``` methodSignature
            public final NdkToolchainDescriptionArg.Builder setObjdump​(SourcePath objdump)
            ```

            ::: block
            Initializes the value for the
            [`objdump`](NdkToolchainDescriptionArg.html#getObjdump())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `objdump` - The value for objdump

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCxxRuntime(com.facebook.buck.android.toolchain.ndk.NdkCxxRuntime)}

        -   #### setCxxRuntime

            ``` methodSignature
            public final NdkToolchainDescriptionArg.Builder setCxxRuntime​(NdkCxxRuntime cxxRuntime)
            ```

            ::: block
            Initializes the value for the
            [`cxxRuntime`](NdkToolchainDescriptionArg.html#getCxxRuntime())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `cxxRuntime` - The value for cxxRuntime

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setNdkPath(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setNdkPath

            ``` methodSignature
            public final NdkToolchainDescriptionArg.Builder setNdkPath​(SourcePath ndkPath)
            ```

            ::: block
            Initializes the optional value
            [`ndkPath`](NdkToolchainDescriptionArg.html#getNdkPath()) to
            ndkPath.
            :::

            [Parameters:]{.paramLabel}
            :   `ndkPath` - The value for ndkPath

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setNdkPath(java.util.Optional)}

        -   #### setNdkPath

            ``` methodSignature
            public final NdkToolchainDescriptionArg.Builder setNdkPath​(Optional<? extends SourcePath> ndkPath)
            ```

            ::: block
            Initializes the optional value
            [`ndkPath`](NdkToolchainDescriptionArg.html#getNdkPath()) to
            ndkPath.
            :::

            [Parameters:]{.paramLabel}
            :   `ndkPath` - The value for ndkPath

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final NdkToolchainDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](NdkToolchainDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final NdkToolchainDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](NdkToolchainDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final NdkToolchainDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](NdkToolchainDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final NdkToolchainDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](NdkToolchainDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String)}

        -   #### addLabels

            ``` methodSignature
            public final NdkToolchainDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](NdkToolchainDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final NdkToolchainDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](NdkToolchainDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final NdkToolchainDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](NdkToolchainDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final NdkToolchainDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](NdkToolchainDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final NdkToolchainDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](NdkToolchainDescriptionArg.html#getDefaultTargetPlatform())
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
            public final NdkToolchainDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](NdkToolchainDescriptionArg.html#getDefaultTargetPlatform())
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
            public final NdkToolchainDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](NdkToolchainDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final NdkToolchainDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](NdkToolchainDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final NdkToolchainDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](NdkToolchainDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final NdkToolchainDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](NdkToolchainDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final NdkToolchainDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](NdkToolchainDescriptionArg.html#getName())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public NdkToolchainDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`NdkToolchainDescriptionArg`](NdkToolchainDescriptionArg.html "class in com.facebook.buck.android").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of NdkToolchainDescriptionArg

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

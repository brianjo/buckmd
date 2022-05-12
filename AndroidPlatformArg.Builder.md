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
[Package]{.packageLabelInType} [com.facebook.buck.android.toolchain.platform](package-summary.html)
:::

## Class AndroidPlatformArg.Builder {#class-androidplatformarg.builder .title title="Class AndroidPlatformArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.toolchain.platform.AndroidPlatformArg.Builder

::: description
-   

    Enclosing class:
    :   [AndroidPlatformArg](AndroidPlatformArg.html "class in com.facebook.buck.android.toolchain.platform")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class AndroidPlatformArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`AndroidPlatformArg`](AndroidPlatformArg.html "class in com.facebook.buck.android.toolchain.platform").
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
        | `AndroidPlatformArg`  | `build()`             | ::: block             |
        |                       |                       | Builds a new          |
        |                       |                       | [`AndroidPlatformArg  |
        |                       |                       | `](AndroidPlatformArg |
        |                       |                       | .html "class in com.f |
        |                       |                       | acebook.buck.android. |
        |                       |                       | toolchain.platform"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Androi               | `from​(AndroidP        | ::: block             |
        | dPlatformArg.Builder` | latformArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `AndroidPlatformArg`  |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Androi               | `from​(com.            | ::: block             |
        | dPlatformArg.Builder` | facebook.buck.android | Copy abstract value   |
        |                       | .toolchain.platform.A | type                  |
        |                       | ndroidPlatformDescrip | `Abstra               |
        |                       | tion.AbstractAndroidP | ctAndroidPlatformArg` |
        |                       | latformArg instance)` | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Androi               | `from​(Cons            | ::: block             |
        | dPlatformArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Androi               | `putAllNati           | ::: block             |
        | dPlatformArg.Builder` | vePlatforms​(Map<? ext | Put all mappings from |
        |                       | ends TargetCpuType,​?  | the specified map as  |
        |                       | extends UnconfiguredB | entries to            |
        |                       | uildTarget> entries)` | [`                    |
        |                       |                       | nativePlatforms`](And |
        |                       |                       | roidPlatformArg.html# |
        |                       |                       | getNativePlatforms()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Androi               | `put                  | ::: block             |
        | dPlatformArg.Builder` | NativePlatforms​(Targe | Put one entry to the  |
        |                       | tCpuType key,         | [`                    |
        |                       |            Unconfigur | nativePlatforms`](And |
        |                       | edBuildTarget value)` | roidPlatformArg.html# |
        |                       |                       | getNativePlatforms()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Androi               | `putNativePl          | ::: block             |
        | dPlatformArg.Builder` | atforms​(Map.Entry<? e | Put one entry to the  |
        |                       | xtends TargetCpuType, | [`                    |
        |                       | ​? extends Unconfigure | nativePlatforms`](And |
        |                       | dBuildTarget> entry)` | roidPlatformArg.html# |
        |                       |                       | getNativePlatforms()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Androi               | `setBasePlatf         | ::: block             |
        | dPlatformArg.Builder` | orm​(UnconfiguredBuild | Initializes the value |
        |                       | Target basePlatform)` | for the               |
        |                       |                       | [`basePlatform`](     |
        |                       |                       | AndroidPlatformArg.ht |
        |                       |                       | ml#getBasePlatform()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Androi               | `                     | ::: block             |
        | dPlatformArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [                     |
        |                       |                       | `name`](AndroidPlatfo |
        |                       |                       | rmArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Androi               | `setNati              | ::: block             |
        | dPlatformArg.Builder` | vePlatforms​(Map<? ext | Sets or replaces all  |
        |                       | ends TargetCpuType,​?  | mappings from the     |
        |                       | extends UnconfiguredB | specified map as      |
        |                       | uildTarget> entries)` | entries for the       |
        |                       |                       | [`                    |
        |                       |                       | nativePlatforms`](And |
        |                       |                       | roidPlatformArg.html# |
        |                       |                       | getNativePlatforms()) |
        |                       |                       | map.                  |
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

        []{#from(com.facebook.buck.android.toolchain.platform.AndroidPlatformArg)}

        -   #### from

            ``` methodSignature
            public final AndroidPlatformArg.Builder from​(AndroidPlatformArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `AndroidPlatformArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.android.toolchain.platform.AndroidPlatformDescription.AbstractAndroidPlatformArg)}

        -   #### from

            ``` methodSignature
            public final AndroidPlatformArg.Builder from​(com.facebook.buck.android.toolchain.platform.AndroidPlatformDescription.AbstractAndroidPlatformArg instance)
            ```

            ::: block
            Copy abstract value type `AbstractAndroidPlatformArg`
            instance into builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.ConstructorArg)}

        -   #### from

            ``` methodSignature
            public final AndroidPlatformArg.Builder from​(ConstructorArg instance)
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

        []{#setBasePlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setBasePlatform

            ``` methodSignature
            public final AndroidPlatformArg.Builder setBasePlatform​(UnconfiguredBuildTarget basePlatform)
            ```

            ::: block
            Initializes the value for the
            [`basePlatform`](AndroidPlatformArg.html#getBasePlatform())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `basePlatform` - The value for basePlatform

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putNativePlatforms(com.facebook.buck.android.toolchain.ndk.TargetCpuType,com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### putNativePlatforms

            ``` methodSignature
            public final AndroidPlatformArg.Builder putNativePlatforms​(TargetCpuType key,
                                                                       UnconfiguredBuildTarget value)
            ```

            ::: block
            Put one entry to the
            [`nativePlatforms`](AndroidPlatformArg.html#getNativePlatforms())
            map.
            :::

            [Parameters:]{.paramLabel}
            :   `key` - The key in the nativePlatforms map
            :   `value` - The associated value in the nativePlatforms
                map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putNativePlatforms(java.util.Map.Entry)}

        -   #### putNativePlatforms

            ``` methodSignature
            public final AndroidPlatformArg.Builder putNativePlatforms​(Map.Entry<? extends TargetCpuType,​? extends UnconfiguredBuildTarget> entry)
            ```

            ::: block
            Put one entry to the
            [`nativePlatforms`](AndroidPlatformArg.html#getNativePlatforms())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setNativePlatforms(java.util.Map)}

        -   #### setNativePlatforms

            ``` methodSignature
            public final AndroidPlatformArg.Builder setNativePlatforms​(Map<? extends TargetCpuType,​? extends UnconfiguredBuildTarget> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`nativePlatforms`](AndroidPlatformArg.html#getNativePlatforms())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                nativePlatforms map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putAllNativePlatforms(java.util.Map)}

        -   #### putAllNativePlatforms

            ``` methodSignature
            public final AndroidPlatformArg.Builder putAllNativePlatforms​(Map<? extends TargetCpuType,​? extends UnconfiguredBuildTarget> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`nativePlatforms`](AndroidPlatformArg.html#getNativePlatforms())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                nativePlatforms map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final AndroidPlatformArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](AndroidPlatformArg.html#getName()) attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public AndroidPlatformArg build()
            ```

            ::: block
            Builds a new
            [`AndroidPlatformArg`](AndroidPlatformArg.html "class in com.facebook.buck.android.toolchain.platform").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of AndroidPlatformArg

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

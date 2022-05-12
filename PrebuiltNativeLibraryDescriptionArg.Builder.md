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

## Class PrebuiltNativeLibraryDescriptionArg.Builder {#class-prebuiltnativelibrarydescriptionarg.builder .title title="Class PrebuiltNativeLibraryDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.PrebuiltNativeLibraryDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [PrebuiltNativeLibraryDescriptionArg](PrebuiltNativeLibraryDescriptionArg.html "class in com.facebook.buck.android")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class PrebuiltNativeLibraryDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`PrebuiltNativeLibraryDescriptionArg`](PrebuiltNativeLibraryDescriptionArg.html "class in com.facebook.buck.android").
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
        | `Pr                   | `addAllCompat         | ::: block             |
        | ebuiltNativeLibraryDe | ibleWith​(Iterable<? e | Adds elements to      |
        | scriptionArg.Builder` | xtends UnconfiguredBu | [`compatibleWith`     |
        |                       | ildTarget> elements)` | ](PrebuiltNativeLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `addAllDeps​(          | ::: block             |
        | ebuiltNativeLibraryDe | Iterable<? extends Bu | Adds elements to      |
        | scriptionArg.Builder` | ildTarget> elements)` | [`deps`](PrebuiltN    |
        |                       |                       | ativeLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `addAllLabels​(Iterab  | ::: block             |
        | ebuiltNativeLibraryDe | le<String> elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [                     |
        |                       |                       | `labels`](PrebuiltNat |
        |                       |                       | iveLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `addAllLicenses       | ::: block             |
        | ebuiltNativeLibraryDe | ​(Iterable<? extends S | Adds elements to      |
        | scriptionArg.Builder` | ourcePath> elements)` | [`lic                 |
        |                       |                       | enses`](PrebuiltNativ |
        |                       |                       | eLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `addCompat            | ::: block             |
        | ebuiltNativeLibraryDe | ibleWith​(Unconfigured | Adds one element to   |
        | scriptionArg.Builder` | BuildTarget element)` | [`compatibleWith`     |
        |                       |                       | ](PrebuiltNativeLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `addCompatible        | ::: block             |
        | ebuiltNativeLibraryDe | With​(UnconfiguredBuil | Adds elements to      |
        | scriptionArg.Builder` | dTarget... elements)` | [`compatibleWith`     |
        |                       |                       | ](PrebuiltNativeLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `addDeps​(             | ::: block             |
        | ebuiltNativeLibraryDe | BuildTarget element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`deps`](PrebuiltN    |
        |                       |                       | ativeLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `addDeps​(Buil         | ::: block             |
        | ebuiltNativeLibraryDe | dTarget... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`deps`](PrebuiltN    |
        |                       |                       | ativeLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `addLa                | ::: block             |
        | ebuiltNativeLibraryDe | bels​(String element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [                     |
        |                       |                       | `labels`](PrebuiltNat |
        |                       |                       | iveLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `addLabels            | ::: block             |
        | ebuiltNativeLibraryDe | ​(String... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [                     |
        |                       |                       | `labels`](PrebuiltNat |
        |                       |                       | iveLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `addLicenses          | ::: block             |
        | ebuiltNativeLibraryDe | ​(SourcePath element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`lic                 |
        |                       |                       | enses`](PrebuiltNativ |
        |                       |                       | eLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `addLicenses​(Sou      | ::: block             |
        | ebuiltNativeLibraryDe | rcePath... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`lic                 |
        |                       |                       | enses`](PrebuiltNativ |
        |                       |                       | eLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltNativeL      | `build()`             | ::: block             |
        | ibraryDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`PrebuiltNati        |
        |                       |                       | veLibraryDescriptionA |
        |                       |                       | rg`](PrebuiltNativeLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml "class in com.fac |
        |                       |                       | ebook.buck.android"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `from​(com.face        | ::: block             |
        | ebuiltNativeLibraryDe | book.buck.android.Pre | Copy abstract value   |
        | scriptionArg.Builder` | builtNativeLibraryDes | type                  |
        |                       | cription.AbstractPreb | `Ab                   |
        |                       | uiltNativeLibraryDesc | stractPrebuiltNativeL |
        |                       | riptionArg instance)` | ibraryDescriptionArg` |
        |                       |                       | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `from​(Preb            | ::: block             |
        | ebuiltNativeLibraryDe | uiltNativeLibraryDesc | Fill a builder with   |
        | scriptionArg.Builder` | riptionArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `PrebuiltNativeL      |
        |                       |                       | ibraryDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `from​(Bu              | ::: block             |
        | ebuiltNativeLibraryDe | ildRuleArg instance)` | Fill a builder with   |
        | scriptionArg.Builder` |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `from​(Cons            | ::: block             |
        | ebuiltNativeLibraryDe | tructorArg instance)` | Fill a builder with   |
        | scriptionArg.Builder` |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `from​(HasDe           | ::: block             |
        | ebuiltNativeLibraryDe | claredDeps instance)` | Fill a builder with   |
        | scriptionArg.Builder` |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasDeclaredDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `setCompat            | ::: block             |
        | ebuiltNativeLibraryDe | ibleWith​(Iterable<? e | Sets or replaces all  |
        | scriptionArg.Builder` | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`compatibleWith`     |
        |                       |                       | ](PrebuiltNativeLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `setDefaul            | ::: block             |
        | ebuiltNativeLibraryDe | tTargetPlatform​(Uncon | Initializes the       |
        | scriptionArg.Builder` | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`defaultT            |
        |                       |                       | argetPlatform`](Prebu |
        |                       |                       | iltNativeLibraryDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `setDefau             | ::: block             |
        | ebuiltNativeLibraryDe | ltTargetPlatform​(Opti | Initializes the       |
        | scriptionArg.Builder` | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`defaultT            |
        |                       | faultTargetPlatform)` | argetPlatform`](Prebu |
        |                       |                       | iltNativeLibraryDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `setDeps​(             | ::: block             |
        | ebuiltNativeLibraryDe | Iterable<? extends Bu | Sets or replaces all  |
        | scriptionArg.Builder` | ildTarget> elements)` | elements for          |
        |                       |                       | [`deps`](PrebuiltN    |
        |                       |                       | ativeLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `setIsAs              | ::: block             |
        | ebuiltNativeLibraryDe | set​(boolean isAsset)` | Initializes the value |
        | scriptionArg.Builder` |                       | for the               |
        |                       |                       | [`i                   |
        |                       |                       | sAsset`](PrebuiltNati |
        |                       |                       | veLibraryDescriptionA |
        |                       |                       | rg.html#getIsAsset()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `setLabels​(Iterab     | ::: block             |
        | ebuiltNativeLibraryDe | le<String> elements)` | Sets or replaces all  |
        | scriptionArg.Builder` |                       | elements for          |
        |                       |                       | [                     |
        |                       |                       | `labels`](PrebuiltNat |
        |                       |                       | iveLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `setLicenses          | ::: block             |
        | ebuiltNativeLibraryDe | ​(Iterable<? extends S | Sets or replaces all  |
        | scriptionArg.Builder` | ourcePath> elements)` | elements for          |
        |                       |                       | [`lic                 |
        |                       |                       | enses`](PrebuiltNativ |
        |                       |                       | eLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `                     | ::: block             |
        | ebuiltNativeLibraryDe | setName​(String name)` | Initializes the value |
        | scriptionArg.Builder` |                       | for the               |
        |                       |                       | [`name`](PrebuiltN    |
        |                       |                       | ativeLibraryDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `setNativeL           | ::: block             |
        | ebuiltNativeLibraryDe | ibs​(Path nativeLibs)` | Initializes the value |
        | scriptionArg.Builder` |                       | for the               |
        |                       |                       | [`nativeL             |
        |                       |                       | ibs`](PrebuiltNativeL |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getNativeLibs()) |
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

        []{#from(com.facebook.buck.core.description.arg.HasDeclaredDeps)}

        -   #### from

            ``` methodSignature
            public final PrebuiltNativeLibraryDescriptionArg.Builder from​(HasDeclaredDeps instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.core.description.arg.HasDeclaredDeps`
            instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.BuildRuleArg)}

        -   #### from

            ``` methodSignature
            public final PrebuiltNativeLibraryDescriptionArg.Builder from​(BuildRuleArg instance)
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
            public final PrebuiltNativeLibraryDescriptionArg.Builder from​(ConstructorArg instance)
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

        []{#from(com.facebook.buck.android.PrebuiltNativeLibraryDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final PrebuiltNativeLibraryDescriptionArg.Builder from​(PrebuiltNativeLibraryDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `PrebuiltNativeLibraryDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.android.PrebuiltNativeLibraryDescription.AbstractPrebuiltNativeLibraryDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final PrebuiltNativeLibraryDescriptionArg.Builder from​(com.facebook.buck.android.PrebuiltNativeLibraryDescription.AbstractPrebuiltNativeLibraryDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type
            `AbstractPrebuiltNativeLibraryDescriptionArg` instance into
            builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setIsAsset(boolean)}

        -   #### setIsAsset

            ``` methodSignature
            public final PrebuiltNativeLibraryDescriptionArg.Builder setIsAsset​(boolean isAsset)
            ```

            ::: block
            Initializes the value for the
            [`isAsset`](PrebuiltNativeLibraryDescriptionArg.html#getIsAsset())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`isAsset`](PrebuiltNativeLibraryDescriptionArg.html#getIsAsset()).*
            :::

            [Parameters:]{.paramLabel}
            :   `isAsset` - The value for isAsset

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setNativeLibs(java.nio.file.Path)}

        -   #### setNativeLibs

            ``` methodSignature
            public final PrebuiltNativeLibraryDescriptionArg.Builder setNativeLibs​(Path nativeLibs)
            ```

            ::: block
            Initializes the value for the
            [`nativeLibs`](PrebuiltNativeLibraryDescriptionArg.html#getNativeLibs())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `nativeLibs` - The value for nativeLibs

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final PrebuiltNativeLibraryDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](PrebuiltNativeLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final PrebuiltNativeLibraryDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](PrebuiltNativeLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final PrebuiltNativeLibraryDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](PrebuiltNativeLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final PrebuiltNativeLibraryDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](PrebuiltNativeLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String)}

        -   #### addLabels

            ``` methodSignature
            public final PrebuiltNativeLibraryDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](PrebuiltNativeLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final PrebuiltNativeLibraryDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](PrebuiltNativeLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final PrebuiltNativeLibraryDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](PrebuiltNativeLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final PrebuiltNativeLibraryDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](PrebuiltNativeLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final PrebuiltNativeLibraryDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](PrebuiltNativeLibraryDescriptionArg.html#getDefaultTargetPlatform())
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
            public final PrebuiltNativeLibraryDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](PrebuiltNativeLibraryDescriptionArg.html#getDefaultTargetPlatform())
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
            public final PrebuiltNativeLibraryDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](PrebuiltNativeLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final PrebuiltNativeLibraryDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](PrebuiltNativeLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final PrebuiltNativeLibraryDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](PrebuiltNativeLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final PrebuiltNativeLibraryDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](PrebuiltNativeLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final PrebuiltNativeLibraryDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](PrebuiltNativeLibraryDescriptionArg.html#getName())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addDeps

            ``` methodSignature
            public final PrebuiltNativeLibraryDescriptionArg.Builder addDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`deps`](PrebuiltNativeLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A deps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addDeps

            ``` methodSignature
            public final PrebuiltNativeLibraryDescriptionArg.Builder addDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`deps`](PrebuiltNativeLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDeps(java.lang.Iterable)}

        -   #### setDeps

            ``` methodSignature
            public final PrebuiltNativeLibraryDescriptionArg.Builder setDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`deps`](PrebuiltNativeLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllDeps(java.lang.Iterable)}

        -   #### addAllDeps

            ``` methodSignature
            public final PrebuiltNativeLibraryDescriptionArg.Builder addAllDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`deps`](PrebuiltNativeLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public PrebuiltNativeLibraryDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`PrebuiltNativeLibraryDescriptionArg`](PrebuiltNativeLibraryDescriptionArg.html "class in com.facebook.buck.android").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of
                PrebuiltNativeLibraryDescriptionArg

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

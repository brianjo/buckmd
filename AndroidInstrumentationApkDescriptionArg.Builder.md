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

## Class AndroidInstrumentationApkDescriptionArg.Builder {#class-androidinstrumentationapkdescriptionarg.builder .title title="Class AndroidInstrumentationApkDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.AndroidInstrumentationApkDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [AndroidInstrumentationApkDescriptionArg](AndroidInstrumentationApkDescriptionArg.html "class in com.facebook.buck.android")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class AndroidInstrumentationApkDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`AndroidInstrumentationApkDescriptionArg`](AndroidInstrumentationApkDescriptionArg.html "class in com.facebook.buck.android").
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
        | `Androi               | `addAllCompat         | ::: block             |
        | dInstrumentationApkDe | ibleWith​(Iterable<? e | Adds elements to      |
        | scriptionArg.Builder` | xtends UnconfiguredBu | [`compatibleWith`](An |
        |                       | ildTarget> elements)` | droidInstrumentationA |
        |                       |                       | pkDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Androi               | `addAllDeps​(          | ::: block             |
        | dInstrumentationApkDe | Iterable<? extends Bu | Adds elements to      |
        | scriptionArg.Builder` | ildTarget> elements)` | [                     |
        |                       |                       | `deps`](AndroidInstru |
        |                       |                       | mentationApkDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Androi               | `addAllLabels​(Iterab  | ::: block             |
        | dInstrumentationApkDe | le<String> elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`lab                 |
        |                       |                       | els`](AndroidInstrume |
        |                       |                       | ntationApkDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Androi               | `addAllLicenses       | ::: block             |
        | dInstrumentationApkDe | ​(Iterable<? extends S | Adds elements to      |
        | scriptionArg.Builder` | ourcePath> elements)` | [`license             |
        |                       |                       | s`](AndroidInstrument |
        |                       |                       | ationApkDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Androi               | `addCompat            | ::: block             |
        | dInstrumentationApkDe | ibleWith​(Unconfigured | Adds one element to   |
        | scriptionArg.Builder` | BuildTarget element)` | [`compatibleWith`](An |
        |                       |                       | droidInstrumentationA |
        |                       |                       | pkDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Androi               | `addCompatible        | ::: block             |
        | dInstrumentationApkDe | With​(UnconfiguredBuil | Adds elements to      |
        | scriptionArg.Builder` | dTarget... elements)` | [`compatibleWith`](An |
        |                       |                       | droidInstrumentationA |
        |                       |                       | pkDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Androi               | `addDeps​(             | ::: block             |
        | dInstrumentationApkDe | BuildTarget element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [                     |
        |                       |                       | `deps`](AndroidInstru |
        |                       |                       | mentationApkDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Androi               | `addDeps​(Buil         | ::: block             |
        | dInstrumentationApkDe | dTarget... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [                     |
        |                       |                       | `deps`](AndroidInstru |
        |                       |                       | mentationApkDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Androi               | `addLa                | ::: block             |
        | dInstrumentationApkDe | bels​(String element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`lab                 |
        |                       |                       | els`](AndroidInstrume |
        |                       |                       | ntationApkDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Androi               | `addLabels            | ::: block             |
        | dInstrumentationApkDe | ​(String... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`lab                 |
        |                       |                       | els`](AndroidInstrume |
        |                       |                       | ntationApkDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Androi               | `addLicenses          | ::: block             |
        | dInstrumentationApkDe | ​(SourcePath element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`license             |
        |                       |                       | s`](AndroidInstrument |
        |                       |                       | ationApkDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Androi               | `addLicenses​(Sou      | ::: block             |
        | dInstrumentationApkDe | rcePath... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`license             |
        |                       |                       | s`](AndroidInstrument |
        |                       |                       | ationApkDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidInstrumentat  | `build()`             | ::: block             |
        | ionApkDescriptionArg` |                       | Builds a new          |
        |                       |                       | [                     |
        |                       |                       | `AndroidInstrumentati |
        |                       |                       | onApkDescriptionArg`] |
        |                       |                       | (AndroidInstrumentati |
        |                       |                       | onApkDescriptionArg.h |
        |                       |                       | tml "class in com.fac |
        |                       |                       | ebook.buck.android"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Androi               | `                     | ::: block             |
        | dInstrumentationApkDe | from​(com.facebook.buc | Copy abstract value   |
        | scriptionArg.Builder` | k.android.AndroidInst | type                  |
        |                       | rumentationApkDescrip | `Abstra               |
        |                       | tion.AbstractAndroidI | ctAndroidInstrumentat |
        |                       | nstrumentationApkDesc | ionApkDescriptionArg` |
        |                       | riptionArg instance)` | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Androi               | `from​(AndroidI        | ::: block             |
        | dInstrumentationApkDe | nstrumentationApkDesc | Fill a builder with   |
        | scriptionArg.Builder` | riptionArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `AndroidInstrumentat  |
        |                       |                       | ionApkDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Androi               | `from​(Bu              | ::: block             |
        | dInstrumentationApkDe | ildRuleArg instance)` | Fill a builder with   |
        | scriptionArg.Builder` |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Androi               | `from​(Cons            | ::: block             |
        | dInstrumentationApkDe | tructorArg instance)` | Fill a builder with   |
        | scriptionArg.Builder` |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Androi               | `from​(HasDe           | ::: block             |
        | dInstrumentationApkDe | claredDeps instance)` | Fill a builder with   |
        | scriptionArg.Builder` |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasDeclaredDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Androi               | `setAaptMode​(com      | ::: block             |
        | dInstrumentationApkDe | .facebook.buck.androi | Initializes the value |
        | scriptionArg.Builder` | d.AaptMode aaptMode)` | for the               |
        |                       |                       | [`aaptMod             |
        |                       |                       | e`](AndroidInstrument |
        |                       |                       | ationApkDescriptionAr |
        |                       |                       | g.html#getAaptMode()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Androi               | `set                  | ::: block             |
        | dInstrumentationApkDe | Apk​(BuildTarget apk)` | Initializes the value |
        | scriptionArg.Builder` |                       | for the               |
        |                       |                       | [`apk`](AndroidInstr  |
        |                       |                       | umentationApkDescript |
        |                       |                       | ionArg.html#getApk()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Androi               | `setCompat            | ::: block             |
        | dInstrumentationApkDe | ibleWith​(Iterable<? e | Sets or replaces all  |
        | scriptionArg.Builder` | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`compatibleWith`](An |
        |                       |                       | droidInstrumentationA |
        |                       |                       | pkDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Androi               | `setDefaul            | ::: block             |
        | dInstrumentationApkDe | tTargetPlatform​(Uncon | Initializes the       |
        | scriptionArg.Builder` | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`defaultTarge        |
        |                       |                       | tPlatform`](AndroidIn |
        |                       |                       | strumentationApkDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Androi               | `setDefau             | ::: block             |
        | dInstrumentationApkDe | ltTargetPlatform​(Opti | Initializes the       |
        | scriptionArg.Builder` | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`defaultTarge        |
        |                       | faultTargetPlatform)` | tPlatform`](AndroidIn |
        |                       |                       | strumentationApkDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Androi               | `setDeps​(             | ::: block             |
        | dInstrumentationApkDe | Iterable<? extends Bu | Sets or replaces all  |
        | scriptionArg.Builder` | ildTarget> elements)` | elements for          |
        |                       |                       | [                     |
        |                       |                       | `deps`](AndroidInstru |
        |                       |                       | mentationApkDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Androi               | `setDex               | ::: block             |
        | dInstrumentationApkDe | Tool​(String dexTool)` | Initializes the value |
        | scriptionArg.Builder` |                       | for the               |
        |                       |                       | [`dexTo               |
        |                       |                       | ol`](AndroidInstrumen |
        |                       |                       | tationApkDescriptionA |
        |                       |                       | rg.html#getDexTool()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Androi               | `setIncludesVectorD   | ::: block             |
        | dInstrumentationApkDe | rawables​(boolean incl | Initializes the value |
        | scriptionArg.Builder` | udesVectorDrawables)` | for the               |
        |                       |                       | [`includesVectorDr    |
        |                       |                       | awables`](AndroidInst |
        |                       |                       | rumentationApkDescrip |
        |                       |                       | tionArg.html#getInclu |
        |                       |                       | desVectorDrawables()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Androi               | `setLabels​(Iterab     | ::: block             |
        | dInstrumentationApkDe | le<String> elements)` | Sets or replaces all  |
        | scriptionArg.Builder` |                       | elements for          |
        |                       |                       | [`lab                 |
        |                       |                       | els`](AndroidInstrume |
        |                       |                       | ntationApkDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Androi               | `setLicenses          | ::: block             |
        | dInstrumentationApkDe | ​(Iterable<? extends S | Sets or replaces all  |
        | scriptionArg.Builder` | ourcePath> elements)` | elements for          |
        |                       |                       | [`license             |
        |                       |                       | s`](AndroidInstrument |
        |                       |                       | ationApkDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Androi               | `setManifest​(         | ::: block             |
        | dInstrumentationApkDe | SourcePath manifest)` | Initializes the       |
        | scriptionArg.Builder` |                       | optional value        |
        |                       |                       | [`manifes             |
        |                       |                       | t`](AndroidInstrument |
        |                       |                       | ationApkDescriptionAr |
        |                       |                       | g.html#getManifest()) |
        |                       |                       | to manifest.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Androi               | `setManifest          | ::: block             |
        | dInstrumentationApkDe | ​(Optional<? extends S | Initializes the       |
        | scriptionArg.Builder` | ourcePath> manifest)` | optional value        |
        |                       |                       | [`manifes             |
        |                       |                       | t`](AndroidInstrument |
        |                       |                       | ationApkDescriptionAr |
        |                       |                       | g.html#getManifest()) |
        |                       |                       | to manifest.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Androi               | `setMani              | ::: block             |
        | dInstrumentationApkDe | festSkeleton​(SourcePa | Initializes the       |
        | scriptionArg.Builder` | th manifestSkeleton)` | optional value        |
        |                       |                       | [`ma                  |
        |                       |                       | nifestSkeleton`](Andr |
        |                       |                       | oidInstrumentationApk |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etManifestSkeleton()) |
        |                       |                       | to manifestSkeleton.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Androi               | `setMan               | ::: block             |
        | dInstrumentationApkDe | ifestSkeleton​(Optiona | Initializes the       |
        | scriptionArg.Builder` | l<? extends SourcePat | optional value        |
        |                       | h> manifestSkeleton)` | [`ma                  |
        |                       |                       | nifestSkeleton`](Andr |
        |                       |                       | oidInstrumentationApk |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etManifestSkeleton()) |
        |                       |                       | to manifestSkeleton.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Androi               | `                     | ::: block             |
        | dInstrumentationApkDe | setName​(String name)` | Initializes the value |
        | scriptionArg.Builder` |                       | for the               |
        |                       |                       | [                     |
        |                       |                       | `name`](AndroidInstru |
        |                       |                       | mentationApkDescripti |
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

        []{#from(com.facebook.buck.core.description.arg.HasDeclaredDeps)}

        -   #### from

            ``` methodSignature
            public final AndroidInstrumentationApkDescriptionArg.Builder from​(HasDeclaredDeps instance)
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
            public final AndroidInstrumentationApkDescriptionArg.Builder from​(BuildRuleArg instance)
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

        []{#from(com.facebook.buck.android.AndroidInstrumentationApkDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final AndroidInstrumentationApkDescriptionArg.Builder from​(AndroidInstrumentationApkDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `AndroidInstrumentationApkDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.android.AndroidInstrumentationApkDescription.AbstractAndroidInstrumentationApkDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final AndroidInstrumentationApkDescriptionArg.Builder from​(com.facebook.buck.android.AndroidInstrumentationApkDescription.AbstractAndroidInstrumentationApkDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type
            `AbstractAndroidInstrumentationApkDescriptionArg` instance
            into builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.ConstructorArg)}

        -   #### from

            ``` methodSignature
            public final AndroidInstrumentationApkDescriptionArg.Builder from​(ConstructorArg instance)
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

        []{#setManifest(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setManifest

            ``` methodSignature
            public final AndroidInstrumentationApkDescriptionArg.Builder setManifest​(SourcePath manifest)
            ```

            ::: block
            Initializes the optional value
            [`manifest`](AndroidInstrumentationApkDescriptionArg.html#getManifest())
            to manifest.
            :::

            [Parameters:]{.paramLabel}
            :   `manifest` - The value for manifest

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setManifest(java.util.Optional)}

        -   #### setManifest

            ``` methodSignature
            public final AndroidInstrumentationApkDescriptionArg.Builder setManifest​(Optional<? extends SourcePath> manifest)
            ```

            ::: block
            Initializes the optional value
            [`manifest`](AndroidInstrumentationApkDescriptionArg.html#getManifest())
            to manifest.
            :::

            [Parameters:]{.paramLabel}
            :   `manifest` - The value for manifest

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setManifestSkeleton(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setManifestSkeleton

            ``` methodSignature
            public final AndroidInstrumentationApkDescriptionArg.Builder setManifestSkeleton​(SourcePath manifestSkeleton)
            ```

            ::: block
            Initializes the optional value
            [`manifestSkeleton`](AndroidInstrumentationApkDescriptionArg.html#getManifestSkeleton())
            to manifestSkeleton.
            :::

            [Parameters:]{.paramLabel}
            :   `manifestSkeleton` - The value for manifestSkeleton

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setManifestSkeleton(java.util.Optional)}

        -   #### setManifestSkeleton

            ``` methodSignature
            public final AndroidInstrumentationApkDescriptionArg.Builder setManifestSkeleton​(Optional<? extends SourcePath> manifestSkeleton)
            ```

            ::: block
            Initializes the optional value
            [`manifestSkeleton`](AndroidInstrumentationApkDescriptionArg.html#getManifestSkeleton())
            to manifestSkeleton.
            :::

            [Parameters:]{.paramLabel}
            :   `manifestSkeleton` - The value for manifestSkeleton

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setApk(com.facebook.buck.core.model.BuildTarget)}

        -   #### setApk

            ``` methodSignature
            public final AndroidInstrumentationApkDescriptionArg.Builder setApk​(BuildTarget apk)
            ```

            ::: block
            Initializes the value for the
            [`apk`](AndroidInstrumentationApkDescriptionArg.html#getApk())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `apk` - The value for apk

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAaptMode(com.facebook.buck.android.AaptMode)}

        -   #### setAaptMode

            ``` methodSignature
            public final AndroidInstrumentationApkDescriptionArg.Builder setAaptMode​(com.facebook.buck.android.AaptMode aaptMode)
            ```

            ::: block
            Initializes the value for the
            [`aaptMode`](AndroidInstrumentationApkDescriptionArg.html#getAaptMode())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`aaptMode`](AndroidInstrumentationApkDescriptionArg.html#getAaptMode()).*
            :::

            [Parameters:]{.paramLabel}
            :   `aaptMode` - The value for aaptMode

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setIncludesVectorDrawables(boolean)}

        -   #### setIncludesVectorDrawables

            ``` methodSignature
            public final AndroidInstrumentationApkDescriptionArg.Builder setIncludesVectorDrawables​(boolean includesVectorDrawables)
            ```

            ::: block
            Initializes the value for the
            [`includesVectorDrawables`](AndroidInstrumentationApkDescriptionArg.html#getIncludesVectorDrawables())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`includesVectorDrawables`](AndroidInstrumentationApkDescriptionArg.html#getIncludesVectorDrawables()).*
            :::

            [Parameters:]{.paramLabel}
            :   `includesVectorDrawables` - The value for
                includesVectorDrawables

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDexTool(java.lang.String)}

        -   #### setDexTool

            ``` methodSignature
            public final AndroidInstrumentationApkDescriptionArg.Builder setDexTool​(String dexTool)
            ```

            ::: block
            Initializes the value for the
            [`dexTool`](AndroidInstrumentationApkDescriptionArg.html#getDexTool())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`dexTool`](AndroidInstrumentationApkDescriptionArg.html#getDexTool()).*
            :::

            [Parameters:]{.paramLabel}
            :   `dexTool` - The value for dexTool

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final AndroidInstrumentationApkDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](AndroidInstrumentationApkDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final AndroidInstrumentationApkDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](AndroidInstrumentationApkDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final AndroidInstrumentationApkDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](AndroidInstrumentationApkDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final AndroidInstrumentationApkDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](AndroidInstrumentationApkDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String)}

        -   #### addLabels

            ``` methodSignature
            public final AndroidInstrumentationApkDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](AndroidInstrumentationApkDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final AndroidInstrumentationApkDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](AndroidInstrumentationApkDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final AndroidInstrumentationApkDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](AndroidInstrumentationApkDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final AndroidInstrumentationApkDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](AndroidInstrumentationApkDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final AndroidInstrumentationApkDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](AndroidInstrumentationApkDescriptionArg.html#getDefaultTargetPlatform())
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
            public final AndroidInstrumentationApkDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](AndroidInstrumentationApkDescriptionArg.html#getDefaultTargetPlatform())
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
            public final AndroidInstrumentationApkDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](AndroidInstrumentationApkDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final AndroidInstrumentationApkDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](AndroidInstrumentationApkDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final AndroidInstrumentationApkDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](AndroidInstrumentationApkDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final AndroidInstrumentationApkDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](AndroidInstrumentationApkDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final AndroidInstrumentationApkDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](AndroidInstrumentationApkDescriptionArg.html#getName())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addDeps

            ``` methodSignature
            public final AndroidInstrumentationApkDescriptionArg.Builder addDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`deps`](AndroidInstrumentationApkDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A deps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addDeps

            ``` methodSignature
            public final AndroidInstrumentationApkDescriptionArg.Builder addDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`deps`](AndroidInstrumentationApkDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDeps(java.lang.Iterable)}

        -   #### setDeps

            ``` methodSignature
            public final AndroidInstrumentationApkDescriptionArg.Builder setDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`deps`](AndroidInstrumentationApkDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllDeps(java.lang.Iterable)}

        -   #### addAllDeps

            ``` methodSignature
            public final AndroidInstrumentationApkDescriptionArg.Builder addAllDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`deps`](AndroidInstrumentationApkDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public AndroidInstrumentationApkDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`AndroidInstrumentationApkDescriptionArg`](AndroidInstrumentationApkDescriptionArg.html "class in com.facebook.buck.android").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of
                AndroidInstrumentationApkDescriptionArg

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

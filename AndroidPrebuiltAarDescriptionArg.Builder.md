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

## Class AndroidPrebuiltAarDescriptionArg.Builder {#class-androidprebuiltaardescriptionarg.builder .title title="Class AndroidPrebuiltAarDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.AndroidPrebuiltAarDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [AndroidPrebuiltAarDescriptionArg](AndroidPrebuiltAarDescriptionArg.html "class in com.facebook.buck.android")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class AndroidPrebuiltAarDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`AndroidPrebuiltAarDescriptionArg`](AndroidPrebuiltAarDescriptionArg.html "class in com.facebook.buck.android").
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
        | `AndroidPrebuiltAarDe | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`compatibleWi        |
        |                       | ildTarget> elements)` | th`](AndroidPrebuiltA |
        |                       |                       | arDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidPrebuiltAarDe | `addAllDeps​(          | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`deps`](Androi       |
        |                       |                       | dPrebuiltAarDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidPrebuiltAarDe | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels`](AndroidP   |
        |                       |                       | rebuiltAarDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidPrebuiltAarDe | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`                    |
        |                       |                       | licenses`](AndroidPre |
        |                       |                       | builtAarDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidPrebuiltAarDe | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`compatibleWi        |
        |                       |                       | th`](AndroidPrebuiltA |
        |                       |                       | arDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidPrebuiltAarDe | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`compatibleWi        |
        |                       |                       | th`](AndroidPrebuiltA |
        |                       |                       | arDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidPrebuiltAarDe | `addDeps​(             | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`deps`](Androi       |
        |                       |                       | dPrebuiltAarDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidPrebuiltAarDe | `addDeps​(Buil         | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`deps`](Androi       |
        |                       |                       | dPrebuiltAarDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidPrebuiltAarDe | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels`](AndroidP   |
        |                       |                       | rebuiltAarDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidPrebuiltAarDe | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels`](AndroidP   |
        |                       |                       | rebuiltAarDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidPrebuiltAarDe | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`                    |
        |                       |                       | licenses`](AndroidPre |
        |                       |                       | builtAarDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidPrebuiltAarDe | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`                    |
        |                       |                       | licenses`](AndroidPre |
        |                       |                       | builtAarDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidPrebu         | `build()`             | ::: block             |
        | iltAarDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`Androi              |
        |                       |                       | dPrebuiltAarDescripti |
        |                       |                       | onArg`](AndroidPrebui |
        |                       |                       | ltAarDescriptionArg.h |
        |                       |                       | tml "class in com.fac |
        |                       |                       | ebook.buck.android"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidPrebuiltAarDe | `from​(co              | ::: block             |
        | scriptionArg.Builder` | m.facebook.buck.andro | Copy abstract value   |
        |                       | id.AndroidPrebuiltAar | type                  |
        |                       | Description.AbstractA | `AbstractAndroidPrebu |
        |                       | ndroidPrebuiltAarDesc | iltAarDescriptionArg` |
        |                       | riptionArg instance)` | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidPrebuiltAarDe | `from​(A               | ::: block             |
        | scriptionArg.Builder` | ndroidPrebuiltAarDesc | Fill a builder with   |
        |                       | riptionArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `AndroidPrebu         |
        |                       |                       | iltAarDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidPrebuiltAarDe | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidPrebuiltAarDe | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidPrebuiltAarDe | `from​(HasDe           | ::: block             |
        | scriptionArg.Builder` | claredDeps instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasDeclaredDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidPrebuiltAarDe | `from​(M               | ::: block             |
        | scriptionArg.Builder` | aybeRequiredForSource | Fill a builder with   |
        |                       | OnlyAbiArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buck.   |
        |                       |                       | jvm.java.MaybeRequire |
        |                       |                       | dForSourceOnlyAbiArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidPrebuiltAarDe | `se                   | ::: block             |
        | scriptionArg.Builder` | tAar​(SourcePath aar)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`aar`](Andro         |
        |                       |                       | idPrebuiltAarDescript |
        |                       |                       | ionArg.html#getAar()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidPrebuiltAarDe | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`compatibleWi        |
        |                       |                       | th`](AndroidPrebuiltA |
        |                       |                       | arDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidPrebuiltAarDe | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`defau               |
        |                       |                       | ltTargetPlatform`](An |
        |                       |                       | droidPrebuiltAarDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidPrebuiltAarDe | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`defau               |
        |                       | faultTargetPlatform)` | ltTargetPlatform`](An |
        |                       |                       | droidPrebuiltAarDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidPrebuiltAarDe | `setDeps​(             | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`deps`](Androi       |
        |                       |                       | dPrebuiltAarDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidPrebuiltAarDe | `setJavadocUr         | ::: block             |
        | scriptionArg.Builder` | l​(String javadocUrl)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`java                |
        |                       |                       | docUrl`](AndroidPrebu |
        |                       |                       | iltAarDescriptionArg. |
        |                       |                       | html#getJavadocUrl()) |
        |                       |                       | to javadocUrl.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidPrebuiltAarDe | `s                    | ::: block             |
        | scriptionArg.Builder` | etJavadocUrl​(Optional | Initializes the       |
        |                       | <String> javadocUrl)` | optional value        |
        |                       |                       | [`java                |
        |                       |                       | docUrl`](AndroidPrebu |
        |                       |                       | iltAarDescriptionArg. |
        |                       |                       | html#getJavadocUrl()) |
        |                       |                       | to javadocUrl.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidPrebuiltAarDe | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels`](AndroidP   |
        |                       |                       | rebuiltAarDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidPrebuiltAarDe | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`                    |
        |                       |                       | licenses`](AndroidPre |
        |                       |                       | builtAarDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidPrebuiltAarDe | `setMavenCoords       | ::: block             |
        | scriptionArg.Builder` | ​(String mavenCoords)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`mavenC              |
        |                       |                       | oords`](AndroidPrebui |
        |                       |                       | ltAarDescriptionArg.h |
        |                       |                       | tml#getMavenCoords()) |
        |                       |                       | to mavenCoords.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidPrebuiltAarDe | `set                  | ::: block             |
        | scriptionArg.Builder` | MavenCoords​(Optional< | Initializes the       |
        |                       | String> mavenCoords)` | optional value        |
        |                       |                       | [`mavenC              |
        |                       |                       | oords`](AndroidPrebui |
        |                       |                       | ltAarDescriptionArg.h |
        |                       |                       | tml#getMavenCoords()) |
        |                       |                       | to mavenCoords.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidPrebuiltAarDe | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`name`](Androi       |
        |                       |                       | dPrebuiltAarDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidPrebuiltAarDe | `setRequiredForSource | ::: block             |
        | scriptionArg.Builder` | OnlyAbi​(boolean requi | Initializes the value |
        |                       | redForSourceOnlyAbi)` | for the               |
        |                       |                       | [`requiredFor         |
        |                       |                       | SourceOnlyAbi`](Andro |
        |                       |                       | idPrebuiltAarDescript |
        |                       |                       | ionArg.html#getRequir |
        |                       |                       | edForSourceOnlyAbi()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidPrebuiltAarDe | `setSourceJar​(S       | ::: block             |
        | scriptionArg.Builder` | ourcePath sourceJar)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`so                  |
        |                       |                       | urceJar`](AndroidPreb |
        |                       |                       | uiltAarDescriptionArg |
        |                       |                       | .html#getSourceJar()) |
        |                       |                       | to sourceJar.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidPrebuiltAarDe | `setSourceJar​(        | ::: block             |
        | scriptionArg.Builder` | Optional<? extends So | Initializes the       |
        |                       | urcePath> sourceJar)` | optional value        |
        |                       |                       | [`so                  |
        |                       |                       | urceJar`](AndroidPreb |
        |                       |                       | uiltAarDescriptionArg |
        |                       |                       | .html#getSourceJar()) |
        |                       |                       | to sourceJar.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidPrebuiltAarDe | `setUseSystemLibr     | ::: block             |
        | scriptionArg.Builder` | aryLoader​(boolean use | Initializes the value |
        |                       | SystemLibraryLoader)` | for the               |
        |                       |                       | [`useSys              |
        |                       |                       | temLibraryLoader`](An |
        |                       |                       | droidPrebuiltAarDescr |
        |                       |                       | iptionArg.html#isUseS |
        |                       |                       | ystemLibraryLoader()) |
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

        []{#from(com.facebook.buck.android.AndroidPrebuiltAarDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final AndroidPrebuiltAarDescriptionArg.Builder from​(AndroidPrebuiltAarDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `AndroidPrebuiltAarDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.android.AndroidPrebuiltAarDescription.AbstractAndroidPrebuiltAarDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final AndroidPrebuiltAarDescriptionArg.Builder from​(com.facebook.buck.android.AndroidPrebuiltAarDescription.AbstractAndroidPrebuiltAarDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type
            `AbstractAndroidPrebuiltAarDescriptionArg` instance into
            builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.HasDeclaredDeps)}

        -   #### from

            ``` methodSignature
            public final AndroidPrebuiltAarDescriptionArg.Builder from​(HasDeclaredDeps instance)
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
            public final AndroidPrebuiltAarDescriptionArg.Builder from​(BuildRuleArg instance)
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
            public final AndroidPrebuiltAarDescriptionArg.Builder from​(ConstructorArg instance)
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

        []{#from(com.facebook.buck.jvm.java.MaybeRequiredForSourceOnlyAbiArg)}

        -   #### from

            ``` methodSignature
            public final AndroidPrebuiltAarDescriptionArg.Builder from​(MaybeRequiredForSourceOnlyAbiArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.jvm.java.MaybeRequiredForSourceOnlyAbiArg`
            instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAar(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setAar

            ``` methodSignature
            public final AndroidPrebuiltAarDescriptionArg.Builder setAar​(SourcePath aar)
            ```

            ::: block
            Initializes the value for the
            [`aar`](AndroidPrebuiltAarDescriptionArg.html#getAar())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `aar` - The value for aar

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSourceJar(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setSourceJar

            ``` methodSignature
            public final AndroidPrebuiltAarDescriptionArg.Builder setSourceJar​(SourcePath sourceJar)
            ```

            ::: block
            Initializes the optional value
            [`sourceJar`](AndroidPrebuiltAarDescriptionArg.html#getSourceJar())
            to sourceJar.
            :::

            [Parameters:]{.paramLabel}
            :   `sourceJar` - The value for sourceJar

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setSourceJar(java.util.Optional)}

        -   #### setSourceJar

            ``` methodSignature
            public final AndroidPrebuiltAarDescriptionArg.Builder setSourceJar​(Optional<? extends SourcePath> sourceJar)
            ```

            ::: block
            Initializes the optional value
            [`sourceJar`](AndroidPrebuiltAarDescriptionArg.html#getSourceJar())
            to sourceJar.
            :::

            [Parameters:]{.paramLabel}
            :   `sourceJar` - The value for sourceJar

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setJavadocUrl(java.lang.String)}

        -   #### setJavadocUrl

            ``` methodSignature
            public final AndroidPrebuiltAarDescriptionArg.Builder setJavadocUrl​(String javadocUrl)
            ```

            ::: block
            Initializes the optional value
            [`javadocUrl`](AndroidPrebuiltAarDescriptionArg.html#getJavadocUrl())
            to javadocUrl.
            :::

            [Parameters:]{.paramLabel}
            :   `javadocUrl` - The value for javadocUrl

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setJavadocUrl(java.util.Optional)}

        -   #### setJavadocUrl

            ``` methodSignature
            public final AndroidPrebuiltAarDescriptionArg.Builder setJavadocUrl​(Optional<String> javadocUrl)
            ```

            ::: block
            Initializes the optional value
            [`javadocUrl`](AndroidPrebuiltAarDescriptionArg.html#getJavadocUrl())
            to javadocUrl.
            :::

            [Parameters:]{.paramLabel}
            :   `javadocUrl` - The value for javadocUrl

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setMavenCoords(java.lang.String)}

        -   #### setMavenCoords

            ``` methodSignature
            public final AndroidPrebuiltAarDescriptionArg.Builder setMavenCoords​(String mavenCoords)
            ```

            ::: block
            Initializes the optional value
            [`mavenCoords`](AndroidPrebuiltAarDescriptionArg.html#getMavenCoords())
            to mavenCoords.
            :::

            [Parameters:]{.paramLabel}
            :   `mavenCoords` - The value for mavenCoords

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setMavenCoords(java.util.Optional)}

        -   #### setMavenCoords

            ``` methodSignature
            public final AndroidPrebuiltAarDescriptionArg.Builder setMavenCoords​(Optional<String> mavenCoords)
            ```

            ::: block
            Initializes the optional value
            [`mavenCoords`](AndroidPrebuiltAarDescriptionArg.html#getMavenCoords())
            to mavenCoords.
            :::

            [Parameters:]{.paramLabel}
            :   `mavenCoords` - The value for mavenCoords

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRequiredForSourceOnlyAbi(boolean)}

        -   #### setRequiredForSourceOnlyAbi

            ``` methodSignature
            public final AndroidPrebuiltAarDescriptionArg.Builder setRequiredForSourceOnlyAbi​(boolean requiredForSourceOnlyAbi)
            ```

            ::: block
            Initializes the value for the
            [`requiredForSourceOnlyAbi`](AndroidPrebuiltAarDescriptionArg.html#getRequiredForSourceOnlyAbi())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`requiredForSourceOnlyAbi`](AndroidPrebuiltAarDescriptionArg.html#getRequiredForSourceOnlyAbi()).*
            :::

            [Parameters:]{.paramLabel}
            :   `requiredForSourceOnlyAbi` - The value for
                requiredForSourceOnlyAbi

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setUseSystemLibraryLoader(boolean)}

        -   #### setUseSystemLibraryLoader

            ``` methodSignature
            public final AndroidPrebuiltAarDescriptionArg.Builder setUseSystemLibraryLoader​(boolean useSystemLibraryLoader)
            ```

            ::: block
            Initializes the value for the
            [`useSystemLibraryLoader`](AndroidPrebuiltAarDescriptionArg.html#isUseSystemLibraryLoader())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`useSystemLibraryLoader`](AndroidPrebuiltAarDescriptionArg.html#isUseSystemLibraryLoader()).*
            :::

            [Parameters:]{.paramLabel}
            :   `useSystemLibraryLoader` - The value for
                useSystemLibraryLoader

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final AndroidPrebuiltAarDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](AndroidPrebuiltAarDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final AndroidPrebuiltAarDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](AndroidPrebuiltAarDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final AndroidPrebuiltAarDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](AndroidPrebuiltAarDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final AndroidPrebuiltAarDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](AndroidPrebuiltAarDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String)}

        -   #### addLabels

            ``` methodSignature
            public final AndroidPrebuiltAarDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](AndroidPrebuiltAarDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final AndroidPrebuiltAarDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](AndroidPrebuiltAarDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final AndroidPrebuiltAarDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](AndroidPrebuiltAarDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final AndroidPrebuiltAarDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](AndroidPrebuiltAarDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final AndroidPrebuiltAarDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](AndroidPrebuiltAarDescriptionArg.html#getDefaultTargetPlatform())
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
            public final AndroidPrebuiltAarDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](AndroidPrebuiltAarDescriptionArg.html#getDefaultTargetPlatform())
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
            public final AndroidPrebuiltAarDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](AndroidPrebuiltAarDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final AndroidPrebuiltAarDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](AndroidPrebuiltAarDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final AndroidPrebuiltAarDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](AndroidPrebuiltAarDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final AndroidPrebuiltAarDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](AndroidPrebuiltAarDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final AndroidPrebuiltAarDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](AndroidPrebuiltAarDescriptionArg.html#getName())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addDeps

            ``` methodSignature
            public final AndroidPrebuiltAarDescriptionArg.Builder addDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`deps`](AndroidPrebuiltAarDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A deps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addDeps

            ``` methodSignature
            public final AndroidPrebuiltAarDescriptionArg.Builder addDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`deps`](AndroidPrebuiltAarDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDeps(java.lang.Iterable)}

        -   #### setDeps

            ``` methodSignature
            public final AndroidPrebuiltAarDescriptionArg.Builder setDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`deps`](AndroidPrebuiltAarDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllDeps(java.lang.Iterable)}

        -   #### addAllDeps

            ``` methodSignature
            public final AndroidPrebuiltAarDescriptionArg.Builder addAllDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`deps`](AndroidPrebuiltAarDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public AndroidPrebuiltAarDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`AndroidPrebuiltAarDescriptionArg`](AndroidPrebuiltAarDescriptionArg.html "class in com.facebook.buck.android").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of
                AndroidPrebuiltAarDescriptionArg

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

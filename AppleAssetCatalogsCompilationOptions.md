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
-   [Nested](#nested.class.summary) \| 
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

## Class AppleAssetCatalogsCompilationOptions {#class-appleassetcatalogscompilationoptions .title title="Class AppleAssetCatalogsCompilationOptions"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.AppleAssetCatalogsCompilationOptions

::: description
-   

    All Implemented Interfaces:
    :   `DataTransferObject`, `AddsToRuleKey`

    ------------------------------------------------------------------------

        @ParametersAreNonnullByDefault
        @Generated("org.immutables.processor.ProxyProcessor")
        @Immutable
        @CheckReturnValue
        public final class AppleAssetCatalogsCompilationOptions
        extends Object

    ::: block
    Argument type for asset_catalogs_compilation_options used in
    apple_bundle
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `App                  | ::: block             |
        |                       | leAssetCatalogsCompil | Builds instances of   |
        |                       | ationOptions.Builder` | type                  |
        |                       |                       | [`AppleAssetCa        |
        |                       |                       | talogsCompilationOpti |
        |                       |                       | ons`](AppleAssetCatal |
        |                       |                       | ogsCompilationOptions |
        |                       |                       | .html "class in com.f |
        |                       |                       | acebook.buck.apple"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static App           | `builder()`           | ::: block             |
        | leAssetCatalogsCompil |                       | Creates a builder for |
        | ationOptions.Builder` |                       | [`AppleAssetCa        |
        |                       |                       | talogsCompilationOpti |
        |                       |                       | ons`](AppleAssetCatal |
        |                       |                       | ogsCompilationOptions |
        |                       |                       | .html "class in com.f |
        |                       |                       | acebook.buck.apple"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `eq                   | ::: block             |
        |                       | uals​(Object another)` | This instance is      |
        |                       |                       | equal to all          |
        |                       |                       | instances of          |
        |                       |                       | `AppleAssetCatalo     |
        |                       |                       | gsCompilationOptions` |
        |                       |                       | that have equal       |
        |                       |                       | attribute values.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getCompressPngs()`   |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getErrors()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getExtraFlags()`     |                       |
        | ogle.common.collect.I |                       |                       |
        | mmutableList<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getNotices()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.facebook.buck.a  | `getOptimization()`   |                       |
        | pple.AbstractAppleAss |                       |                       |
        | etCatalogsCompilation |                       |                       |
        | Options.Optimization` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.facebook.buck.a  | `getOutputFormat()`   |                       |
        | pple.AbstractAppleAss |                       |                       |
        | etCatalogsCompilation |                       |                       |
        | Options.OutputFormat` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getWarnings()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          | ::: block             |
        |                       |                       | Computes a hash code  |
        |                       |                       | from attributes:      |
        |                       |                       | `notices`,            |
        |                       |                       | `warnings`, `errors`, |
        |                       |                       | `compressPngs`,       |
        |                       |                       | `optimization`,       |
        |                       |                       | `outputFormat`,       |
        |                       |                       | `extraFlags`.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          | ::: block             |
        |                       |                       | Prints the immutable  |
        |                       |                       | value                 |
        |                       |                       | `AppleAssetCatalo     |
        |                       |                       | gsCompilationOptions` |
        |                       |                       | with attribute        |
        |                       |                       | values.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getNotices()}

        -   #### getNotices

            ``` methodSignature
            public boolean getNotices()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `notices` attribute

        []{#getWarnings()}

        -   #### getWarnings

            ``` methodSignature
            public boolean getWarnings()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `warnings` attribute

        []{#getErrors()}

        -   #### getErrors

            ``` methodSignature
            public boolean getErrors()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `errors` attribute

        []{#getCompressPngs()}

        -   #### getCompressPngs

            ``` methodSignature
            public boolean getCompressPngs()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `compressPngs` attribute

        []{#getOptimization()}

        -   #### getOptimization

            ``` methodSignature
            public com.facebook.buck.apple.AbstractAppleAssetCatalogsCompilationOptions.Optimization getOptimization()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `optimization` attribute

        []{#getOutputFormat()}

        -   #### getOutputFormat

            ``` methodSignature
            public com.facebook.buck.apple.AbstractAppleAssetCatalogsCompilationOptions.OutputFormat getOutputFormat()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `outputFormat` attribute

        []{#getExtraFlags()}

        -   #### getExtraFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getExtraFlags()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `extraFlags` attribute

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(@Nullable
                                  Object another)
            ```

            ::: block
            This instance is equal to all instances of
            `AppleAssetCatalogsCompilationOptions` that have equal
            attribute values.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `Object`

            [Returns:]{.returnLabel}
            :   `true` if `this` is equal to `another` instance

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            ::: block
            Computes a hash code from attributes: `notices`, `warnings`,
            `errors`, `compressPngs`, `optimization`, `outputFormat`,
            `extraFlags`.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `Object`

            [Returns:]{.returnLabel}
            :   hashCode value

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            ::: block
            Prints the immutable value
            `AppleAssetCatalogsCompilationOptions` with attribute
            values.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

            [Returns:]{.returnLabel}
            :   A string representation of the value

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static AppleAssetCatalogsCompilationOptions.Builder builder()
            ```

            ::: block
            Creates a builder for
            [`AppleAssetCatalogsCompilationOptions`](AppleAssetCatalogsCompilationOptions.html "class in com.facebook.buck.apple").
            :::

            [Returns:]{.returnLabel}
            :   A new AppleAssetCatalogsCompilationOptions builder
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
-   [Nested](#nested.class.summary) \| 
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

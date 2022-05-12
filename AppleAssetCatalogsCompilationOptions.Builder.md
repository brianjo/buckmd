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

## Class AppleAssetCatalogsCompilationOptions.Builder {#class-appleassetcatalogscompilationoptions.builder .title title="Class AppleAssetCatalogsCompilationOptions.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.AppleAssetCatalogsCompilationOptions.Builder

::: description
-   

    Enclosing class:
    :   [AppleAssetCatalogsCompilationOptions](AppleAssetCatalogsCompilationOptions.html "class in com.facebook.buck.apple")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class AppleAssetCatalogsCompilationOptions.Builder
        extends Object

    ::: block
    Builds instances of type
    [`AppleAssetCatalogsCompilationOptions`](AppleAssetCatalogsCompilationOptions.html "class in com.facebook.buck.apple").
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
        | `App                  | `ad                   | ::: block             |
        | leAssetCatalogsCompil | dAllExtraFlags​(Iterab | Adds elements to      |
        | ationOptions.Builder` | le<String> elements)` | [`extraFla            |
        |                       |                       | gs`](AppleAssetCatalo |
        |                       |                       | gsCompilationOptions. |
        |                       |                       | html#getExtraFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `App                  | `addExtraF            | ::: block             |
        | leAssetCatalogsCompil | lags​(String element)` | Adds one element to   |
        | ationOptions.Builder` |                       | [`extraFla            |
        |                       |                       | gs`](AppleAssetCatalo |
        |                       |                       | gsCompilationOptions. |
        |                       |                       | html#getExtraFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `App                  | `addExtraFlags        | ::: block             |
        | leAssetCatalogsCompil | ​(String... elements)` | Adds elements to      |
        | ationOptions.Builder` |                       | [`extraFla            |
        |                       |                       | gs`](AppleAssetCatalo |
        |                       |                       | gsCompilationOptions. |
        |                       |                       | html#getExtraFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleAssetCatalo     | `build()`             | ::: block             |
        | gsCompilationOptions` |                       | Builds a new          |
        |                       |                       | [`AppleAssetCa        |
        |                       |                       | talogsCompilationOpti |
        |                       |                       | ons`](AppleAssetCatal |
        |                       |                       | ogsCompilationOptions |
        |                       |                       | .html "class in com.f |
        |                       |                       | acebook.buck.apple"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `App                  | `from​(Apple           | ::: block             |
        | leAssetCatalogsCompil | AssetCatalogsCompilat | Fill a builder with   |
        | ationOptions.Builder` | ionOptions instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `AppleAssetCatalo     |
        |                       |                       | gsCompilationOptions` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `App                  | `setCompressPngs​(b    | ::: block             |
        | leAssetCatalogsCompil | oolean compressPngs)` | Initializes the value |
        | ationOptions.Builder` |                       | for the               |
        |                       |                       | [`compressPngs        |
        |                       |                       | `](AppleAssetCatalogs |
        |                       |                       | CompilationOptions.ht |
        |                       |                       | ml#getCompressPngs()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `App                  | `setEr                | ::: block             |
        | leAssetCatalogsCompil | rors​(boolean errors)` | Initializes the value |
        | ationOptions.Builder` |                       | for the               |
        |                       |                       | [`                    |
        |                       |                       | errors`](AppleAssetCa |
        |                       |                       | talogsCompilationOpti |
        |                       |                       | ons.html#getErrors()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `App                  | `setExtraFlags​(Iterab | ::: block             |
        | leAssetCatalogsCompil | le<String> elements)` | Sets or replaces all  |
        | ationOptions.Builder` |                       | elements for          |
        |                       |                       | [`extraFla            |
        |                       |                       | gs`](AppleAssetCatalo |
        |                       |                       | gsCompilationOptions. |
        |                       |                       | html#getExtraFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `App                  | `setNoti              | ::: block             |
        | leAssetCatalogsCompil | ces​(boolean notices)` | Initializes the value |
        | ationOptions.Builder` |                       | for the               |
        |                       |                       | [`no                  |
        |                       |                       | tices`](AppleAssetCat |
        |                       |                       | alogsCompilationOptio |
        |                       |                       | ns.html#getNotices()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `App                  | `setOpti              | ::: block             |
        | leAssetCatalogsCompil | mization​(com.facebook | Initializes the value |
        | ationOptions.Builder` | .buck.apple.AbstractA | for the               |
        |                       | ppleAssetCatalogsComp | [`optimization        |
        |                       | ilationOptions.Optimi | `](AppleAssetCatalogs |
        |                       | zation optimization)` | CompilationOptions.ht |
        |                       |                       | ml#getOptimization()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `App                  | `setOutp              | ::: block             |
        | leAssetCatalogsCompil | utFormat​(com.facebook | Initializes the value |
        | ationOptions.Builder` | .buck.apple.AbstractA | for the               |
        |                       | ppleAssetCatalogsComp | [`outputFormat        |
        |                       | ilationOptions.Output | `](AppleAssetCatalogs |
        |                       | Format outputFormat)` | CompilationOptions.ht |
        |                       |                       | ml#getOutputFormat()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `App                  | `setWarnin            | ::: block             |
        | leAssetCatalogsCompil | gs​(boolean warnings)` | Initializes the value |
        | ationOptions.Builder` |                       | for the               |
        |                       |                       | [`warn                |
        |                       |                       | ings`](AppleAssetCata |
        |                       |                       | logsCompilationOption |
        |                       |                       | s.html#getWarnings()) |
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

        []{#from(com.facebook.buck.apple.AppleAssetCatalogsCompilationOptions)}

        -   #### from

            ``` methodSignature
            public final AppleAssetCatalogsCompilationOptions.Builder from​(AppleAssetCatalogsCompilationOptions instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `AppleAssetCatalogsCompilationOptions` instance. Regular
            attribute values will be replaced with those from the given
            instance. Absent optional values will not replace present
            values. Collection elements and entries will be added, not
            replaced.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setNotices(boolean)}

        -   #### setNotices

            ``` methodSignature
            public final AppleAssetCatalogsCompilationOptions.Builder setNotices​(boolean notices)
            ```

            ::: block
            Initializes the value for the
            [`notices`](AppleAssetCatalogsCompilationOptions.html#getNotices())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`notices`](AppleAssetCatalogsCompilationOptions.html#getNotices()).*
            :::

            [Parameters:]{.paramLabel}
            :   `notices` - The value for notices

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setWarnings(boolean)}

        -   #### setWarnings

            ``` methodSignature
            public final AppleAssetCatalogsCompilationOptions.Builder setWarnings​(boolean warnings)
            ```

            ::: block
            Initializes the value for the
            [`warnings`](AppleAssetCatalogsCompilationOptions.html#getWarnings())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`warnings`](AppleAssetCatalogsCompilationOptions.html#getWarnings()).*
            :::

            [Parameters:]{.paramLabel}
            :   `warnings` - The value for warnings

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setErrors(boolean)}

        -   #### setErrors

            ``` methodSignature
            public final AppleAssetCatalogsCompilationOptions.Builder setErrors​(boolean errors)
            ```

            ::: block
            Initializes the value for the
            [`errors`](AppleAssetCatalogsCompilationOptions.html#getErrors())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`errors`](AppleAssetCatalogsCompilationOptions.html#getErrors()).*
            :::

            [Parameters:]{.paramLabel}
            :   `errors` - The value for errors

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompressPngs(boolean)}

        -   #### setCompressPngs

            ``` methodSignature
            public final AppleAssetCatalogsCompilationOptions.Builder setCompressPngs​(boolean compressPngs)
            ```

            ::: block
            Initializes the value for the
            [`compressPngs`](AppleAssetCatalogsCompilationOptions.html#getCompressPngs())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`compressPngs`](AppleAssetCatalogsCompilationOptions.html#getCompressPngs()).*
            :::

            [Parameters:]{.paramLabel}
            :   `compressPngs` - The value for compressPngs

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setOptimization(com.facebook.buck.apple.AbstractAppleAssetCatalogsCompilationOptions.Optimization)}

        -   #### setOptimization

            ``` methodSignature
            public final AppleAssetCatalogsCompilationOptions.Builder setOptimization​(com.facebook.buck.apple.AbstractAppleAssetCatalogsCompilationOptions.Optimization optimization)
            ```

            ::: block
            Initializes the value for the
            [`optimization`](AppleAssetCatalogsCompilationOptions.html#getOptimization())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`optimization`](AppleAssetCatalogsCompilationOptions.html#getOptimization()).*
            :::

            [Parameters:]{.paramLabel}
            :   `optimization` - The value for optimization

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setOutputFormat(com.facebook.buck.apple.AbstractAppleAssetCatalogsCompilationOptions.OutputFormat)}

        -   #### setOutputFormat

            ``` methodSignature
            public final AppleAssetCatalogsCompilationOptions.Builder setOutputFormat​(com.facebook.buck.apple.AbstractAppleAssetCatalogsCompilationOptions.OutputFormat outputFormat)
            ```

            ::: block
            Initializes the value for the
            [`outputFormat`](AppleAssetCatalogsCompilationOptions.html#getOutputFormat())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`outputFormat`](AppleAssetCatalogsCompilationOptions.html#getOutputFormat()).*
            :::

            [Parameters:]{.paramLabel}
            :   `outputFormat` - The value for outputFormat

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExtraFlags(java.lang.String)}

        -   #### addExtraFlags

            ``` methodSignature
            public final AppleAssetCatalogsCompilationOptions.Builder addExtraFlags​(String element)
            ```

            ::: block
            Adds one element to
            [`extraFlags`](AppleAssetCatalogsCompilationOptions.html#getExtraFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A extraFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExtraFlags(java.lang.String...)}

        -   #### addExtraFlags

            ``` methodSignature
            public final AppleAssetCatalogsCompilationOptions.Builder addExtraFlags​(String... elements)
            ```

            ::: block
            Adds elements to
            [`extraFlags`](AppleAssetCatalogsCompilationOptions.html#getExtraFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of extraFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExtraFlags(java.lang.Iterable)}

        -   #### setExtraFlags

            ``` methodSignature
            public final AppleAssetCatalogsCompilationOptions.Builder setExtraFlags​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`extraFlags`](AppleAssetCatalogsCompilationOptions.html#getExtraFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of extraFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllExtraFlags(java.lang.Iterable)}

        -   #### addAllExtraFlags

            ``` methodSignature
            public final AppleAssetCatalogsCompilationOptions.Builder addAllExtraFlags​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`extraFlags`](AppleAssetCatalogsCompilationOptions.html#getExtraFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of extraFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public AppleAssetCatalogsCompilationOptions build()
            ```

            ::: block
            Builds a new
            [`AppleAssetCatalogsCompilationOptions`](AppleAssetCatalogsCompilationOptions.html "class in com.facebook.buck.apple").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of
                AppleAssetCatalogsCompilationOptions

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

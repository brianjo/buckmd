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

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../deprecated-list.html)
-   [Index](../../../../../index-all.html)
-   [Help](../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.features.python](package-summary.html)
:::

## Class PrebuiltPythonLibraryDescriptionArg.Builder {#class-prebuiltpythonlibrarydescriptionarg.builder .title title="Class PrebuiltPythonLibraryDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.python.PrebuiltPythonLibraryDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [PrebuiltPythonLibraryDescriptionArg](PrebuiltPythonLibraryDescriptionArg.html "class in com.facebook.buck.features.python")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class PrebuiltPythonLibraryDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`PrebuiltPythonLibraryDescriptionArg`](PrebuiltPythonLibraryDescriptionArg.html "class in com.facebook.buck.features.python").
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
        | ebuiltPythonLibraryDe | ibleWith​(Iterable<? e | Adds elements to      |
        | scriptionArg.Builder` | xtends UnconfiguredBu | [`compatibleWith`     |
        |                       | ildTarget> elements)` | ](PrebuiltPythonLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `addAllDeps​(          | ::: block             |
        | ebuiltPythonLibraryDe | Iterable<? extends Bu | Adds elements to      |
        | scriptionArg.Builder` | ildTarget> elements)` | [`deps`](PrebuiltP    |
        |                       |                       | ythonLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `addAllLabels​(Iterab  | ::: block             |
        | ebuiltPythonLibraryDe | le<String> elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [                     |
        |                       |                       | `labels`](PrebuiltPyt |
        |                       |                       | honLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `addAllLicenses       | ::: block             |
        | ebuiltPythonLibraryDe | ​(Iterable<? extends S | Adds elements to      |
        | scriptionArg.Builder` | ourcePath> elements)` | [`lic                 |
        |                       |                       | enses`](PrebuiltPytho |
        |                       |                       | nLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `addCompat            | ::: block             |
        | ebuiltPythonLibraryDe | ibleWith​(Unconfigured | Adds one element to   |
        | scriptionArg.Builder` | BuildTarget element)` | [`compatibleWith`     |
        |                       |                       | ](PrebuiltPythonLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `addCompatible        | ::: block             |
        | ebuiltPythonLibraryDe | With​(UnconfiguredBuil | Adds elements to      |
        | scriptionArg.Builder` | dTarget... elements)` | [`compatibleWith`     |
        |                       |                       | ](PrebuiltPythonLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `addDeps​(             | ::: block             |
        | ebuiltPythonLibraryDe | BuildTarget element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`deps`](PrebuiltP    |
        |                       |                       | ythonLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `addDeps​(Buil         | ::: block             |
        | ebuiltPythonLibraryDe | dTarget... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`deps`](PrebuiltP    |
        |                       |                       | ythonLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `addLa                | ::: block             |
        | ebuiltPythonLibraryDe | bels​(String element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [                     |
        |                       |                       | `labels`](PrebuiltPyt |
        |                       |                       | honLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `addLabels            | ::: block             |
        | ebuiltPythonLibraryDe | ​(String... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [                     |
        |                       |                       | `labels`](PrebuiltPyt |
        |                       |                       | honLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `addLicenses          | ::: block             |
        | ebuiltPythonLibraryDe | ​(SourcePath element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`lic                 |
        |                       |                       | enses`](PrebuiltPytho |
        |                       |                       | nLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `addLicenses​(Sou      | ::: block             |
        | ebuiltPythonLibraryDe | rcePath... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`lic                 |
        |                       |                       | enses`](PrebuiltPytho |
        |                       |                       | nLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltPythonL      | `build()`             | ::: block             |
        | ibraryDescriptionArg` |                       | Builds a new          |
        |                       |                       | [                     |
        |                       |                       | `PrebuiltPythonLibrar |
        |                       |                       | yDescriptionArg`](Pre |
        |                       |                       | builtPythonLibraryDes |
        |                       |                       | criptionArg.html "cla |
        |                       |                       | ss in com.facebook.bu |
        |                       |                       | ck.features.python"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `from​(Bu              | ::: block             |
        | ebuiltPythonLibraryDe | ildRuleArg instance)` | Fill a builder with   |
        | scriptionArg.Builder` |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `from​(Cons            | ::: block             |
        | ebuiltPythonLibraryDe | tructorArg instance)` | Fill a builder with   |
        | scriptionArg.Builder` |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `from​(HasDe           | ::: block             |
        | ebuiltPythonLibraryDe | claredDeps instance)` | Fill a builder with   |
        | scriptionArg.Builder` |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasDeclaredDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `                     | ::: block             |
        | ebuiltPythonLibraryDe | from​(com.facebook.buc | Copy abstract value   |
        | scriptionArg.Builder` | k.features.python.Pre | type                  |
        |                       | builtPythonLibraryDes | `Ab                   |
        |                       | cription.AbstractPreb | stractPrebuiltPythonL |
        |                       | uiltPythonLibraryDesc | ibraryDescriptionArg` |
        |                       | riptionArg instance)` | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `from​(Preb            | ::: block             |
        | ebuiltPythonLibraryDe | uiltPythonLibraryDesc | Fill a builder with   |
        | scriptionArg.Builder` | riptionArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `PrebuiltPythonL      |
        |                       |                       | ibraryDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `setBinarySrc​(S       | ::: block             |
        | ebuiltPythonLibraryDe | ourcePath binarySrc)` | Initializes the value |
        | scriptionArg.Builder` |                       | for the               |
        |                       |                       | [`binar               |
        |                       |                       | ySrc`](PrebuiltPython |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getBinarySrc()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `setCompat            | ::: block             |
        | ebuiltPythonLibraryDe | ibleWith​(Iterable<? e | Sets or replaces all  |
        | scriptionArg.Builder` | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`compatibleWith`     |
        |                       |                       | ](PrebuiltPythonLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `setComp              | ::: block             |
        | ebuiltPythonLibraryDe | ile​(boolean compile)` | Initializes the value |
        | scriptionArg.Builder` |                       | for the               |
        |                       |                       | [`                    |
        |                       |                       | compile`](PrebuiltPyt |
        |                       |                       | honLibraryDescription |
        |                       |                       | Arg.html#isCompile()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `setDefaul            | ::: block             |
        | ebuiltPythonLibraryDe | tTargetPlatform​(Uncon | Initializes the       |
        | scriptionArg.Builder` | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`defaultT            |
        |                       |                       | argetPlatform`](Prebu |
        |                       |                       | iltPythonLibraryDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `setDefau             | ::: block             |
        | ebuiltPythonLibraryDe | ltTargetPlatform​(Opti | Initializes the       |
        | scriptionArg.Builder` | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`defaultT            |
        |                       | faultTargetPlatform)` | argetPlatform`](Prebu |
        |                       |                       | iltPythonLibraryDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `setDeps​(             | ::: block             |
        | ebuiltPythonLibraryDe | Iterable<? extends Bu | Sets or replaces all  |
        | scriptionArg.Builder` | ildTarget> elements)` | elements for          |
        |                       |                       | [`deps`](PrebuiltP    |
        |                       |                       | ythonLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `setExcl              | ::: block             |
        | ebuiltPythonLibraryDe | udeDepsFromMergedLink | Initializes the value |
        | scriptionArg.Builder` | ing​(boolean excludeDe | for the               |
        |                       | psFromMergedLinking)` | [`                    |
        |                       |                       | excludeDepsFromMerged |
        |                       |                       | Linking`](PrebuiltPyt |
        |                       |                       | honLibraryDescription |
        |                       |                       | Arg.html#isExcludeDep |
        |                       |                       | sFromMergedLinking()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `setIgnoreC           | ::: block             |
        | ebuiltPythonLibraryDe | ompileErrors​(boolean  | Initializes the value |
        | scriptionArg.Builder` | ignoreCompileErrors)` | for the               |
        |                       |                       | [`ign                 |
        |                       |                       | oreCompileErrors`](Pr |
        |                       |                       | ebuiltPythonLibraryDe |
        |                       |                       | scriptionArg.html#isI |
        |                       |                       | gnoreCompileErrors()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `setLabels​(Iterab     | ::: block             |
        | ebuiltPythonLibraryDe | le<String> elements)` | Sets or replaces all  |
        | scriptionArg.Builder` |                       | elements for          |
        |                       |                       | [                     |
        |                       |                       | `labels`](PrebuiltPyt |
        |                       |                       | honLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `setLicenses          | ::: block             |
        | ebuiltPythonLibraryDe | ​(Iterable<? extends S | Sets or replaces all  |
        | scriptionArg.Builder` | ourcePath> elements)` | elements for          |
        |                       |                       | [`lic                 |
        |                       |                       | enses`](PrebuiltPytho |
        |                       |                       | nLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `                     | ::: block             |
        | ebuiltPythonLibraryDe | setName​(String name)` | Initializes the value |
        | scriptionArg.Builder` |                       | for the               |
        |                       |                       | [`name`](PrebuiltP    |
        |                       |                       | ythonLibraryDescripti |
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

        []{#from(com.facebook.buck.features.python.PrebuiltPythonLibraryDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final PrebuiltPythonLibraryDescriptionArg.Builder from​(PrebuiltPythonLibraryDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `PrebuiltPythonLibraryDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.features.python.PrebuiltPythonLibraryDescription.AbstractPrebuiltPythonLibraryDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final PrebuiltPythonLibraryDescriptionArg.Builder from​(com.facebook.buck.features.python.PrebuiltPythonLibraryDescription.AbstractPrebuiltPythonLibraryDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type
            `AbstractPrebuiltPythonLibraryDescriptionArg` instance into
            builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.HasDeclaredDeps)}

        -   #### from

            ``` methodSignature
            public final PrebuiltPythonLibraryDescriptionArg.Builder from​(HasDeclaredDeps instance)
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
            public final PrebuiltPythonLibraryDescriptionArg.Builder from​(BuildRuleArg instance)
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
            public final PrebuiltPythonLibraryDescriptionArg.Builder from​(ConstructorArg instance)
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

        []{#setBinarySrc(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setBinarySrc

            ``` methodSignature
            public final PrebuiltPythonLibraryDescriptionArg.Builder setBinarySrc​(SourcePath binarySrc)
            ```

            ::: block
            Initializes the value for the
            [`binarySrc`](PrebuiltPythonLibraryDescriptionArg.html#getBinarySrc())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `binarySrc` - The value for binarySrc

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExcludeDepsFromMergedLinking(boolean)}

        -   #### setExcludeDepsFromMergedLinking

            ``` methodSignature
            public final PrebuiltPythonLibraryDescriptionArg.Builder setExcludeDepsFromMergedLinking​(boolean excludeDepsFromMergedLinking)
            ```

            ::: block
            Initializes the value for the
            [`excludeDepsFromMergedLinking`](PrebuiltPythonLibraryDescriptionArg.html#isExcludeDepsFromMergedLinking())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`excludeDepsFromMergedLinking`](PrebuiltPythonLibraryDescriptionArg.html#isExcludeDepsFromMergedLinking()).*
            :::

            [Parameters:]{.paramLabel}
            :   `excludeDepsFromMergedLinking` - The value for
                excludeDepsFromMergedLinking

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setIgnoreCompileErrors(boolean)}

        -   #### setIgnoreCompileErrors

            ``` methodSignature
            public final PrebuiltPythonLibraryDescriptionArg.Builder setIgnoreCompileErrors​(boolean ignoreCompileErrors)
            ```

            ::: block
            Initializes the value for the
            [`ignoreCompileErrors`](PrebuiltPythonLibraryDescriptionArg.html#isIgnoreCompileErrors())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`ignoreCompileErrors`](PrebuiltPythonLibraryDescriptionArg.html#isIgnoreCompileErrors()).*
            :::

            [Parameters:]{.paramLabel}
            :   `ignoreCompileErrors` - The value for
                ignoreCompileErrors

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompile(boolean)}

        -   #### setCompile

            ``` methodSignature
            public final PrebuiltPythonLibraryDescriptionArg.Builder setCompile​(boolean compile)
            ```

            ::: block
            Initializes the value for the
            [`compile`](PrebuiltPythonLibraryDescriptionArg.html#isCompile())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`compile`](PrebuiltPythonLibraryDescriptionArg.html#isCompile()).*
            :::

            [Parameters:]{.paramLabel}
            :   `compile` - The value for compile

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final PrebuiltPythonLibraryDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](PrebuiltPythonLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final PrebuiltPythonLibraryDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](PrebuiltPythonLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final PrebuiltPythonLibraryDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](PrebuiltPythonLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final PrebuiltPythonLibraryDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](PrebuiltPythonLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final PrebuiltPythonLibraryDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](PrebuiltPythonLibraryDescriptionArg.html#getDefaultTargetPlatform())
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
            public final PrebuiltPythonLibraryDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](PrebuiltPythonLibraryDescriptionArg.html#getDefaultTargetPlatform())
            to defaultTargetPlatform.
            :::

            [Parameters:]{.paramLabel}
            :   `defaultTargetPlatform` - The value for
                defaultTargetPlatform

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String)}

        -   #### addLabels

            ``` methodSignature
            public final PrebuiltPythonLibraryDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](PrebuiltPythonLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final PrebuiltPythonLibraryDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](PrebuiltPythonLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final PrebuiltPythonLibraryDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](PrebuiltPythonLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final PrebuiltPythonLibraryDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](PrebuiltPythonLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final PrebuiltPythonLibraryDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](PrebuiltPythonLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final PrebuiltPythonLibraryDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](PrebuiltPythonLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final PrebuiltPythonLibraryDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](PrebuiltPythonLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final PrebuiltPythonLibraryDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](PrebuiltPythonLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final PrebuiltPythonLibraryDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](PrebuiltPythonLibraryDescriptionArg.html#getName())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addDeps

            ``` methodSignature
            public final PrebuiltPythonLibraryDescriptionArg.Builder addDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`deps`](PrebuiltPythonLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A deps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addDeps

            ``` methodSignature
            public final PrebuiltPythonLibraryDescriptionArg.Builder addDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`deps`](PrebuiltPythonLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDeps(java.lang.Iterable)}

        -   #### setDeps

            ``` methodSignature
            public final PrebuiltPythonLibraryDescriptionArg.Builder setDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`deps`](PrebuiltPythonLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllDeps(java.lang.Iterable)}

        -   #### addAllDeps

            ``` methodSignature
            public final PrebuiltPythonLibraryDescriptionArg.Builder addAllDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`deps`](PrebuiltPythonLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public PrebuiltPythonLibraryDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`PrebuiltPythonLibraryDescriptionArg`](PrebuiltPythonLibraryDescriptionArg.html "class in com.facebook.buck.features.python").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of
                PrebuiltPythonLibraryDescriptionArg

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

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../deprecated-list.html)
-   [Index](../../../../../index-all.html)
-   [Help](../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../allclasses.html)

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

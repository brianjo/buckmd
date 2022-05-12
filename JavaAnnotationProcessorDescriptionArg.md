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
-   [Nested](#nested.class.summary) \| 
-   [Field](#field.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java](package-summary.html)
:::

## Class JavaAnnotationProcessorDescriptionArg {#class-javaannotationprocessordescriptionarg .title title="Class JavaAnnotationProcessorDescriptionArg"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.JavaAnnotationProcessorDescriptionArg

::: description
-   

    All Implemented Interfaces:
    :   `BuildRuleArg`, `ConstructorArg`, `DataTransferObject`,
        `HasDeclaredDeps`, `JavacPluginArgs`

    ------------------------------------------------------------------------

        @ParametersAreNonnullByDefault
        @Generated("org.immutables.processor.ProxyProcessor")
        @Immutable
        @CheckReturnValue
        public final class JavaAnnotationProcessorDescriptionArg
        extends Object

    ::: block
    Immutable implementation of
    `JavaAnnotationProcessorDescription.AbstractJavaAnnotationProcessorDescriptionArg`.
    Use the builder to create immutable instances:
    `JavaAnnotationProcessorDescriptionArg.builder()`.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `Java                 | ::: block             |
        |                       | AnnotationProcessorDe | Builds instances of   |
        |                       | scriptionArg.Builder` | type                  |
        |                       |                       | [`JavaAnnotationPro   |
        |                       |                       | cessorDescriptionArg` |
        |                       |                       | ](JavaAnnotationProce |
        |                       |                       | ssorDescriptionArg.ht |
        |                       |                       | ml "class in com.face |
        |                       |                       | book.buck.jvm.java"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.core.description.arg.BuildRuleArg}

            ### Fields inherited from interface com.facebook.buck.core.description.arg.[BuildRuleArg](../../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")

            `DEFAULT_TARGET_PLATFORM_PARAM_NAME`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static Java          | `builder()`           | ::: block             |
        | AnnotationProcessorDe |                       | Creates a builder for |
        | scriptionArg.Builder` |                       | [`JavaAnnotationPro   |
        |                       |                       | cessorDescriptionArg` |
        |                       |                       | ](JavaAnnotationProce |
        |                       |                       | ssorDescriptionArg.ht |
        |                       |                       | ml "class in com.face |
        |                       |                       | book.buck.jvm.java"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `eq                   | ::: block             |
        |                       | uals​(Object another)` | This instance is      |
        |                       |                       | equal to all          |
        |                       |                       | instances of          |
        |                       |                       | `JavaAnnotationPro    |
        |                       |                       | cessorDescriptionArg` |
        |                       |                       | that have equal       |
        |                       |                       | attribute values.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `co                   | `getCompatibleWith()` | ::: block             |
        | m.google.common.colle |                       | A list of             |
        | ct.ImmutableList<Unco |                       | `config_setting` a    |
        | nfiguredBuildTarget>` |                       | target is compatible  |
        |                       |                       | with.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Unco        | `getDef               | ::: block             |
        | nfiguredBuildTarget>` | aultTargetPlatform()` | The name of build     |
        |                       |                       | target default        |
        |                       |                       | \"new\" platform: it  |
        |                       |                       | is used when a        |
        |                       |                       | platform is not       |
        |                       |                       | specified either      |
        |                       |                       | globally or in a      |
        |                       |                       | target which used     |
        |                       |                       | this target as a      |
        |                       |                       | dependency.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getDeps()`           |                       |
        | n.collect.ImmutableSo |                       |                       |
        | rtedSet<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `getLabels()`         |                       |
        | common.collect.Immuta |                       |                       |
        | bleSortedSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `getLicenses()`       |                       |
        | e.common.collect.Immu |                       |                       |
        | tableSet<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getName()`           | ::: block             |
        |                       |                       | Each rule has a name  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getProcessorClass()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.g                | `g                    |                       |
        | oogle.common.collect. | etProcessorClasses()` |                       |
        | ImmutableSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          | ::: block             |
        |                       |                       | Computes a hash code  |
        |                       |                       | from attributes:      |
        |                       |                       | `processorClass`,     |
        |                       |                       | `processorClasses`,   |
        |                       |                       | `isolateClassLoader`, |
        |                       |                       | `doesNotAffectAbi`,   |
        |                       |                       | `supportsAbiG         |
        |                       |                       | enerationFromSource`, |
        |                       |                       | `licenses`, `labels`, |
        |                       |                       | `de                   |
        |                       |                       | faultTargetPlatform`, |
        |                       |                       | `compatibleWith`,     |
        |                       |                       | `name`, `deps`.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `                     | ::: block             |
        |                       | isDoesNotAffectAbi()` | A value of false      |
        |                       |                       | indicates that the    |
        |                       |                       | plugin either         |
        |                       |                       | generates classes     |
        |                       |                       | that are intended for |
        |                       |                       | use outside of the    |
        |                       |                       | code being processed  |
        |                       |                       | or modifies bytecode  |
        |                       |                       | in a way that         |
        |                       |                       | modifies ABI.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `is                   | ::: block             |
        |                       | IsolateClassLoader()` | A value of false      |
        |                       |                       | indicates that the    |
        |                       |                       | plugin will not use a |
        |                       |                       | shared class loader   |
        |                       |                       | to be loaded.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isSupportsAbiGe      | ::: block             |
        |                       | nerationFromSource()` | If true, allows       |
        |                       |                       | ABI-affecting plugins |
        |                       |                       | to run during ABI     |
        |                       |                       | generation from       |
        |                       |                       | source.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          | ::: block             |
        |                       |                       | Prints the immutable  |
        |                       |                       | value                 |
        |                       |                       | `JavaAnnotationPro    |
        |                       |                       | cessorDescriptionArg` |
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

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.arg.BuildRuleArg}

            ### Methods inherited from interface com.facebook.buck.core.description.arg.[BuildRuleArg](../../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")

            `labelsContainsAnyOf`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getProcessorClass()}

        -   #### getProcessorClass

            ``` methodSignature
            public Optional<String> getProcessorClass()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `processorClass` attribute

        []{#getProcessorClasses()}

        -   #### getProcessorClasses

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<String> getProcessorClasses()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `processorClasses` attribute

        []{#isIsolateClassLoader()}

        -   #### isIsolateClassLoader

            ``` methodSignature
            public boolean isIsolateClassLoader()
            ```

            ::: block
            A value of false indicates that the plugin will not use a
            shared class loader to be loaded. This should be true if the
            same instance of the plugin has not support to run
            concurrently multiple times for different javac calls.
            Defaults to false because that\'s the \"safe\" value and
            optimizes build time.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `isIsolateClassLoader` in interface `JavacPluginArgs`

        []{#isDoesNotAffectAbi()}

        -   #### isDoesNotAffectAbi

            ``` methodSignature
            public boolean isDoesNotAffectAbi()
            ```

            ::: block
            A value of false indicates that the plugin either generates
            classes that are intended for use outside of the code being
            processed or modifies bytecode in a way that modifies ABI.
            Plugins that affect the ABI of the rule in which they run
            must be run during ABI generation from source.
            Defaults to false because that\'s the \"safe\" value. When
            migrating to ABI generation from source, having as few
            ABI-affecting plugins as possible will yield the fastest ABI
            generation.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `isDoesNotAffectAbi` in interface `JavacPluginArgs`

        []{#isSupportsAbiGenerationFromSource()}

        -   #### isSupportsAbiGenerationFromSource

            ``` methodSignature
            public boolean isSupportsAbiGenerationFromSource()
            ```

            ::: block
            If true, allows ABI-affecting plugins to run during ABI
            generation from source. To run during ABI generation from
            source, a plugin must meet all of the following criteria:

            ```{=html}
            <!-- -->
            ```

            Defaults to false because that\'s the \"safe\" value. When
            migrating to ABI generation from source, having as many
            ABI-affecting plugins as possible running during ABI
            generation will result in the flattest build graph.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `isSupportsAbiGenerationFromSource` in
                interface `JavacPluginArgs`

        []{#getLicenses()}

        -   #### getLicenses

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<SourcePath> getLicenses()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLicenses` in interface `BuildRuleArg`

            [Returns:]{.returnLabel}
            :   The value of the `licenses` attribute

        []{#getLabels()}

        -   #### getLabels

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<String> getLabels()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLabels` in interface `BuildRuleArg`

            [Returns:]{.returnLabel}
            :   The value of the `labels` attribute

        []{#getDefaultTargetPlatform()}

        -   #### getDefaultTargetPlatform

            ``` methodSignature
            public Optional<UnconfiguredBuildTarget> getDefaultTargetPlatform()
            ```

            ::: block
            The name of build target default \"new\" platform: it is
            used when a platform is not specified either globally or in
            a target which used this target as a dependency.
            The value is a build target, but we specify it as string,
            because this function is not actually called, but the attr
            is fetched by name from the raw (unconfigured) target node.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDefaultTargetPlatform` in interface `BuildRuleArg`

        []{#getCompatibleWith()}

        -   #### getCompatibleWith

            ``` methodSignature
            public com.google.common.collect.ImmutableList<UnconfiguredBuildTarget> getCompatibleWith()
            ```

            ::: block
            A list of `config_setting` a target is compatible with.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCompatibleWith` in interface `BuildRuleArg`

        []{#getName()}

        -   #### getName

            ``` methodSignature
            public String getName()
            ```

            ::: block
            Each rule has a name
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getName` in interface `ConstructorArg`

        []{#getDeps()}

        -   #### getDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<BuildTarget> getDeps()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDeps` in interface `HasDeclaredDeps`

            [Returns:]{.returnLabel}
            :   The value of the `deps` attribute

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(@Nullable
                                  Object another)
            ```

            ::: block
            This instance is equal to all instances of
            `JavaAnnotationProcessorDescriptionArg` that have equal
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
            Computes a hash code from attributes: `processorClass`,
            `processorClasses`, `isolateClassLoader`,
            `doesNotAffectAbi`, `supportsAbiGenerationFromSource`,
            `licenses`, `labels`, `defaultTargetPlatform`,
            `compatibleWith`, `name`, `deps`.
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
            `JavaAnnotationProcessorDescriptionArg` with attribute
            values.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

            [Returns:]{.returnLabel}
            :   A string representation of the value

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static JavaAnnotationProcessorDescriptionArg.Builder builder()
            ```

            ::: block
            Creates a builder for
            [`JavaAnnotationProcessorDescriptionArg`](JavaAnnotationProcessorDescriptionArg.html "class in com.facebook.buck.jvm.java").
            :::

            [Returns:]{.returnLabel}
            :   A new JavaAnnotationProcessorDescriptionArg builder
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
-   [Nested](#nested.class.summary) \| 
-   [Field](#field.summary) \| 
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

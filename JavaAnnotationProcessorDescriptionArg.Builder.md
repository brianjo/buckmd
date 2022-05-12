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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java](package-summary.html)
:::

## Class JavaAnnotationProcessorDescriptionArg.Builder {#class-javaannotationprocessordescriptionarg.builder .title title="Class JavaAnnotationProcessorDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.JavaAnnotationProcessorDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [JavaAnnotationProcessorDescriptionArg](JavaAnnotationProcessorDescriptionArg.html "class in com.facebook.buck.jvm.java")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class JavaAnnotationProcessorDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`JavaAnnotationProcessorDescriptionArg`](JavaAnnotationProcessorDescriptionArg.html "class in com.facebook.buck.jvm.java").
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
        | `Java                 | `addAllCompat         | ::: block             |
        | AnnotationProcessorDe | ibleWith​(Iterable<? e | Adds elements to      |
        | scriptionArg.Builder` | xtends UnconfiguredBu | [`compatibleWith`](   |
        |                       | ildTarget> elements)` | JavaAnnotationProcess |
        |                       |                       | orDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Java                 | `addAllDeps​(          | ::: block             |
        | AnnotationProcessorDe | Iterable<? extends Bu | Adds elements to      |
        | scriptionArg.Builder` | ildTarget> elements)` | [`deps`](JavaAnnotat  |
        |                       |                       | ionProcessorDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Java                 | `addAllLabels​(Iterab  | ::: block             |
        | AnnotationProcessorDe | le<String> elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`l                   |
        |                       |                       | abels`](JavaAnnotatio |
        |                       |                       | nProcessorDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Java                 | `addAllLicenses       | ::: block             |
        | AnnotationProcessorDe | ​(Iterable<? extends S | Adds elements to      |
        | scriptionArg.Builder` | ourcePath> elements)` | [`licen               |
        |                       |                       | ses`](JavaAnnotationP |
        |                       |                       | rocessorDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Java                 | `addAllPr             | ::: block             |
        | AnnotationProcessorDe | ocessorClasses​(Iterab | Adds elements to      |
        | scriptionArg.Builder` | le<String> elements)` | [`                    |
        |                       |                       | processorClasses`](Ja |
        |                       |                       | vaAnnotationProcessor |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etProcessorClasses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Java                 | `addCompat            | ::: block             |
        | AnnotationProcessorDe | ibleWith​(Unconfigured | Adds one element to   |
        | scriptionArg.Builder` | BuildTarget element)` | [`compatibleWith`](   |
        |                       |                       | JavaAnnotationProcess |
        |                       |                       | orDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Java                 | `addCompatible        | ::: block             |
        | AnnotationProcessorDe | With​(UnconfiguredBuil | Adds elements to      |
        | scriptionArg.Builder` | dTarget... elements)` | [`compatibleWith`](   |
        |                       |                       | JavaAnnotationProcess |
        |                       |                       | orDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Java                 | `addDeps​(             | ::: block             |
        | AnnotationProcessorDe | BuildTarget element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`deps`](JavaAnnotat  |
        |                       |                       | ionProcessorDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Java                 | `addDeps​(Buil         | ::: block             |
        | AnnotationProcessorDe | dTarget... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`deps`](JavaAnnotat  |
        |                       |                       | ionProcessorDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Java                 | `addLa                | ::: block             |
        | AnnotationProcessorDe | bels​(String element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`l                   |
        |                       |                       | abels`](JavaAnnotatio |
        |                       |                       | nProcessorDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Java                 | `addLabels            | ::: block             |
        | AnnotationProcessorDe | ​(String... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`l                   |
        |                       |                       | abels`](JavaAnnotatio |
        |                       |                       | nProcessorDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Java                 | `addLicenses          | ::: block             |
        | AnnotationProcessorDe | ​(SourcePath element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`licen               |
        |                       |                       | ses`](JavaAnnotationP |
        |                       |                       | rocessorDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Java                 | `addLicenses​(Sou      | ::: block             |
        | AnnotationProcessorDe | rcePath... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`licen               |
        |                       |                       | ses`](JavaAnnotationP |
        |                       |                       | rocessorDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Java                 | `addProcessorCla      | ::: block             |
        | AnnotationProcessorDe | sses​(String element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`                    |
        |                       |                       | processorClasses`](Ja |
        |                       |                       | vaAnnotationProcessor |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etProcessorClasses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Java                 | `addProcessorClasses  | ::: block             |
        | AnnotationProcessorDe | ​(String... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`                    |
        |                       |                       | processorClasses`](Ja |
        |                       |                       | vaAnnotationProcessor |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etProcessorClasses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaAnnotationPro    | `build()`             | ::: block             |
        | cessorDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`JavaAnnotationPro   |
        |                       |                       | cessorDescriptionArg` |
        |                       |                       | ](JavaAnnotationProce |
        |                       |                       | ssorDescriptionArg.ht |
        |                       |                       | ml "class in com.face |
        |                       |                       | book.buck.jvm.java"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Java                 | `from​(Bu              | ::: block             |
        | AnnotationProcessorDe | ildRuleArg instance)` | Fill a builder with   |
        | scriptionArg.Builder` |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Java                 | `from​(Cons            | ::: block             |
        | AnnotationProcessorDe | tructorArg instance)` | Fill a builder with   |
        | scriptionArg.Builder` |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Java                 | `from​(HasDe           | ::: block             |
        | AnnotationProcessorDe | claredDeps instance)` | Fill a builder with   |
        | scriptionArg.Builder` |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasDeclaredDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Java                 | `from​(com.facebook.   | ::: block             |
        | AnnotationProcessorDe | buck.jvm.java.JavaAnn | Copy abstract value   |
        | scriptionArg.Builder` | otationProcessorDescr | type                  |
        |                       | iption.AbstractJavaAn | `Abst                 |
        |                       | notationProcessorDesc | ractJavaAnnotationPro |
        |                       | riptionArg instance)` | cessorDescriptionArg` |
        |                       |                       | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Java                 | `from​(JavaAn          | ::: block             |
        | AnnotationProcessorDe | notationProcessorDesc | Fill a builder with   |
        | scriptionArg.Builder` | riptionArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `JavaAnnotationPro    |
        |                       |                       | cessorDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Java                 | `from​(Javac           | ::: block             |
        | AnnotationProcessorDe | PluginArgs instance)` | Fill a builder with   |
        | scriptionArg.Builder` |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `c                    |
        |                       |                       | om.facebook.buck.jvm. |
        |                       |                       | java.JavacPluginArgs` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Java                 | `setCompat            | ::: block             |
        | AnnotationProcessorDe | ibleWith​(Iterable<? e | Sets or replaces all  |
        | scriptionArg.Builder` | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`compatibleWith`](   |
        |                       |                       | JavaAnnotationProcess |
        |                       |                       | orDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Java                 | `setDefaul            | ::: block             |
        | AnnotationProcessorDe | tTargetPlatform​(Uncon | Initializes the       |
        | scriptionArg.Builder` | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`defaultTar          |
        |                       |                       | getPlatform`](JavaAnn |
        |                       |                       | otationProcessorDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Java                 | `setDefau             | ::: block             |
        | AnnotationProcessorDe | ltTargetPlatform​(Opti | Initializes the       |
        | scriptionArg.Builder` | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`defaultTar          |
        |                       | faultTargetPlatform)` | getPlatform`](JavaAnn |
        |                       |                       | otationProcessorDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Java                 | `setDeps​(             | ::: block             |
        | AnnotationProcessorDe | Iterable<? extends Bu | Sets or replaces all  |
        | scriptionArg.Builder` | ildTarget> elements)` | elements for          |
        |                       |                       | [`deps`](JavaAnnotat  |
        |                       |                       | ionProcessorDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Java                 | `setD                 | ::: block             |
        | AnnotationProcessorDe | oesNotAffectAbi​(boole | Initializes the value |
        | scriptionArg.Builder` | an doesNotAffectAbi)` | for the               |
        |                       |                       | [                     |
        |                       |                       | `doesNotAffectAbi`](J |
        |                       |                       | avaAnnotationProcesso |
        |                       |                       | rDescriptionArg.html# |
        |                       |                       | isDoesNotAffectAbi()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Java                 | `setIsola             | ::: block             |
        | AnnotationProcessorDe | teClassLoader​(boolean | Initializes the value |
        | scriptionArg.Builder` |  isolateClassLoader)` | for the               |
        |                       |                       | [`iso                 |
        |                       |                       | lateClassLoader`](Jav |
        |                       |                       | aAnnotationProcessorD |
        |                       |                       | escriptionArg.html#is |
        |                       |                       | IsolateClassLoader()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Java                 | `setLabels​(Iterab     | ::: block             |
        | AnnotationProcessorDe | le<String> elements)` | Sets or replaces all  |
        | scriptionArg.Builder` |                       | elements for          |
        |                       |                       | [`l                   |
        |                       |                       | abels`](JavaAnnotatio |
        |                       |                       | nProcessorDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Java                 | `setLicenses          | ::: block             |
        | AnnotationProcessorDe | ​(Iterable<? extends S | Sets or replaces all  |
        | scriptionArg.Builder` | ourcePath> elements)` | elements for          |
        |                       |                       | [`licen               |
        |                       |                       | ses`](JavaAnnotationP |
        |                       |                       | rocessorDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Java                 | `                     | ::: block             |
        | AnnotationProcessorDe | setName​(String name)` | Initializes the value |
        | scriptionArg.Builder` |                       | for the               |
        |                       |                       | [`name`](JavaAnnotat  |
        |                       |                       | ionProcessorDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Java                 | `setProcessorClass​(St | ::: block             |
        | AnnotationProcessorDe | ring processorClass)` | Initializes the       |
        | scriptionArg.Builder` |                       | optional value        |
        |                       |                       | [`processorClass`](   |
        |                       |                       | JavaAnnotationProcess |
        |                       |                       | orDescriptionArg.html |
        |                       |                       | #getProcessorClass()) |
        |                       |                       | to processorClass.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Java                 | `setProces            | ::: block             |
        | AnnotationProcessorDe | sorClass​(Optional<Str | Initializes the       |
        | scriptionArg.Builder` | ing> processorClass)` | optional value        |
        |                       |                       | [`processorClass`](   |
        |                       |                       | JavaAnnotationProcess |
        |                       |                       | orDescriptionArg.html |
        |                       |                       | #getProcessorClass()) |
        |                       |                       | to processorClass.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Java                 | `setPr                | ::: block             |
        | AnnotationProcessorDe | ocessorClasses​(Iterab | Sets or replaces all  |
        | scriptionArg.Builder` | le<String> elements)` | elements for          |
        |                       |                       | [`                    |
        |                       |                       | processorClasses`](Ja |
        |                       |                       | vaAnnotationProcessor |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etProcessorClasses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Java                 | `setSupportsAb        | ::: block             |
        | AnnotationProcessorDe | iGenerationFromSource | Initializes the value |
        | scriptionArg.Builder` | ​(boolean supportsAbiG | for the               |
        |                       | enerationFromSource)` | [`supports            |
        |                       |                       | AbiGenerationFromSour |
        |                       |                       | ce`](JavaAnnotationPr |
        |                       |                       | ocessorDescriptionArg |
        |                       |                       | .html#isSupportsAbiGe |
        |                       |                       | nerationFromSource()) |
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

        []{#from(com.facebook.buck.jvm.java.JavacPluginArgs)}

        -   #### from

            ``` methodSignature
            public final JavaAnnotationProcessorDescriptionArg.Builder from​(JavacPluginArgs instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.jvm.java.JavacPluginArgs` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.jvm.java.JavaAnnotationProcessorDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final JavaAnnotationProcessorDescriptionArg.Builder from​(JavaAnnotationProcessorDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `JavaAnnotationProcessorDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.jvm.java.JavaAnnotationProcessorDescription.AbstractJavaAnnotationProcessorDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final JavaAnnotationProcessorDescriptionArg.Builder from​(com.facebook.buck.jvm.java.JavaAnnotationProcessorDescription.AbstractJavaAnnotationProcessorDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type
            `AbstractJavaAnnotationProcessorDescriptionArg` instance
            into builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.HasDeclaredDeps)}

        -   #### from

            ``` methodSignature
            public final JavaAnnotationProcessorDescriptionArg.Builder from​(HasDeclaredDeps instance)
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
            public final JavaAnnotationProcessorDescriptionArg.Builder from​(BuildRuleArg instance)
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
            public final JavaAnnotationProcessorDescriptionArg.Builder from​(ConstructorArg instance)
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

        []{#setProcessorClass(java.lang.String)}

        -   #### setProcessorClass

            ``` methodSignature
            public final JavaAnnotationProcessorDescriptionArg.Builder setProcessorClass​(String processorClass)
            ```

            ::: block
            Initializes the optional value
            [`processorClass`](JavaAnnotationProcessorDescriptionArg.html#getProcessorClass())
            to processorClass.
            :::

            [Parameters:]{.paramLabel}
            :   `processorClass` - The value for processorClass

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setProcessorClass(java.util.Optional)}

        -   #### setProcessorClass

            ``` methodSignature
            public final JavaAnnotationProcessorDescriptionArg.Builder setProcessorClass​(Optional<String> processorClass)
            ```

            ::: block
            Initializes the optional value
            [`processorClass`](JavaAnnotationProcessorDescriptionArg.html#getProcessorClass())
            to processorClass.
            :::

            [Parameters:]{.paramLabel}
            :   `processorClass` - The value for processorClass

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addProcessorClasses(java.lang.String)}

        -   #### addProcessorClasses

            ``` methodSignature
            public final JavaAnnotationProcessorDescriptionArg.Builder addProcessorClasses​(String element)
            ```

            ::: block
            Adds one element to
            [`processorClasses`](JavaAnnotationProcessorDescriptionArg.html#getProcessorClasses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A processorClasses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addProcessorClasses(java.lang.String...)}

        -   #### addProcessorClasses

            ``` methodSignature
            public final JavaAnnotationProcessorDescriptionArg.Builder addProcessorClasses​(String... elements)
            ```

            ::: block
            Adds elements to
            [`processorClasses`](JavaAnnotationProcessorDescriptionArg.html#getProcessorClasses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of processorClasses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setProcessorClasses(java.lang.Iterable)}

        -   #### setProcessorClasses

            ``` methodSignature
            public final JavaAnnotationProcessorDescriptionArg.Builder setProcessorClasses​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`processorClasses`](JavaAnnotationProcessorDescriptionArg.html#getProcessorClasses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of processorClasses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllProcessorClasses(java.lang.Iterable)}

        -   #### addAllProcessorClasses

            ``` methodSignature
            public final JavaAnnotationProcessorDescriptionArg.Builder addAllProcessorClasses​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`processorClasses`](JavaAnnotationProcessorDescriptionArg.html#getProcessorClasses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of processorClasses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setIsolateClassLoader(boolean)}

        -   #### setIsolateClassLoader

            ``` methodSignature
            public final JavaAnnotationProcessorDescriptionArg.Builder setIsolateClassLoader​(boolean isolateClassLoader)
            ```

            ::: block
            Initializes the value for the
            [`isolateClassLoader`](JavaAnnotationProcessorDescriptionArg.html#isIsolateClassLoader())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`isolateClassLoader`](JavaAnnotationProcessorDescriptionArg.html#isIsolateClassLoader()).*
            :::

            [Parameters:]{.paramLabel}
            :   `isolateClassLoader` - The value for isolateClassLoader

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDoesNotAffectAbi(boolean)}

        -   #### setDoesNotAffectAbi

            ``` methodSignature
            public final JavaAnnotationProcessorDescriptionArg.Builder setDoesNotAffectAbi​(boolean doesNotAffectAbi)
            ```

            ::: block
            Initializes the value for the
            [`doesNotAffectAbi`](JavaAnnotationProcessorDescriptionArg.html#isDoesNotAffectAbi())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`doesNotAffectAbi`](JavaAnnotationProcessorDescriptionArg.html#isDoesNotAffectAbi()).*
            :::

            [Parameters:]{.paramLabel}
            :   `doesNotAffectAbi` - The value for doesNotAffectAbi

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSupportsAbiGenerationFromSource(boolean)}

        -   #### setSupportsAbiGenerationFromSource

            ``` methodSignature
            public final JavaAnnotationProcessorDescriptionArg.Builder setSupportsAbiGenerationFromSource​(boolean supportsAbiGenerationFromSource)
            ```

            ::: block
            Initializes the value for the
            [`supportsAbiGenerationFromSource`](JavaAnnotationProcessorDescriptionArg.html#isSupportsAbiGenerationFromSource())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`supportsAbiGenerationFromSource`](JavaAnnotationProcessorDescriptionArg.html#isSupportsAbiGenerationFromSource()).*
            :::

            [Parameters:]{.paramLabel}
            :   `supportsAbiGenerationFromSource` - The value for
                supportsAbiGenerationFromSource

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final JavaAnnotationProcessorDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](JavaAnnotationProcessorDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final JavaAnnotationProcessorDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](JavaAnnotationProcessorDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final JavaAnnotationProcessorDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](JavaAnnotationProcessorDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final JavaAnnotationProcessorDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](JavaAnnotationProcessorDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String)}

        -   #### addLabels

            ``` methodSignature
            public final JavaAnnotationProcessorDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](JavaAnnotationProcessorDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final JavaAnnotationProcessorDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](JavaAnnotationProcessorDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final JavaAnnotationProcessorDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](JavaAnnotationProcessorDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final JavaAnnotationProcessorDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](JavaAnnotationProcessorDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final JavaAnnotationProcessorDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](JavaAnnotationProcessorDescriptionArg.html#getDefaultTargetPlatform())
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
            public final JavaAnnotationProcessorDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](JavaAnnotationProcessorDescriptionArg.html#getDefaultTargetPlatform())
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
            public final JavaAnnotationProcessorDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](JavaAnnotationProcessorDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final JavaAnnotationProcessorDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](JavaAnnotationProcessorDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final JavaAnnotationProcessorDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](JavaAnnotationProcessorDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final JavaAnnotationProcessorDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](JavaAnnotationProcessorDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final JavaAnnotationProcessorDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](JavaAnnotationProcessorDescriptionArg.html#getName())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addDeps

            ``` methodSignature
            public final JavaAnnotationProcessorDescriptionArg.Builder addDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`deps`](JavaAnnotationProcessorDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A deps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addDeps

            ``` methodSignature
            public final JavaAnnotationProcessorDescriptionArg.Builder addDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`deps`](JavaAnnotationProcessorDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDeps(java.lang.Iterable)}

        -   #### setDeps

            ``` methodSignature
            public final JavaAnnotationProcessorDescriptionArg.Builder setDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`deps`](JavaAnnotationProcessorDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllDeps(java.lang.Iterable)}

        -   #### addAllDeps

            ``` methodSignature
            public final JavaAnnotationProcessorDescriptionArg.Builder addAllDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`deps`](JavaAnnotationProcessorDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public JavaAnnotationProcessorDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`JavaAnnotationProcessorDescriptionArg`](JavaAnnotationProcessorDescriptionArg.html "class in com.facebook.buck.jvm.java").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of
                JavaAnnotationProcessorDescriptionArg

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

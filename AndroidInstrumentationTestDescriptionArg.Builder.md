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

## Class AndroidInstrumentationTestDescriptionArg.Builder {#class-androidinstrumentationtestdescriptionarg.builder .title title="Class AndroidInstrumentationTestDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.AndroidInstrumentationTestDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [AndroidInstrumentationTestDescriptionArg](AndroidInstrumentationTestDescriptionArg.html "class in com.facebook.buck.android")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class AndroidInstrumentationTestDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`AndroidInstrumentationTestDescriptionArg`](AndroidInstrumentationTestDescriptionArg.html "class in com.facebook.buck.android").
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
        | `Android              | `addAllCompat         | ::: block             |
        | InstrumentationTestDe | ibleWith​(Iterable<? e | Adds elements to      |
        | scriptionArg.Builder` | xtends UnconfiguredBu | [                     |
        |                       | ildTarget> elements)` | `compatibleWith`](And |
        |                       |                       | roidInstrumentationTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Android              | `                     | ::: block             |
        | InstrumentationTestDe | addAllContacts​(Iterab | Adds elements to      |
        | scriptionArg.Builder` | le<String> elements)` | [`contacts            |
        |                       |                       | `](AndroidInstrumenta |
        |                       |                       | tionTestDescriptionAr |
        |                       |                       | g.html#getContacts()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Android              | `addAllLabels​(Iterab  | ::: block             |
        | InstrumentationTestDe | le<String> elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`labe                |
        |                       |                       | ls`](AndroidInstrumen |
        |                       |                       | tationTestDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Android              | `addAllLicenses       | ::: block             |
        | InstrumentationTestDe | ​(Iterable<? extends S | Adds elements to      |
        | scriptionArg.Builder` | ourcePath> elements)` | [`licenses            |
        |                       |                       | `](AndroidInstrumenta |
        |                       |                       | tionTestDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Android              | `addCompat            | ::: block             |
        | InstrumentationTestDe | ibleWith​(Unconfigured | Adds one element to   |
        | scriptionArg.Builder` | BuildTarget element)` | [                     |
        |                       |                       | `compatibleWith`](And |
        |                       |                       | roidInstrumentationTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Android              | `addCompatible        | ::: block             |
        | InstrumentationTestDe | With​(UnconfiguredBuil | Adds elements to      |
        | scriptionArg.Builder` | dTarget... elements)` | [                     |
        |                       |                       | `compatibleWith`](And |
        |                       |                       | roidInstrumentationTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Android              | `addCont              | ::: block             |
        | InstrumentationTestDe | acts​(String element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`contacts            |
        |                       |                       | `](AndroidInstrumenta |
        |                       |                       | tionTestDescriptionAr |
        |                       |                       | g.html#getContacts()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Android              | `addContacts          | ::: block             |
        | InstrumentationTestDe | ​(String... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`contacts            |
        |                       |                       | `](AndroidInstrumenta |
        |                       |                       | tionTestDescriptionAr |
        |                       |                       | g.html#getContacts()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Android              | `addLa                | ::: block             |
        | InstrumentationTestDe | bels​(String element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`labe                |
        |                       |                       | ls`](AndroidInstrumen |
        |                       |                       | tationTestDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Android              | `addLabels            | ::: block             |
        | InstrumentationTestDe | ​(String... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`labe                |
        |                       |                       | ls`](AndroidInstrumen |
        |                       |                       | tationTestDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Android              | `addLicenses          | ::: block             |
        | InstrumentationTestDe | ​(SourcePath element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`licenses            |
        |                       |                       | `](AndroidInstrumenta |
        |                       |                       | tionTestDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Android              | `addLicenses​(Sou      | ::: block             |
        | InstrumentationTestDe | rcePath... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`licenses            |
        |                       |                       | `](AndroidInstrumenta |
        |                       |                       | tionTestDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidInstrumentati | `build()`             | ::: block             |
        | onTestDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`A                   |
        |                       |                       | ndroidInstrumentation |
        |                       |                       | TestDescriptionArg`]( |
        |                       |                       | AndroidInstrumentatio |
        |                       |                       | nTestDescriptionArg.h |
        |                       |                       | tml "class in com.fac |
        |                       |                       | ebook.buck.android"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Android              | `fr                   | ::: block             |
        | InstrumentationTestDe | om​(com.facebook.buck. | Copy abstract value   |
        | scriptionArg.Builder` | android.AndroidInstru | type                  |
        |                       | mentationTestDescript | `Abstrac              |
        |                       | ion.AbstractAndroidIn | tAndroidInstrumentati |
        |                       | strumentationTestDesc | onTestDescriptionArg` |
        |                       | riptionArg instance)` | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Android              | `from​(AndroidIn       | ::: block             |
        | InstrumentationTestDe | strumentationTestDesc | Fill a builder with   |
        | scriptionArg.Builder` | riptionArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `AndroidInstrumentati |
        |                       |                       | onTestDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Android              | `from​(Bu              | ::: block             |
        | InstrumentationTestDe | ildRuleArg instance)` | Fill a builder with   |
        | scriptionArg.Builder` |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Android              | `from​(Cons            | ::: block             |
        | InstrumentationTestDe | tructorArg instance)` | Fill a builder with   |
        | scriptionArg.Builder` |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Android              | `from​(H               | ::: block             |
        | InstrumentationTestDe | asContacts instance)` | Fill a builder with   |
        | scriptionArg.Builder` |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.faceb            |
        |                       |                       | ook.buck.core.descrip |
        |                       |                       | tion.arg.HasContacts` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Android              | `from​(HasT            | ::: block             |
        | InstrumentationTestDe | estTimeout instance)` | Fill a builder with   |
        | scriptionArg.Builder` |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.HasTestTimeout` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Android              | `set                  | ::: block             |
        | InstrumentationTestDe | Apk​(BuildTarget apk)` | Initializes the value |
        | scriptionArg.Builder` |                       | for the               |
        |                       |                       | [`apk`](AndroidInstru |
        |                       |                       | mentationTestDescript |
        |                       |                       | ionArg.html#getApk()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Android              | `setCompat            | ::: block             |
        | InstrumentationTestDe | ibleWith​(Iterable<? e | Sets or replaces all  |
        | scriptionArg.Builder` | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [                     |
        |                       |                       | `compatibleWith`](And |
        |                       |                       | roidInstrumentationTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Android              | `setContacts​(Iterab   | ::: block             |
        | InstrumentationTestDe | le<String> elements)` | Sets or replaces all  |
        | scriptionArg.Builder` |                       | elements for          |
        |                       |                       | [`contacts            |
        |                       |                       | `](AndroidInstrumenta |
        |                       |                       | tionTestDescriptionAr |
        |                       |                       | g.html#getContacts()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Android              | `setDefaul            | ::: block             |
        | InstrumentationTestDe | tTargetPlatform​(Uncon | Initializes the       |
        | scriptionArg.Builder` | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`defaultTarget       |
        |                       |                       | Platform`](AndroidIns |
        |                       |                       | trumentationTestDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Android              | `setDefau             | ::: block             |
        | InstrumentationTestDe | ltTargetPlatform​(Opti | Initializes the       |
        | scriptionArg.Builder` | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`defaultTarget       |
        |                       | faultTargetPlatform)` | Platform`](AndroidIns |
        |                       |                       | trumentationTestDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Android              | `setLabels​(Iterab     | ::: block             |
        | InstrumentationTestDe | le<String> elements)` | Sets or replaces all  |
        | scriptionArg.Builder` |                       | elements for          |
        |                       |                       | [`labe                |
        |                       |                       | ls`](AndroidInstrumen |
        |                       |                       | tationTestDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Android              | `setLicenses          | ::: block             |
        | InstrumentationTestDe | ​(Iterable<? extends S | Sets or replaces all  |
        | scriptionArg.Builder` | ourcePath> elements)` | elements for          |
        |                       |                       | [`licenses            |
        |                       |                       | `](AndroidInstrumenta |
        |                       |                       | tionTestDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Android              | `                     | ::: block             |
        | InstrumentationTestDe | setName​(String name)` | Initializes the value |
        | scriptionArg.Builder` |                       | for the               |
        |                       |                       | [`                    |
        |                       |                       | name`](AndroidInstrum |
        |                       |                       | entationTestDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Android              | `set                  | ::: block             |
        | InstrumentationTestDe | TestRuleTimeoutMs​(lon | Initializes the       |
        | scriptionArg.Builder` | g testRuleTimeoutMs)` | optional value        |
        |                       |                       | [`testR               |
        |                       |                       | uleTimeoutMs`](Androi |
        |                       |                       | dInstrumentationTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tTestRuleTimeoutMs()) |
        |                       |                       | to testRuleTimeoutMs. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Android              | `setTestRuleTi        | ::: block             |
        | InstrumentationTestDe | meoutMs​(Optional<Long | Initializes the       |
        | scriptionArg.Builder` | > testRuleTimeoutMs)` | optional value        |
        |                       |                       | [`testR               |
        |                       |                       | uleTimeoutMs`](Androi |
        |                       |                       | dInstrumentationTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tTestRuleTimeoutMs()) |
        |                       |                       | to testRuleTimeoutMs. |
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

        []{#from(com.facebook.buck.core.description.arg.HasTestTimeout)}

        -   #### from

            ``` methodSignature
            public final AndroidInstrumentationTestDescriptionArg.Builder from​(HasTestTimeout instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.core.description.arg.HasTestTimeout`
            instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.BuildRuleArg)}

        -   #### from

            ``` methodSignature
            public final AndroidInstrumentationTestDescriptionArg.Builder from​(BuildRuleArg instance)
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

        []{#from(com.facebook.buck.core.description.arg.HasContacts)}

        -   #### from

            ``` methodSignature
            public final AndroidInstrumentationTestDescriptionArg.Builder from​(HasContacts instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.core.description.arg.HasContacts`
            instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.android.AndroidInstrumentationTestDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final AndroidInstrumentationTestDescriptionArg.Builder from​(AndroidInstrumentationTestDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `AndroidInstrumentationTestDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.android.AndroidInstrumentationTestDescription.AbstractAndroidInstrumentationTestDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final AndroidInstrumentationTestDescriptionArg.Builder from​(com.facebook.buck.android.AndroidInstrumentationTestDescription.AbstractAndroidInstrumentationTestDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type
            `AbstractAndroidInstrumentationTestDescriptionArg` instance
            into builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.ConstructorArg)}

        -   #### from

            ``` methodSignature
            public final AndroidInstrumentationTestDescriptionArg.Builder from​(ConstructorArg instance)
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

        []{#setApk(com.facebook.buck.core.model.BuildTarget)}

        -   #### setApk

            ``` methodSignature
            public final AndroidInstrumentationTestDescriptionArg.Builder setApk​(BuildTarget apk)
            ```

            ::: block
            Initializes the value for the
            [`apk`](AndroidInstrumentationTestDescriptionArg.html#getApk())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `apk` - The value for apk

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final AndroidInstrumentationTestDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](AndroidInstrumentationTestDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final AndroidInstrumentationTestDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](AndroidInstrumentationTestDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final AndroidInstrumentationTestDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](AndroidInstrumentationTestDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final AndroidInstrumentationTestDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](AndroidInstrumentationTestDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String)}

        -   #### addLabels

            ``` methodSignature
            public final AndroidInstrumentationTestDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](AndroidInstrumentationTestDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final AndroidInstrumentationTestDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](AndroidInstrumentationTestDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final AndroidInstrumentationTestDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](AndroidInstrumentationTestDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final AndroidInstrumentationTestDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](AndroidInstrumentationTestDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final AndroidInstrumentationTestDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](AndroidInstrumentationTestDescriptionArg.html#getDefaultTargetPlatform())
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
            public final AndroidInstrumentationTestDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](AndroidInstrumentationTestDescriptionArg.html#getDefaultTargetPlatform())
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
            public final AndroidInstrumentationTestDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](AndroidInstrumentationTestDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final AndroidInstrumentationTestDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](AndroidInstrumentationTestDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final AndroidInstrumentationTestDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](AndroidInstrumentationTestDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final AndroidInstrumentationTestDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](AndroidInstrumentationTestDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final AndroidInstrumentationTestDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](AndroidInstrumentationTestDescriptionArg.html#getName())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addContacts(java.lang.String)}

        -   #### addContacts

            ``` methodSignature
            public final AndroidInstrumentationTestDescriptionArg.Builder addContacts​(String element)
            ```

            ::: block
            Adds one element to
            [`contacts`](AndroidInstrumentationTestDescriptionArg.html#getContacts())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A contacts element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addContacts(java.lang.String...)}

        -   #### addContacts

            ``` methodSignature
            public final AndroidInstrumentationTestDescriptionArg.Builder addContacts​(String... elements)
            ```

            ::: block
            Adds elements to
            [`contacts`](AndroidInstrumentationTestDescriptionArg.html#getContacts())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of contacts elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setContacts(java.lang.Iterable)}

        -   #### setContacts

            ``` methodSignature
            public final AndroidInstrumentationTestDescriptionArg.Builder setContacts​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`contacts`](AndroidInstrumentationTestDescriptionArg.html#getContacts())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of contacts elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllContacts(java.lang.Iterable)}

        -   #### addAllContacts

            ``` methodSignature
            public final AndroidInstrumentationTestDescriptionArg.Builder addAllContacts​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`contacts`](AndroidInstrumentationTestDescriptionArg.html#getContacts())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of contacts elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTestRuleTimeoutMs(long)}

        -   #### setTestRuleTimeoutMs

            ``` methodSignature
            public final AndroidInstrumentationTestDescriptionArg.Builder setTestRuleTimeoutMs​(long testRuleTimeoutMs)
            ```

            ::: block
            Initializes the optional value
            [`testRuleTimeoutMs`](AndroidInstrumentationTestDescriptionArg.html#getTestRuleTimeoutMs())
            to testRuleTimeoutMs.
            :::

            [Parameters:]{.paramLabel}
            :   `testRuleTimeoutMs` - The value for testRuleTimeoutMs

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setTestRuleTimeoutMs(java.util.Optional)}

        -   #### setTestRuleTimeoutMs

            ``` methodSignature
            public final AndroidInstrumentationTestDescriptionArg.Builder setTestRuleTimeoutMs​(Optional<Long> testRuleTimeoutMs)
            ```

            ::: block
            Initializes the optional value
            [`testRuleTimeoutMs`](AndroidInstrumentationTestDescriptionArg.html#getTestRuleTimeoutMs())
            to testRuleTimeoutMs.
            :::

            [Parameters:]{.paramLabel}
            :   `testRuleTimeoutMs` - The value for testRuleTimeoutMs

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public AndroidInstrumentationTestDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`AndroidInstrumentationTestDescriptionArg`](AndroidInstrumentationTestDescriptionArg.html "class in com.facebook.buck.android").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of
                AndroidInstrumentationTestDescriptionArg

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

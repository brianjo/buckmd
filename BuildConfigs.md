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
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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

## Class BuildConfigs {#class-buildconfigs .title title="Class BuildConfigs"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.BuildConfigs

::: description
-   

    ------------------------------------------------------------------------

        public class BuildConfigs
        extends Object

    ::: block
    Utilities for generating a `BuildConfig.java` file for Android.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Field                 | Description           |
        +=======================+=======================+=======================+
        | `static String`       | `DEBUG_CONSTANT`      | ::: block             |
        |                       |                       | Name of the boolean   |
        |                       |                       | global variable       |
        |                       |                       | provided by the       |
        |                       |                       | standard Android      |
        |                       |                       | tools to indicate     |
        |                       |                       | whether an app was    |
        |                       |                       | built in debug mode   |
        |                       |                       | or not.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `EXOPACKAGE_FLAGS`    | ::: block             |
        |                       |                       | Name of a global      |
        |                       |                       | variable that         |
        |                       |                       | includes the          |
        |                       |                       | exopackage            |
        |                       |                       | configuration as a    |
        |                       |                       | bitmask.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `IS_EXO_CONSTANT`     | ::: block             |
        |                       |                       | Name of a             |
        |                       |                       | Buck-specific global  |
        |                       |                       | variable that         |
        |                       |                       | indicates whether an  |
        |                       |                       | app was built using   |
        |                       |                       | exopackage.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static String`       | `generateBuildConfig  | ::: block             |
        |                       | DotJava​(UnflavoredBui | Generates the source  |
        |                       | ldTarget source,      | code for an Android   |
        |                       |                       | `BuildConfig.java`    |
        |                       |  String javaPackage)` | file with the default |
        |                       |                       | set of fields         |
        |                       |                       | specified by          |
        |                       |                       | [`g                   |
        |                       |                       | etDefaultBuildConfigF |
        |                       |                       | ields()`](#getDefault |
        |                       |                       | BuildConfigFields()). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `generat              | ::: block             |
        |                       | eBuildConfigDotJava​(U | Generates the source  |
        |                       | nflavoredBuildTarget  | code for an Android   |
        |                       | source,               | `BuildConfig.java`    |
        |                       |              String j | file with fields      |
        |                       | avaPackage,           | specified by          |
        |                       |                  bool | `userFields`.         |
        |                       | ean useConstantExpres | :::                   |
        |                       | sions,                |                       |
        |                       |             BuildConf |                       |
        |                       | igFields userFields)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `stat                 | `getDefaul            | ::: block             |
        | ic BuildConfigFields` | tBuildConfigFields()` | Returns a list of     |
        |                       |                       | fields (with values)  |
        |                       |                       | that every            |
        |                       |                       | `BuildConfig.java`    |
        |                       |                       | should declare.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#DEBUG_CONSTANT}

        -   #### DEBUG_CONSTANT

                public static final String DEBUG_CONSTANT

            ::: block
            Name of the boolean global variable provided by the standard
            Android tools to indicate whether an app was built in debug
            mode or not.
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.android.BuildConfigs.DEBUG_CONSTANT)

        []{#IS_EXO_CONSTANT}

        -   #### IS_EXO_CONSTANT

                public static final String IS_EXO_CONSTANT

            ::: block
            Name of a Buck-specific global variable that indicates
            whether an app was built using exopackage.
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.android.BuildConfigs.IS_EXO_CONSTANT)

        []{#EXOPACKAGE_FLAGS}

        -   #### EXOPACKAGE_FLAGS

                public static final String EXOPACKAGE_FLAGS

            ::: block
            Name of a global variable that includes the exopackage
            configuration as a bitmask.
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.android.BuildConfigs.EXOPACKAGE_FLAGS)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getDefaultBuildConfigFields()}

        -   #### getDefaultBuildConfigFields

            ``` methodSignature
            public static BuildConfigFields getDefaultBuildConfigFields()
            ```

            ::: block
            Returns a list of fields (with values) that every
            `BuildConfig.java` should declare. The default value of each
            constant may be overridden by the `userFields` passed to
            [`generateBuildConfigDotJava(UnflavoredBuildTarget, String, boolean, BuildConfigFields)`](#generateBuildConfigDotJava(com.facebook.buck.core.model.UnflavoredBuildTarget,java.lang.String,boolean,com.facebook.buck.rules.coercer.BuildConfigFields))
            when generating a `BuildConfig.java`.
            :::

        []{#generateBuildConfigDotJava(com.facebook.buck.core.model.UnflavoredBuildTarget,java.lang.String)}

        -   #### generateBuildConfigDotJava

            ``` methodSignature
            public static String generateBuildConfigDotJava​(UnflavoredBuildTarget source,
                                                            String javaPackage)
            ```

            ::: block
            Generates the source code for an Android `BuildConfig.java`
            file with the default set of fields specified by
            [`getDefaultBuildConfigFields()`](#getDefaultBuildConfigFields()).
            :::

        []{#generateBuildConfigDotJava(com.facebook.buck.core.model.UnflavoredBuildTarget,java.lang.String,boolean,com.facebook.buck.rules.coercer.BuildConfigFields)}

        -   #### generateBuildConfigDotJava

            ``` methodSignature
            public static String generateBuildConfigDotJava​(UnflavoredBuildTarget source,
                                                            String javaPackage,
                                                            boolean useConstantExpressions,
                                                            BuildConfigFields userFields)
            ```

            ::: block
            Generates the source code for an Android `BuildConfig.java`
            file with fields specified by `userFields`.
            The output will also contain a constant for every entry in
            the collection returned by
            [`getDefaultBuildConfigFields()`](#getDefaultBuildConfigFields()).

            If the name of a field in `userFields` matches one in the
            collection returned by
            [`getDefaultBuildConfigFields()`](#getDefaultBuildConfigFields()),
            the value in the `userFields` map will be used.
            :::

            [Parameters:]{.paramLabel}
            :   `javaPackage` - The package for the Java class generated
                by this method.
            :   `useConstantExpressions` - If `true`, the value for each
                static final field in the generated class will be
                declared as the literal value in `userFields`. The
                values of such fields can be inlined by `javac`.

                If `false`, the value for each static final field in the
                generated class will be declared as a non-constant
                expression that is guaranteed to evaluate to the same
                value in `userFields`. This ensures that the generated
                `BuildConfig.java` can still be used in Robolectric
                tests, but does not run the risk of its values being
                inlined by `      javac`. This is important if the
                generated `BuildConfig` class is going to be swapped out
                by a different implementation by
                [`AndroidBinary`](AndroidBinary.html "class in com.facebook.buck.android").
                See
                [`AndroidBuildConfig`](AndroidBuildConfig.html "class in com.facebook.buck.android")
                for details.
            :   `userFields` - represents the fields that should be
                declared in the generated `      BuildConfig` class.
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
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

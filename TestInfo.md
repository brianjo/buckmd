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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.providers.lib](package-summary.html)
:::

## Class TestInfo {#class-testinfo .title title="Class TestInfo"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.starlark.compatible.BuckStarlarkStructObject](../../../starlark/compatible/BuckStarlarkStructObject.html "class in com.facebook.buck.core.starlark.compatible")

    -   -   [com.facebook.buck.core.rules.providers.impl.BuiltInProviderInfo](../impl/BuiltInProviderInfo.html "class in com.facebook.buck.core.rules.providers.impl")\<[TestInfo](TestInfo.html "class in com.facebook.buck.core.rules.providers.lib")\>

        -   -   com.facebook.buck.core.rules.providers.lib.TestInfo

::: description
-   

    All Implemented Interfaces:
    :   `ProviderInfo<TestInfo>`, `SkylarkProviderInfo`,
        `com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable`,
        `com.google.devtools.build.lib.skylarkinterface.SkylarkValue`,
        `com.google.devtools.build.lib.syntax.ClassObject`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `ImmutableTestInfo`

    ------------------------------------------------------------------------

        public abstract class TestInfo
        extends BuiltInProviderInfo<TestInfo>

    ::: block
    Provider that passes along information needed by the buck test
    runner / external test runners
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                    Field        Description
          ------------------------------------ ------------ -------------
          `static BuiltInProvider<TestInfo>`   `PROVIDER`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor    Description
          -------------- -------------
          `TestInfo()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `abstract com.g       | `contacts()`          |                       |
        | oogle.common.collect. |                       |                       |
        | ImmutableSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static TestInfo`     | `                     | ::: block             |
        |                       | instantiateFromSkylar | Create an instance    |
        |                       | k​(String testName,    | from skylark objects  |
        |                       |                     S | :::                   |
        |                       | tring testCaseName,   |                       |
        |                       |                       |                       |
        |                       | com.google.devtools.b |                       |
        |                       | uild.lib.syntax.Skyla |                       |
        |                       | rkList<String> labels |                       |
        |                       | ,                     |                       |
        |                       |    com.google.devtool |                       |
        |                       | s.build.lib.syntax.Sk |                       |
        |                       | ylarkList<String> con |                       |
        |                       | tacts,                |                       |
        |                       |         Object timeou |                       |
        |                       | tMs,                  |                       |
        |                       |       boolean runTest |                       |
        |                       | sSeparately,          |                       |
        |                       |               String  |                       |
        |                       | type,                 |                       |
        |                       |        com.google.dev |                       |
        |                       | tools.build.lib.event |                       |
        |                       | s.Location location)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract com.g       | `labels()`            |                       |
        | oogle.common.collect. |                       |                       |
        | ImmutableSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static TestInfo`     | `o                    | ::: block             |
        |                       | f​(String testName,    | Create an instance    |
        |                       | String testCaseName,  | from native values    |
        |                       |   com.google.common.c | :::                   |
        |                       | ollect.ImmutableSet<S |                       |
        |                       | tring> labels,   com. |                       |
        |                       | google.common.collect |                       |
        |                       | .ImmutableSet<String> |                       |
        |                       |  contacts,   Optional |                       |
        |                       | <Long> timeoutMs,   b |                       |
        |                       | oolean runTestsSepara |                       |
        |                       | tely,   String type)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract boolean`    | `                     |                       |
        |                       | runTestsSeparately()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract String`     | `testCaseName()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract String`     | `testName()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Object`     | `timeoutMs()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract String`     | `type()`              |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Long>`      | `typedTimeoutMs()`    |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.providers.impl.BuiltInProviderInfo}

            ### Methods inherited from class com.facebook.buck.core.rules.providers.impl.[BuiltInProviderInfo](../impl/BuiltInProviderInfo.html "class in com.facebook.buck.core.rules.providers.impl")

            `getDeclaredClass, getProvider, getProviderInfo, isImmutable`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.starlark.compatible.BuckStarlarkStructObject}

            ### Methods inherited from class com.facebook.buck.core.starlark.compatible.[BuckStarlarkStructObject](../../../starlark/compatible/BuckStarlarkStructObject.html "class in com.facebook.buck.core.starlark.compatible")

            `getErrorMessageForUnknownField, getFieldNames, getMethods, getValue, repr`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable}

            ### Methods inherited from interface com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable

            `debugPrint, repr, str`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.google.devtools.build.lib.skylarkinterface.SkylarkValue}

            ### Methods inherited from interface com.google.devtools.build.lib.skylarkinterface.SkylarkValue

            `isHashable`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#PROVIDER}

        -   #### PROVIDER

                public static final BuiltInProvider<TestInfo> PROVIDER
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### TestInfo

                public TestInfo()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#testName()}

        -   #### testName

            ``` methodSignature
            public abstract String testName()
            ```

            [Returns:]{.returnLabel}
            :   the type of test. This should generally be the rule name

        []{#testCaseName()}

        -   #### testCaseName

            ``` methodSignature
            public abstract String testCaseName()
            ```

            [Returns:]{.returnLabel}
            :   the name of the test case

        []{#labels()}

        -   #### labels

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSet<String> labels()
            ```

        []{#contacts()}

        -   #### contacts

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSet<String> contacts()
            ```

        []{#timeoutMs()}

        -   #### timeoutMs

            ``` methodSignature
            public abstract Object timeoutMs()
            ```

        []{#runTestsSeparately()}

        -   #### runTestsSeparately

            ``` methodSignature
            public abstract boolean runTestsSeparately()
            ```

        []{#type()}

        -   #### type

            ``` methodSignature
            public abstract String type()
            ```

            [Returns:]{.returnLabel}
            :   the \'type\' to pass to the external test runner

        []{#typedTimeoutMs()}

        -   #### typedTimeoutMs

            ``` methodSignature
            @Lazy
            public Optional<Long> typedTimeoutMs()
            ```

        []{#of(java.lang.String,java.lang.String,com.google.common.collect.ImmutableSet,com.google.common.collect.ImmutableSet,java.util.Optional,boolean,java.lang.String)}

        -   #### of

            ``` methodSignature
            public static TestInfo of​(String testName,
                                      String testCaseName,
                                      com.google.common.collect.ImmutableSet<String> labels,
                                      com.google.common.collect.ImmutableSet<String> contacts,
                                      Optional<Long> timeoutMs,
                                      boolean runTestsSeparately,
                                      String type)
            ```

            ::: block
            Create an instance from native values
            :::

        []{#instantiateFromSkylark(java.lang.String,java.lang.String,com.google.devtools.build.lib.syntax.SkylarkList,com.google.devtools.build.lib.syntax.SkylarkList,java.lang.Object,boolean,java.lang.String,com.google.devtools.build.lib.events.Location)}

        -   #### instantiateFromSkylark

            ``` methodSignature
            public static TestInfo instantiateFromSkylark​(String testName,
                                                          String testCaseName,
                                                          com.google.devtools.build.lib.syntax.SkylarkList<String> labels,
                                                          com.google.devtools.build.lib.syntax.SkylarkList<String> contacts,
                                                          Object timeoutMs,
                                                          boolean runTestsSeparately,
                                                          String type,
                                                          com.google.devtools.build.lib.events.Location location)
                                                   throws com.google.devtools.build.lib.syntax.EvalException
            ```

            ::: block
            Create an instance from skylark objects
            :::

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`
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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

<div>

-   Summary: 
-   Nested \| 
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

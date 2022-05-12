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
-   [Enum Constants](#enum.constant.summary) \| 
-   Field \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Enum Constants](#enum.constant.detail) \| 
-   Field \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.features.project.intellij.model](package-summary.html)
:::

## Enum IjModuleType {#enum-ijmoduletype .title title="Enum IjModuleType"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<[IjModuleType](IjModuleType.html "enum in com.facebook.buck.features.project.intellij.model")\>

    -   -   com.facebook.buck.features.project.intellij.model.IjModuleType

::: description
-   

    All Implemented Interfaces:
    :   `Serializable`, `Comparable<IjModuleType>`

    ------------------------------------------------------------------------

        public enum IjModuleType
        extends Enum<IjModuleType>

    ::: block
    List of module types that are recognized by the model.
    The types in this enum are ordered by priority. When multiple
    targets apply the type on a module only the type with the highest
    priority is used as the result type.

    For example, if one target\'s rule sets the type to ANDROID_MODULE
    and another target\'s rule sets it to JAVA_MODULE, the final module
    type would be ANDROID_MODULE.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#enum.constant.summary}

        ### Enum Constant Summary

        +-----------------------------------+-----------------------------------+
        | Enum Constant                     | Description                       |
        +===================================+===================================+
        | `ANDROID_MODULE`                  | ::: block                         |
        |                                   | A module with code that does not  |
        |                                   | contain Android resources.        |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `ANDROID_RESOURCES_MODULE`        | ::: block                         |
        |                                   | Similar to                        |
        |                                   | [`                                |
        |                                   | ANDROID_MODULE`](#ANDROID_MODULE) |
        |                                   | but can contain Android resources |
        |                                   | and thus cannot be aggregated     |
        |                                   | with a module located in the      |
        |                                   | parent directory.                 |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `INTELLIJ_PLUGIN_MODULE`          | ::: block                         |
        |                                   | Modules that contain IntelliJ     |
        |                                   | plugins use this custom type to   |
        |                                   | indicate that they should be run  |
        |                                   | in an environment with an IDEA    |
        |                                   | installation.                     |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `JAVA_MODULE`                     |                                   |
        +-----------------------------------+-----------------------------------+
        | `PYTHON_MODULE`                   |                                   |
        +-----------------------------------+-----------------------------------+
        | `UNKNOWN_MODULE`                  |                                   |
        +-----------------------------------+-----------------------------------+

        : Enum Constants[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `boolean`             | `canBe                |                       |
        |                       | Aggregated​(IjProjectC |                       |
        |                       | onfig projectConfig)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getAggreg            |                       |
        |                       | ationLimit​(IjProjectC |                       |
        |                       | onfig projectConfig)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getImlModuleType()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstr                | `                     |                       |
        | act Optional<String>` | getSdkName​(IjProjectC |                       |
        |                       | onfig projectConfig)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract String`     | `                     |                       |
        |                       | getSdkType​(IjProjectC |                       |
        |                       | onfig projectConfig)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `hasHi                |                       |
        |                       | gherPriorityThan​(IjMo |                       |
        |                       | duleType moduleType)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static IjModuleType` | `                     | ::: block             |
        |                       | valueOf​(String name)` | Returns the enum      |
        |                       |                       | constant of this type |
        |                       |                       | with the specified    |
        |                       |                       | name.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `s                    | `values()`            | ::: block             |
        | tatic IjModuleType[]` |                       | Returns an array      |
        |                       |                       | containing the        |
        |                       |                       | constants of this     |
        |                       |                       | enum type, in the     |
        |                       |                       | order they are        |
        |                       |                       | declared.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Enum}

            ### Methods inherited from class java.lang.[Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, compareTo, equals, finalize, getDeclaringClass, hashCode, name, ordinal, toString, valueOf`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `getClass, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#enum.constant.detail}

        ### Enum Constant Detail

        []{#INTELLIJ_PLUGIN_MODULE}

        -   #### INTELLIJ_PLUGIN_MODULE

                public static final IjModuleType INTELLIJ_PLUGIN_MODULE

            ::: block
            Modules that contain IntelliJ plugins use this custom type
            to indicate that they should be run in an environment with
            an IDEA installation.
            :::

        []{#ANDROID_RESOURCES_MODULE}

        -   #### ANDROID_RESOURCES_MODULE

                public static final IjModuleType ANDROID_RESOURCES_MODULE

            ::: block
            Similar to [`ANDROID_MODULE`](#ANDROID_MODULE) but can
            contain Android resources and thus cannot be aggregated with
            a module located in the parent directory.
            :::

        []{#ANDROID_MODULE}

        -   #### ANDROID_MODULE

                public static final IjModuleType ANDROID_MODULE

            ::: block
            A module with code that does not contain Android resources.
            :::

            [See Also:]{.seeLabel}
            :   [`ANDROID_RESOURCES_MODULE`](#ANDROID_RESOURCES_MODULE)

        []{#JAVA_MODULE}

        -   #### JAVA_MODULE

                public static final IjModuleType JAVA_MODULE

        []{#PYTHON_MODULE}

        -   #### PYTHON_MODULE

                public static final IjModuleType PYTHON_MODULE

        []{#UNKNOWN_MODULE}

        -   #### UNKNOWN_MODULE

                public static final IjModuleType UNKNOWN_MODULE
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#values()}

        -   #### values

            ``` methodSignature
            public static IjModuleType[] values()
            ```

            ::: block
            Returns an array containing the constants of this enum type,
            in the order they are declared. This method may be used to
            iterate over the constants as follows:
                for (IjModuleType c : IjModuleType.values())
                    System.out.println(c);
            :::

            [Returns:]{.returnLabel}
            :   an array containing the constants of this enum type, in
                the order they are declared

        []{#valueOf(java.lang.String)}

        -   #### valueOf

            ``` methodSignature
            public static IjModuleType valueOf​(String name)
            ```

            ::: block
            Returns the enum constant of this type with the specified
            name. The string must match *exactly* an identifier used to
            declare an enum constant in this type. (Extraneous
            whitespace characters are not permitted.)
            :::

            [Parameters:]{.paramLabel}
            :   `name` - the name of the enum constant to be returned.

            [Returns:]{.returnLabel}
            :   the enum constant with the specified name

            [Throws:]{.throwsLabel}
            :   `IllegalArgumentException` - if this enum type has no
                constant with the specified name
            :   `NullPointerException` - if the argument is null

        []{#getSdkName(com.facebook.buck.features.project.intellij.model.IjProjectConfig)}

        -   #### getSdkName

            ``` methodSignature
            public abstract Optional<String> getSdkName​(IjProjectConfig projectConfig)
            ```

        []{#getSdkType(com.facebook.buck.features.project.intellij.model.IjProjectConfig)}

        -   #### getSdkType

            ``` methodSignature
            public abstract String getSdkType​(IjProjectConfig projectConfig)
            ```

        []{#canBeAggregated(com.facebook.buck.features.project.intellij.model.IjProjectConfig)}

        -   #### canBeAggregated

            ``` methodSignature
            public boolean canBeAggregated​(IjProjectConfig projectConfig)
            ```

        []{#getImlModuleType()}

        -   #### getImlModuleType

            ``` methodSignature
            public String getImlModuleType()
            ```

        []{#hasHigherPriorityThan(com.facebook.buck.features.project.intellij.model.IjModuleType)}

        -   #### hasHigherPriorityThan

            ``` methodSignature
            public boolean hasHigherPriorityThan​(IjModuleType moduleType)
            ```

        []{#getAggregationLimit(com.facebook.buck.features.project.intellij.model.IjProjectConfig)}

        -   #### getAggregationLimit

            ``` methodSignature
            public int getAggregationLimit​(IjProjectConfig projectConfig)
            ```
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
-   [Enum Constants](#enum.constant.summary) \| 
-   Field \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Enum Constants](#enum.constant.detail) \| 
-   Field \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

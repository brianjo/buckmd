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

## Enum DependencyType {#enum-dependencytype .title title="Enum DependencyType"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<[DependencyType](DependencyType.html "enum in com.facebook.buck.features.project.intellij.model")\>

    -   -   com.facebook.buck.features.project.intellij.model.DependencyType

::: description
-   

    All Implemented Interfaces:
    :   `Serializable`, `Comparable<DependencyType>`

    ------------------------------------------------------------------------

        public enum DependencyType
        extends Enum<DependencyType>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#enum.constant.summary}

        ### Enum Constant Summary

        +-----------------------------------+-----------------------------------+
        | Enum Constant                     | Description                       |
        +===================================+===================================+
        | `COMPILED_SHADOW`                 | ::: block                         |
        |                                   | This dependency means that the    |
        |                                   | other element contains a compiled |
        |                                   | counterpart to this element.      |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `PROD`                            | ::: block                         |
        |                                   | The current                       |
        |                                   | [`IjModule`](IjModule.            |
        |                                   | html "class in com.facebook.buck. |
        |                                   | features.project.intellij.model") |
        |                                   | depends on the other element from |
        |                                   | production (non-test) code.       |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `RUNTIME`                         | ::: block                         |
        |                                   | The current                       |
        |                                   | [`IjModule`](IjModule.            |
        |                                   | html "class in com.facebook.buck. |
        |                                   | features.project.intellij.model") |
        |                                   | depends on the other element from |
        |                                   | runtime only.                     |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `TEST`                            | ::: block                         |
        |                                   | The current                       |
        |                                   | [`IjModule`](IjModule.            |
        |                                   | html "class in com.facebook.buck. |
        |                                   | features.project.intellij.model") |
        |                                   | depends on the other element from |
        |                                   | test code only.                   |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+

        : Enum Constants[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `s                    | `merge​(Depend         |                       |
        | tatic DependencyType` | encyType left,      D |                       |
        |                       | ependencyType right)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static <T> void`     | `putWithMe            |                       |
        |                       | rge​(Map<T,​DependencyT |                       |
        |                       | ype> map,             |                       |
        |                       |  T key,             D |                       |
        |                       | ependencyType value)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `s                    | `                     | ::: block             |
        | tatic DependencyType` | valueOf​(String name)` | Returns the enum      |
        |                       |                       | constant of this type |
        |                       |                       | with the specified    |
        |                       |                       | name.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `values()`            | ::: block             |
        | tic DependencyType[]` |                       | Returns an array      |
        |                       |                       | containing the        |
        |                       |                       | constants of this     |
        |                       |                       | enum type, in the     |
        |                       |                       | order they are        |
        |                       |                       | declared.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
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

        []{#TEST}

        -   #### TEST

                public static final DependencyType TEST

            ::: block
            The current
            [`IjModule`](IjModule.html "class in com.facebook.buck.features.project.intellij.model")
            depends on the other element from test code only. This only
            happens if a particular module contains both test and
            production code and only code in the test folders needs to
            reference the other element.
            :::

        []{#PROD}

        -   #### PROD

                public static final DependencyType PROD

            ::: block
            The current
            [`IjModule`](IjModule.html "class in com.facebook.buck.features.project.intellij.model")
            depends on the other element from production (non-test)
            code.
            :::

        []{#RUNTIME}

        -   #### RUNTIME

                public static final DependencyType RUNTIME

            ::: block
            The current
            [`IjModule`](IjModule.html "class in com.facebook.buck.features.project.intellij.model")
            depends on the other element from runtime only.
            :::

        []{#COMPILED_SHADOW}

        -   #### COMPILED_SHADOW

                public static final DependencyType COMPILED_SHADOW

            ::: block
            This dependency means that the other element contains a
            compiled counterpart to this element. This is used when the
            current element uses BUCK features which cannot be expressed
            in IntelliJ.
            :::
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#values()}

        -   #### values

            ``` methodSignature
            public static DependencyType[] values()
            ```

            ::: block
            Returns an array containing the constants of this enum type,
            in the order they are declared. This method may be used to
            iterate over the constants as follows:
                for (DependencyType c : DependencyType.values())
                    System.out.println(c);
            :::

            [Returns:]{.returnLabel}
            :   an array containing the constants of this enum type, in
                the order they are declared

        []{#valueOf(java.lang.String)}

        -   #### valueOf

            ``` methodSignature
            public static DependencyType valueOf​(String name)
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

        []{#merge(com.facebook.buck.features.project.intellij.model.DependencyType,com.facebook.buck.features.project.intellij.model.DependencyType)}

        -   #### merge

            ``` methodSignature
            public static DependencyType merge​(DependencyType left,
                                               DependencyType right)
            ```

        []{#putWithMerge(java.util.Map,java.lang.Object,com.facebook.buck.features.project.intellij.model.DependencyType)}
        []{#putWithMerge(java.util.Map,T,com.facebook.buck.features.project.intellij.model.DependencyType)}

        -   #### putWithMerge

            ``` methodSignature
            public static <T> void putWithMerge​(Map<T,​DependencyType> map,
                                                T key,
                                                DependencyType value)
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

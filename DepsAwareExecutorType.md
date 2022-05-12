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

-   [Overview](../../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../../index-all.html)
-   [Help](../../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.graph.transformation.executor.factory](package-summary.html)
:::

## Enum DepsAwareExecutorType {#enum-depsawareexecutortype .title title="Enum DepsAwareExecutorType"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<[DepsAwareExecutorType](DepsAwareExecutorType.html "enum in com.facebook.buck.core.graph.transformation.executor.factory")\>

    -   -   com.facebook.buck.core.graph.transformation.executor.factory.DepsAwareExecutorType

::: description
-   

    All Implemented Interfaces:
    :   `WithProbability`, `Serializable`,
        `Comparable<DepsAwareExecutorType>`

    ------------------------------------------------------------------------

        public enum DepsAwareExecutorType
        extends Enum<DepsAwareExecutorType>
        implements WithProbability

    ::: block
    An enumeration for identifying which implementation of the
    [`DepsAwareExecutor`](../DepsAwareExecutor.html "interface in com.facebook.buck.core.graph.transformation.executor")
    to use.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#enum.constant.summary}

        ### Enum Constant Summary

        +-----------------------------------+-----------------------------------+
        | Enum Constant                     | Description                       |
        +===================================+===================================+
        | `DEFAULT`                         | ::: block                         |
        |                                   | use                               |
        |                                   | [`De                              |
        |                                   | faultDepsAwareExecutor`](../impl/ |
        |                                   | DefaultDepsAwareExecutor.html "cl |
        |                                   | ass in com.facebook.buck.core.gra |
        |                                   | ph.transformation.executor.impl") |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `DEFAULT_WITH_LS`                 | ::: block                         |
        |                                   | use                               |
        |                                   | [`DefaultDepsAwareExecutorWithLo  |
        |                                   | calStack`](../impl/DefaultDepsAwa |
        |                                   | reExecutorWithLocalStack.html "cl |
        |                                   | ass in com.facebook.buck.core.gra |
        |                                   | ph.transformation.executor.impl") |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `JAVA_BASED`                      | ::: block                         |
        |                                   | use                               |
        |                                   | [`JavaE                           |
        |                                   | xecutorBackedDefaultDepsAwareExec |
        |                                   | utor`](../impl/JavaExecutorBacked |
        |                                   | DefaultDepsAwareExecutor.html "cl |
        |                                   | ass in com.facebook.buck.core.gra |
        |                                   | ph.transformation.executor.impl") |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `TOPOSORT_BASED`                  | ::: block                         |
        |                                   | use                               |
        |                                   | [`ToposortBasedD                  |
        |                                   | epsAwareExecutor`](../impl/Toposo |
        |                                   | rtBasedDepsAwareExecutor.html "cl |
        |                                   | ass in com.facebook.buck.core.gra |
        |                                   | ph.transformation.executor.impl") |
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
        | `double`              | `getProbability()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static D             | `                     | ::: block             |
        | epsAwareExecutorType` | valueOf​(String name)` | Returns the enum      |
        |                       |                       | constant of this type |
        |                       |                       | with the specified    |
        |                       |                       | name.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Dep           | `values()`            | ::: block             |
        | sAwareExecutorType[]` |                       | Returns an array      |
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

        []{#DEFAULT}

        -   #### DEFAULT

                public static final DepsAwareExecutorType DEFAULT

            ::: block
            use
            [`DefaultDepsAwareExecutor`](../impl/DefaultDepsAwareExecutor.html "class in com.facebook.buck.core.graph.transformation.executor.impl")
            :::

        []{#DEFAULT_WITH_LS}

        -   #### DEFAULT_WITH_LS

                public static final DepsAwareExecutorType DEFAULT_WITH_LS

            ::: block
            use
            [`DefaultDepsAwareExecutorWithLocalStack`](../impl/DefaultDepsAwareExecutorWithLocalStack.html "class in com.facebook.buck.core.graph.transformation.executor.impl")
            :::

        []{#JAVA_BASED}

        -   #### JAVA_BASED

                public static final DepsAwareExecutorType JAVA_BASED

            ::: block
            use
            [`JavaExecutorBackedDefaultDepsAwareExecutor`](../impl/JavaExecutorBackedDefaultDepsAwareExecutor.html "class in com.facebook.buck.core.graph.transformation.executor.impl")
            :::

        []{#TOPOSORT_BASED}

        -   #### TOPOSORT_BASED

                public static final DepsAwareExecutorType TOPOSORT_BASED

            ::: block
            use
            [`ToposortBasedDepsAwareExecutor`](../impl/ToposortBasedDepsAwareExecutor.html "class in com.facebook.buck.core.graph.transformation.executor.impl")
            :::
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#values()}

        -   #### values

            ``` methodSignature
            public static DepsAwareExecutorType[] values()
            ```

            ::: block
            Returns an array containing the constants of this enum type,
            in the order they are declared. This method may be used to
            iterate over the constants as follows:
                for (DepsAwareExecutorType c : DepsAwareExecutorType.values())
                    System.out.println(c);
            :::

            [Returns:]{.returnLabel}
            :   an array containing the constants of this enum type, in
                the order they are declared

        []{#valueOf(java.lang.String)}

        -   #### valueOf

            ``` methodSignature
            public static DepsAwareExecutorType valueOf​(String name)
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

        []{#getProbability()}

        -   #### getProbability

            ``` methodSignature
            public double getProbability()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getProbability` in interface `WithProbability`

            [Returns:]{.returnLabel}
            :   the probability of an item of the enum being selected.
                This should sum up to 1.0 for all items of an enum.
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

-   [Overview](../../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../../index-all.html)
-   [Help](../../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../../allclasses.html)

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

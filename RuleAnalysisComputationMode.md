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
-   [Field](#field.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Enum Constants](#enum.constant.detail) \| 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.analysis.config](package-summary.html)
:::

## Enum RuleAnalysisComputationMode {#enum-ruleanalysiscomputationmode .title title="Enum RuleAnalysisComputationMode"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<[RuleAnalysisComputationMode](RuleAnalysisComputationMode.html "enum in com.facebook.buck.core.rules.analysis.config")\>

    -   -   com.facebook.buck.core.rules.analysis.config.RuleAnalysisComputationMode

::: description
-   

    All Implemented Interfaces:
    :   `Serializable`, `Comparable<RuleAnalysisComputationMode>`

    ------------------------------------------------------------------------

        public enum RuleAnalysisComputationMode
        extends Enum<RuleAnalysisComputationMode>

    ::: block
    Indicates what mode of
    [`RuleAnalysisGraph`](../computation/RuleAnalysisGraph.html "interface in com.facebook.buck.core.rules.analysis.computation")
    should be ran.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#enum.constant.summary}

        ### Enum Constant Summary

        +-----------------------------------+-----------------------------------+
        | Enum Constant                     | Description                       |
        +===================================+===================================+
        | `COMPATIBLE`                      | ::: block                         |
        |                                   | run in combination with existing  |
        |                                   | [`ActionGraphBuilder`](../../Ac   |
        |                                   | tionGraphBuilder.html "interface  |
        |                                   | in com.facebook.buck.core.rules") |
        |                                   | for compatibility                 |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `DISABLED`                        | ::: block                         |
        |                                   | don\'t run                        |
        |                                   | [`RuleAnalysisGraph`](../c        |
        |                                   | omputation/RuleAnalysisGraph.html |
        |                                   |  "interface in com.facebook.buck. |
        |                                   | core.rules.analysis.computation") |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `PROVIDER_COMPATIBLE`             | ::: block                         |
        |                                   | same as                           |
        |                                   | [`COMPATIBLE`](#COMPATIBLE), but  |
        |                                   | also with the ability for rule    |
        |                                   | analysis to depend on providers   |
        |                                   | from action graph                 |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+

        : Enum Constants[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                      Field       Description
          -------------------------------------- ----------- -------------
          `static RuleAnalysisComputationMode`   `DEFAULT`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static RuleAna       | `                     | ::: block             |
        | lysisComputationMode` | valueOf​(String name)` | Returns the enum      |
        |                       |                       | constant of this type |
        |                       |                       | with the specified    |
        |                       |                       | name.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static RuleAnaly     | `values()`            | ::: block             |
        | sisComputationMode[]` |                       | Returns an array      |
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

        []{#DISABLED}

        -   #### DISABLED

                public static final RuleAnalysisComputationMode DISABLED

            ::: block
            don\'t run
            [`RuleAnalysisGraph`](../computation/RuleAnalysisGraph.html "interface in com.facebook.buck.core.rules.analysis.computation")
            :::

        []{#COMPATIBLE}

        -   #### COMPATIBLE

                public static final RuleAnalysisComputationMode COMPATIBLE

            ::: block
            run in combination with existing
            [`ActionGraphBuilder`](../../ActionGraphBuilder.html "interface in com.facebook.buck.core.rules")
            for compatibility
            :::

        []{#PROVIDER_COMPATIBLE}

        -   #### PROVIDER_COMPATIBLE

                public static final RuleAnalysisComputationMode PROVIDER_COMPATIBLE

            ::: block
            same as [`COMPATIBLE`](#COMPATIBLE), but also with the
            ability for rule analysis to depend on providers from action
            graph
            :::
    :::

    ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#DEFAULT}

        -   #### DEFAULT

                public static final RuleAnalysisComputationMode DEFAULT
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#values()}

        -   #### values

            ``` methodSignature
            public static RuleAnalysisComputationMode[] values()
            ```

            ::: block
            Returns an array containing the constants of this enum type,
            in the order they are declared. This method may be used to
            iterate over the constants as follows:
                for (RuleAnalysisComputationMode c : RuleAnalysisComputationMode.values())
                    System.out.println(c);
            :::

            [Returns:]{.returnLabel}
            :   an array containing the constants of this enum type, in
                the order they are declared

        []{#valueOf(java.lang.String)}

        -   #### valueOf

            ``` methodSignature
            public static RuleAnalysisComputationMode valueOf​(String name)
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
-   [Field](#field.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Enum Constants](#enum.constant.detail) \| 
-   [Field](#field.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

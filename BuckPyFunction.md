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
[Package]{.packageLabelInType} [com.facebook.buck.parser.function](package-summary.html)
:::

## Class BuckPyFunction {#class-buckpyfunction .title title="Class BuckPyFunction"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.parser.function.BuckPyFunction

::: description
-   

    ------------------------------------------------------------------------

        public class BuckPyFunction
        extends Object

    ::: block
    Used to generate a function for use within buck.py for the rule
    described by a
    [`Description`](../../core/description/Description.html "interface in com.facebook.buck.core.description").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Field                 | Description           |
        +=======================+=======================+=======================+
        | `static String`       | `BUCK_                |                       |
        |                       | PY_FUNCTION_TEMPLATE` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `INTERNAL_            | ::: block             |
        |                       | PROPERTY_NAME_PREFIX` | Properties from the   |
        |                       |                       | JSON produced by      |
        |                       |                       | `buck.py` that start  |
        |                       |                       | with this prefix do   |
        |                       |                       | not correspond to     |
        |                       |                       | build rule arguments  |
        |                       |                       | specified by the      |
        |                       |                       | user.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `TYPE_PROPERTY_NAME`  | ::: block             |
        |                       |                       | The name of the       |
        |                       |                       | property in the JSON  |
        |                       |                       | produced by `buck.py` |
        |                       |                       | that identifies the   |
        |                       |                       | type of the build     |
        |                       |                       | rule being defined.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                               Description
          --------------------------------------------------------- -------------
          `BuckPyFunction​(TypeCoercerFactory typeCoercerFactory)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `String`              | `ad                   | ::: block             |
        |                       | dDefaultAttributes()` | Returns a python      |
        |                       |                       | string containing all |
        |                       |                       | of the default rule   |
        |                       |                       | parameters that       |
        |                       |                       | should be made        |
        |                       |                       | available to user     |
        |                       |                       | defined rules in the  |
        |                       |                       | python build file     |
        |                       |                       | parser                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toPythonFu           | ::: block             |
        |                       | nction​(RuleType type, | Create a Python       |
        |                       |                  Clas | function definition   |
        |                       | s<? extends DataTrans | for given rule type   |
        |                       | ferObject> dtoClass)` | and parameters        |
        |                       |                       | described by DTO      |
        |                       |                       | type.                 |
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
    -   []{#field.detail}

        ### Field Detail

        []{#INTERNAL_PROPERTY_NAME_PREFIX}

        -   #### INTERNAL_PROPERTY_NAME_PREFIX

                public static final String INTERNAL_PROPERTY_NAME_PREFIX

            ::: block
            Properties from the JSON produced by `buck.py` that start
            with this prefix do not correspond to build rule arguments
            specified by the user. Instead, they contain internal-only
            metadata, so they should not be printed when the build rule
            is reproduced.
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.parser.function.BuckPyFunction.INTERNAL_PROPERTY_NAME_PREFIX)

        []{#TYPE_PROPERTY_NAME}

        -   #### TYPE_PROPERTY_NAME

                public static final String TYPE_PROPERTY_NAME

            ::: block
            The name of the property in the JSON produced by `buck.py`
            that identifies the type of the build rule being defined.
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.parser.function.BuckPyFunction.TYPE_PROPERTY_NAME)

        []{#BUCK_PY_FUNCTION_TEMPLATE}

        -   #### BUCK_PY_FUNCTION_TEMPLATE

                public static final String BUCK_PY_FUNCTION_TEMPLATE

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.parser.function.BuckPyFunction.BUCK_PY_FUNCTION_TEMPLATE)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.rules.coercer.TypeCoercerFactory)}

        -   #### BuckPyFunction

                public BuckPyFunction​(TypeCoercerFactory typeCoercerFactory)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#toPythonFunction(com.facebook.buck.core.model.RuleType,java.lang.Class)}

        -   #### toPythonFunction

            ``` methodSignature
            public String toPythonFunction​(RuleType type,
                                           Class<? extends DataTransferObject> dtoClass)
            ```

            ::: block
            Create a Python function definition for given rule type and
            parameters described by DTO type.
            :::

        []{#addDefaultAttributes()}

        -   #### addDefaultAttributes

            ``` methodSignature
            public String addDefaultAttributes()
            ```

            ::: block
            Returns a python string containing all of the default rule
            parameters that should be made available to user defined
            rules in the python build file parser
            :::
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

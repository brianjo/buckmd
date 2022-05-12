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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
-   [Field](#annotation.type.field.summary) \| 
-   Required \| 
-   [Optional](#annotation.type.optional.element.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#annotation.type.field.detail) \| 
-   [Element](#annotation.type.element.detail)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.description.arg](package-summary.html)
:::

## Annotation Type Hint {#annotation-type-hint .title title="Annotation Type Hint"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        @Retention(RUNTIME)
        @Target({FIELD,METHOD})
        public @interface Hint

    ::: block
    Represents hints given when deal with the value of a type returned
    by
    [`BaseDescription.getConstructorArgType()`](../BaseDescription.html#getConstructorArgType()).
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#annotation.type.field.summary}

        ### Field Summary

          Modifier and Type   Fields                               Description
          ------------------- ------------------------------------ -------------
          `static boolean`    `DEFAULT_EXEC_CONFIGURATION`          
          `static boolean`    `DEFAULT_IS_CONFIGURABLE`             
          `static boolean`    `DEFAULT_IS_DEP`                      
          `static boolean`    `DEFAULT_IS_INPUT`                    
          `static boolean`    `DEFAULT_IS_TARGET_GRAPH_ONLY_DEP`    
          `static boolean`    `DEFAULT_SPLIT_CONFIGURATION`         

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#annotation.type.optional.element.summary}

        ### Optional Element Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Optional Element      | Description           |
        +=======================+=======================+=======================+
        | `boolean`             | `execConfiguration`   | ::: block             |
        |                       |                       | Indicates that        |
        |                       |                       | execution             |
        |                       |                       | configuration (as     |
        |                       |                       | opposed to target     |
        |                       |                       | configuration) should |
        |                       |                       | be used when          |
        |                       |                       | resolving targets.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isConfigurable`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isDep`               |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isInput`             |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `                     |                       |
        |                       | isTargetGraphOnlyDep` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `splitConfiguration`  | ::: block             |
        |                       |                       | Indicates that target |
        |                       |                       | configuration needs   |
        |                       |                       | to be split.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Optional Elements[ ]{.tabEnd}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#annotation.type.field.detail}

        ### Field Detail

        []{#DEFAULT_IS_DEP}

        -   #### DEFAULT_IS_DEP

                static final boolean DEFAULT_IS_DEP
    :::

    ::: {.section role="region"}
    -   []{#DEFAULT_IS_INPUT}
        -   #### DEFAULT_IS_INPUT

                static final boolean DEFAULT_IS_INPUT
    :::

    ::: {.section role="region"}
    -   []{#DEFAULT_IS_TARGET_GRAPH_ONLY_DEP}
        -   #### DEFAULT_IS_TARGET_GRAPH_ONLY_DEP

                static final boolean DEFAULT_IS_TARGET_GRAPH_ONLY_DEP
    :::

    ::: {.section role="region"}
    -   []{#DEFAULT_IS_CONFIGURABLE}
        -   #### DEFAULT_IS_CONFIGURABLE

                static final boolean DEFAULT_IS_CONFIGURABLE
    :::

    ::: {.section role="region"}
    -   []{#DEFAULT_SPLIT_CONFIGURATION}
        -   #### DEFAULT_SPLIT_CONFIGURATION

                static final boolean DEFAULT_SPLIT_CONFIGURATION
    :::

    ::: {.section role="region"}
    -   []{#DEFAULT_EXEC_CONFIGURATION}
        -   #### DEFAULT_EXEC_CONFIGURATION

                static final boolean DEFAULT_EXEC_CONFIGURATION
    :::

    ::: {.section role="region"}
    -   []{#annotation.type.element.detail}

        ### Element Detail

        []{#isDep()}

        -   #### isDep

                boolean isDep

            [Returns:]{.returnLabel}
            :   Whether to search the field\'s value for dependencies

            ```{=html}
            <!-- -->
            ```

            Default:
            :   true
    :::

    ::: {.section role="region"}
    -   []{#isInput()}
        -   #### isInput

                boolean isInput

            [Returns:]{.returnLabel}
            :   Whether to use the field\'s value as an input

            ```{=html}
            <!-- -->
            ```

            Default:
            :   true
    :::

    ::: {.section role="region"}
    -   []{#isTargetGraphOnlyDep()}
        -   #### isTargetGraphOnlyDep

                boolean isTargetGraphOnlyDep

            [Returns:]{.returnLabel}

            :   Whether to add the field\'s value to the target graph,
                but do not automatically propagate it to the build rule
                (action graph). During action graph construction, build
                rules can still decide to add them to action graph based
                on some condition. Build rules must explicitly handle
                these dependencies if they should be used during build.

                For example, rules that support platform-specific
                dependencies must explicitly include dependencies
                matching target platform into the action graph.

            ```{=html}
            <!-- -->
            ```

            Default:
            :   false
    :::

    ::: {.section role="region"}
    -   []{#isConfigurable()}
        -   #### isConfigurable

                boolean isConfigurable

            [Returns:]{.returnLabel}
            :   Whether an attribute can be configured using `select`.

            ```{=html}
            <!-- -->
            ```

            Default:
            :   true
    :::

    ::: {.section role="region"}
    -   []{#splitConfiguration()}
        -   #### splitConfiguration

                boolean splitConfiguration

            ::: block
            Indicates that target configuration needs to be split.
            The target configuration will be transformed into multiple
            other configurations and every target in this attribute
            (target-based object) will be created for every
            configuration and the resulting list will be stored in this
            attribute.

            Note that this logic only applies when target configuration
            supports transformation into multiple configurations and the
            attribute type supports concatenation.
            :::

            Default:
            :   false
    :::

    ::: {.section role="region"}
    -   []{#execConfiguration()}
        -   #### execConfiguration

                boolean execConfiguration

            ::: block
            Indicates that execution configuration (as opposed to target
            configuration) should be used when resolving targets.
            This is used for example in `cxx_toolchain` rule: toolchain
            itself need to be created with target configuration, but if
            it specifies c compiler as a build target, that target need
            to be built for execution configuration.
            :::

            Default:
            :   false
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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

<div>

-   Summary: 
-   [Field](#annotation.type.field.summary) \| 
-   Required \| 
-   [Optional](#annotation.type.optional.element.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#annotation.type.field.detail) \| 
-   [Element](#annotation.type.element.detail)

</div>

[]{#skip.navbar.bottom}
:::

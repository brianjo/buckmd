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
[Package]{.packageLabelInType} [com.facebook.buck.features.apple.project](package-summary.html)
:::

## Enum ProjectGenerator.FilterFlags {#enum-projectgenerator.filterflags .title title="Enum ProjectGenerator.FilterFlags"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<[ProjectGenerator.FilterFlags](ProjectGenerator.FilterFlags.html "enum in com.facebook.buck.features.apple.project")\>

    -   -   com.facebook.buck.features.apple.project.ProjectGenerator.FilterFlags

::: description
-   

    All Implemented Interfaces:
    :   `Serializable`, `Comparable<ProjectGenerator.FilterFlags>`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [ProjectGenerator](ProjectGenerator.html "class in com.facebook.buck.features.apple.project")

    ------------------------------------------------------------------------

        public static enum ProjectGenerator.FilterFlags
        extends Enum<ProjectGenerator.FilterFlags>

    ::: block
    Filter Flags for subdividing dependencies
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#enum.constant.summary}

        ### Enum Constant Summary

          Enum Constant          Description
          ---------------------- -------------
          `CURRENT_PROJECT`       
          `FRAMEWORK`             
          `LIBRARY`               
          `OTHER_FOCUSED`         
          `OTHER_NON_FOCUSED`     
          `WITH_FORCE_LOAD`       
          `WITHOUT_FORCE_LOAD`    

          : Enum Constants[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Field                 | Description           |
        +=======================+=======================+=======================+
        | `sta                  | `FRAME                | ::: block             |
        | tic EnumSet<ProjectGe | WORK_CURRENT_PROJECT` | Filter framework deps |
        | nerator.FilterFlags>` |                       | \*                    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `FRAMEWORK_FOCUSED`   |                       |
        | tic EnumSet<ProjectGe |                       |                       |
        | nerator.FilterFlags>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `FRAMEWORK_OTHER`     |                       |
        | tic EnumSet<ProjectGe |                       |                       |
        | nerator.FilterFlags>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `LIB                  | ::: block             |
        | tic EnumSet<ProjectGe | RARY_CURRENT_PROJECT` | Filter deps for the   |
        | nerator.FilterFlags>` |                       | current project \*    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `LIBRARY_CURRENT_PRO  |                       |
        | tic EnumSet<ProjectGe | JECT_WITH_FORCE_LOAD` |                       |
        | nerator.FilterFlags>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `L                    |                       |
        | tic EnumSet<ProjectGe | IBRARY_CURRENT_PROJEC |                       |
        | nerator.FilterFlags>` | T_WITHOUT_FORCE_LOAD` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `LIBRARY_FOCUSED`     | ::: block             |
        | tic EnumSet<ProjectGe |                       | Filter deps for       |
        | nerator.FilterFlags>` |                       | within the workspace  |
        |                       |                       | and built by Xcode    |
        |                       |                       | but not in the        |
        |                       |                       | current project \*    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `LIBRARY_FOC          |                       |
        | tic EnumSet<ProjectGe | USED_WITH_FORCE_LOAD` |                       |
        | nerator.FilterFlags>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `LIBRARY_FOCUSE       |                       |
        | tic EnumSet<ProjectGe | D_WITHOUT_FORCE_LOAD` |                       |
        | nerator.FilterFlags>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `LIBRARY_OTHER`       | ::: block             |
        | tic EnumSet<ProjectGe |                       | Filter deps not       |
        | nerator.FilterFlags>` |                       | included within the   |
        |                       |                       | workspace \*          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `LIBRARY_O            |                       |
        | tic EnumSet<ProjectGe | THER_WITH_FORCE_LOAD` |                       |
        | nerator.FilterFlags>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `LIBRARY_OTHE         |                       |
        | tic EnumSet<ProjectGe | R_WITHOUT_FORCE_LOAD` |                       |
        | nerator.FilterFlags>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+

        : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static ProjectG      | `                     | ::: block             |
        | enerator.FilterFlags` | valueOf​(String name)` | Returns the enum      |
        |                       |                       | constant of this type |
        |                       |                       | with the specified    |
        |                       |                       | name.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static ProjectGen    | `values()`            | ::: block             |
        | erator.FilterFlags[]` |                       | Returns an array      |
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

        []{#CURRENT_PROJECT}

        -   #### CURRENT_PROJECT

                public static final ProjectGenerator.FilterFlags CURRENT_PROJECT

        []{#OTHER_FOCUSED}

        -   #### OTHER_FOCUSED

                public static final ProjectGenerator.FilterFlags OTHER_FOCUSED

        []{#OTHER_NON_FOCUSED}

        -   #### OTHER_NON_FOCUSED

                public static final ProjectGenerator.FilterFlags OTHER_NON_FOCUSED

        []{#FRAMEWORK}

        -   #### FRAMEWORK

                public static final ProjectGenerator.FilterFlags FRAMEWORK

        []{#LIBRARY}

        -   #### LIBRARY

                public static final ProjectGenerator.FilterFlags LIBRARY

        []{#WITH_FORCE_LOAD}

        -   #### WITH_FORCE_LOAD

                public static final ProjectGenerator.FilterFlags WITH_FORCE_LOAD

        []{#WITHOUT_FORCE_LOAD}

        -   #### WITHOUT_FORCE_LOAD

                public static final ProjectGenerator.FilterFlags WITHOUT_FORCE_LOAD
    :::

    ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#LIBRARY_CURRENT_PROJECT}

        -   #### LIBRARY_CURRENT_PROJECT

                public static final EnumSet<ProjectGenerator.FilterFlags> LIBRARY_CURRENT_PROJECT

            ::: block
            Filter deps for the current project \*
            :::

        []{#LIBRARY_CURRENT_PROJECT_WITH_FORCE_LOAD}

        -   #### LIBRARY_CURRENT_PROJECT_WITH_FORCE_LOAD

                public static final EnumSet<ProjectGenerator.FilterFlags> LIBRARY_CURRENT_PROJECT_WITH_FORCE_LOAD

        []{#LIBRARY_CURRENT_PROJECT_WITHOUT_FORCE_LOAD}

        -   #### LIBRARY_CURRENT_PROJECT_WITHOUT_FORCE_LOAD

                public static final EnumSet<ProjectGenerator.FilterFlags> LIBRARY_CURRENT_PROJECT_WITHOUT_FORCE_LOAD

        []{#LIBRARY_FOCUSED}

        -   #### LIBRARY_FOCUSED

                public static final EnumSet<ProjectGenerator.FilterFlags> LIBRARY_FOCUSED

            ::: block
            Filter deps for within the workspace and built by Xcode but
            not in the current project \*
            :::

        []{#LIBRARY_FOCUSED_WITH_FORCE_LOAD}

        -   #### LIBRARY_FOCUSED_WITH_FORCE_LOAD

                public static final EnumSet<ProjectGenerator.FilterFlags> LIBRARY_FOCUSED_WITH_FORCE_LOAD

        []{#LIBRARY_FOCUSED_WITHOUT_FORCE_LOAD}

        -   #### LIBRARY_FOCUSED_WITHOUT_FORCE_LOAD

                public static final EnumSet<ProjectGenerator.FilterFlags> LIBRARY_FOCUSED_WITHOUT_FORCE_LOAD

        []{#LIBRARY_OTHER}

        -   #### LIBRARY_OTHER

                public static final EnumSet<ProjectGenerator.FilterFlags> LIBRARY_OTHER

            ::: block
            Filter deps not included within the workspace \*
            :::

        []{#LIBRARY_OTHER_WITH_FORCE_LOAD}

        -   #### LIBRARY_OTHER_WITH_FORCE_LOAD

                public static final EnumSet<ProjectGenerator.FilterFlags> LIBRARY_OTHER_WITH_FORCE_LOAD

        []{#LIBRARY_OTHER_WITHOUT_FORCE_LOAD}

        -   #### LIBRARY_OTHER_WITHOUT_FORCE_LOAD

                public static final EnumSet<ProjectGenerator.FilterFlags> LIBRARY_OTHER_WITHOUT_FORCE_LOAD

        []{#FRAMEWORK_CURRENT_PROJECT}

        -   #### FRAMEWORK_CURRENT_PROJECT

                public static final EnumSet<ProjectGenerator.FilterFlags> FRAMEWORK_CURRENT_PROJECT

            ::: block
            Filter framework deps \*
            :::

        []{#FRAMEWORK_FOCUSED}

        -   #### FRAMEWORK_FOCUSED

                public static final EnumSet<ProjectGenerator.FilterFlags> FRAMEWORK_FOCUSED

        []{#FRAMEWORK_OTHER}

        -   #### FRAMEWORK_OTHER

                public static final EnumSet<ProjectGenerator.FilterFlags> FRAMEWORK_OTHER
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#values()}

        -   #### values

            ``` methodSignature
            public static ProjectGenerator.FilterFlags[] values()
            ```

            ::: block
            Returns an array containing the constants of this enum type,
            in the order they are declared. This method may be used to
            iterate over the constants as follows:
                for (ProjectGenerator.FilterFlags c : ProjectGenerator.FilterFlags.values())
                    System.out.println(c);
            :::

            [Returns:]{.returnLabel}
            :   an array containing the constants of this enum type, in
                the order they are declared

        []{#valueOf(java.lang.String)}

        -   #### valueOf

            ``` methodSignature
            public static ProjectGenerator.FilterFlags valueOf​(String name)
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

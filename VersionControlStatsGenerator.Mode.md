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
[Package]{.packageLabelInType} [com.facebook.buck.util.versioncontrol](package-summary.html)
:::

## Enum VersionControlStatsGenerator.Mode {#enum-versioncontrolstatsgenerator.mode .title title="Enum VersionControlStatsGenerator.Mode"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<[VersionControlStatsGenerator.Mode](VersionControlStatsGenerator.Mode.html "enum in com.facebook.buck.util.versioncontrol")\>

    -   -   com.facebook.buck.util.versioncontrol.VersionControlStatsGenerator.Mode

::: description
-   

    All Implemented Interfaces:
    :   `Serializable`, `Comparable<VersionControlStatsGenerator.Mode>`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [VersionControlStatsGenerator](VersionControlStatsGenerator.html "class in com.facebook.buck.util.versioncontrol")

    ------------------------------------------------------------------------

        public static enum VersionControlStatsGenerator.Mode
        extends Enum<VersionControlStatsGenerator.Mode>

    ::: block
    Modes the generator can get stats in, in order from least
    comprehensive to most comprehensive. Each mode should include all
    the information present in the previous one.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#enum.constant.summary}

        ### Enum Constant Summary

        +-----------------------------------+-----------------------------------+
        | Enum Constant                     | Description                       |
        +===================================+===================================+
        | `FAST`                            | ::: block                         |
        |                                   | Generate a set of stats that is   |
        |                                   | fast to generate but incomplete   |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `FULL`                            | ::: block                         |
        |                                   | Generate the full set of stats    |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `PREGENERATED`                    | ::: block                         |
        |                                   | Do not generate new information,  |
        |                                   | but return whatever is already    |
        |                                   | generated                         |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `SLOW`                            | ::: block                         |
        |                                   | Generate a set of stats that is   |
        |                                   | slow to generate but incomplete   |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+

        : Enum Constants[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                                 Description
          ------------------- ------------------------------------- -------------
          `boolean`           `hasDiff`                              
          `boolean`           `hasPathsChangedInWorkingDirectory`    
          `boolean`           `shouldGenerate`                       

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static VersionContro | `                     | ::: block             |
        | lStatsGenerator.Mode` | valueOf​(String name)` | Returns the enum      |
        |                       |                       | constant of this type |
        |                       |                       | with the specified    |
        |                       |                       | name.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `s                    | `values()`            | ::: block             |
        | tatic VersionControlS |                       | Returns an array      |
        | tatsGenerator.Mode[]` |                       | containing the        |
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

        []{#PREGENERATED}

        -   #### PREGENERATED

                public static final VersionControlStatsGenerator.Mode PREGENERATED

            ::: block
            Do not generate new information, but return whatever is
            already generated
            :::

        []{#FAST}

        -   #### FAST

                public static final VersionControlStatsGenerator.Mode FAST

            ::: block
            Generate a set of stats that is fast to generate but
            incomplete
            :::

        []{#SLOW}

        -   #### SLOW

                public static final VersionControlStatsGenerator.Mode SLOW

            ::: block
            Generate a set of stats that is slow to generate but
            incomplete
            :::

        []{#FULL}

        -   #### FULL

                public static final VersionControlStatsGenerator.Mode FULL

            ::: block
            Generate the full set of stats
            :::
    :::

    ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#shouldGenerate}

        -   #### shouldGenerate

                public final boolean shouldGenerate

        []{#hasPathsChangedInWorkingDirectory}

        -   #### hasPathsChangedInWorkingDirectory

                public final boolean hasPathsChangedInWorkingDirectory

        []{#hasDiff}

        -   #### hasDiff

                public final boolean hasDiff
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#values()}

        -   #### values

            ``` methodSignature
            public static VersionControlStatsGenerator.Mode[] values()
            ```

            ::: block
            Returns an array containing the constants of this enum type,
            in the order they are declared. This method may be used to
            iterate over the constants as follows:
                for (VersionControlStatsGenerator.Mode c : VersionControlStatsGenerator.Mode.values())
                    System.out.println(c);
            :::

            [Returns:]{.returnLabel}
            :   an array containing the constants of this enum type, in
                the order they are declared

        []{#valueOf(java.lang.String)}

        -   #### valueOf

            ``` methodSignature
            public static VersionControlStatsGenerator.Mode valueOf​(String name)
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

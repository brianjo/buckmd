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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java.abi](package-summary.html)
:::

## Enum AbiGenerationMode {#enum-abigenerationmode .title title="Enum AbiGenerationMode"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<[AbiGenerationMode](AbiGenerationMode.html "enum in com.facebook.buck.jvm.java.abi")\>

    -   -   com.facebook.buck.jvm.java.abi.AbiGenerationMode

::: description
-   

    All Implemented Interfaces:
    :   `Serializable`, `Comparable<AbiGenerationMode>`

    ------------------------------------------------------------------------

        public enum AbiGenerationMode
        extends Enum<AbiGenerationMode>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#enum.constant.summary}

        ### Enum Constant Summary

        +-----------------------------------+-----------------------------------+
        | Enum Constant                     | Description                       |
        +===================================+===================================+
        | `CLASS`                           | ::: block                         |
        |                                   | Generate ABIs by stripping .class |
        |                                   | files                             |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `MIGRATING_TO_SOURCE_ONLY`        | ::: block                         |
        |                                   | Output warnings for things that   |
        |                                   | aren\'t legal when generating     |
        |                                   | ABIs from source without          |
        |                                   | dependency ABIs                   |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `SOURCE`                          | ::: block                         |
        |                                   | Generate ABIs by parsing .java    |
        |                                   | files with dependency ABIs        |
        |                                   | available                         |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `SOURCE_ONLY`                     | ::: block                         |
        |                                   | Generate ABIs by parsing .java    |
        |                                   | files without dependency ABIs     |
        |                                   | available (has some limitations)  |
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
        | `boolean`             | `checkForSourceOn     |                       |
        |                       | lyAbiCompatibility()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Diagnostic.Kind`     | `getDiag              |                       |
        |                       | nosticKindForSourceOn |                       |
        |                       | lyAbiCompatibility()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isSourceAbi()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `usesDependencies()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `stat                 | `                     | ::: block             |
        | ic AbiGenerationMode` | valueOf​(String name)` | Returns the enum      |
        |                       |                       | constant of this type |
        |                       |                       | with the specified    |
        |                       |                       | name.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `values()`            | ::: block             |
        |  AbiGenerationMode[]` |                       | Returns an array      |
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

        []{#CLASS}

        -   #### CLASS

                public static final AbiGenerationMode CLASS

            ::: block
            Generate ABIs by stripping .class files
            :::

        []{#SOURCE}

        -   #### SOURCE

                public static final AbiGenerationMode SOURCE

            ::: block
            Generate ABIs by parsing .java files with dependency ABIs
            available
            :::

        []{#MIGRATING_TO_SOURCE_ONLY}

        -   #### MIGRATING_TO_SOURCE_ONLY

                public static final AbiGenerationMode MIGRATING_TO_SOURCE_ONLY

            ::: block
            Output warnings for things that aren\'t legal when
            generating ABIs from source without dependency ABIs
            :::

        []{#SOURCE_ONLY}

        -   #### SOURCE_ONLY

                public static final AbiGenerationMode SOURCE_ONLY

            ::: block
            Generate ABIs by parsing .java files without dependency ABIs
            available (has some limitations)
            :::
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#values()}

        -   #### values

            ``` methodSignature
            public static AbiGenerationMode[] values()
            ```

            ::: block
            Returns an array containing the constants of this enum type,
            in the order they are declared. This method may be used to
            iterate over the constants as follows:
                for (AbiGenerationMode c : AbiGenerationMode.values())
                    System.out.println(c);
            :::

            [Returns:]{.returnLabel}
            :   an array containing the constants of this enum type, in
                the order they are declared

        []{#valueOf(java.lang.String)}

        -   #### valueOf

            ``` methodSignature
            public static AbiGenerationMode valueOf​(String name)
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

        []{#checkForSourceOnlyAbiCompatibility()}

        -   #### checkForSourceOnlyAbiCompatibility

            ``` methodSignature
            public boolean checkForSourceOnlyAbiCompatibility()
            ```

        []{#getDiagnosticKindForSourceOnlyAbiCompatibility()}

        -   #### getDiagnosticKindForSourceOnlyAbiCompatibility

            ``` methodSignature
            public Diagnostic.Kind getDiagnosticKindForSourceOnlyAbiCompatibility()
            ```

        []{#isSourceAbi()}

        -   #### isSourceAbi

            ``` methodSignature
            public boolean isSourceAbi()
            ```

        []{#usesDependencies()}

        -   #### usesDependencies

            ``` methodSignature
            public boolean usesDependencies()
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

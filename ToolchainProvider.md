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
-   Field \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.core.toolchain](package-summary.html)
:::

## Interface ToolchainProvider {#interface-toolchainprovider .title title="Interface ToolchainProvider"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `BaseToolchainProvider`, `DefaultToolchainProvider`

    ------------------------------------------------------------------------

        public interface ToolchainProvider

    ::: block
    An interface that give access to specific toolchains by toolchain
    name.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Toolchain`           | `getByNa              |                       |
        |                       | me​(String toolchainNa |                       |
        |                       | me,          TargetCo |                       |
        |                       | nfiguration toolchain |                       |
        |                       | TargetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `<T                   | `getByName​(String too |                       |
        |  extends Toolchain>T` | lchainName,           |                       |
        |                       | TargetConfiguration t |                       |
        |                       | oolchainTargetConfigu |                       |
        |                       | ration,          Clas |                       |
        |                       | s<T> toolchainClass)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `<T extends T         | `getBy                |                       |
        | oolchain>Optional<T>` | NameIfPresent​(String  |                       |
        |                       | toolchainName,        |                       |
        |                       |             TargetCon |                       |
        |                       | figuration toolchainT |                       |
        |                       | argetConfiguration,   |                       |
        |                       |                  Clas |                       |
        |                       | s<T> toolchainClass)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getToolchainIns      |                       |
        | Optional<ToolchainIns | tantiationException​(S |                       |
        | tantiationException>` | tring toolchainName,  |                       |
        |                       |                       |                       |
        |                       |              TargetCo |                       |
        |                       | nfiguration toolchain |                       |
        |                       | TargetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `<T extends T         | `getTool              | ::: block             |
        | oolchainWithCapabilit | chainsWithCapability​( | Provides access to    |
        | y>Collection<String>` | Class<T> capability)` | all known toolchains  |
        |                       |                       | that support the      |
        |                       |                       | provided capability.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isTo                 |                       |
        |                       | olchainCreated​(String |                       |
        |                       |  toolchainName,       |                       |
        |                       |              TargetCo |                       |
        |                       | nfiguration toolchain |                       |
        |                       | TargetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `is                   |                       |
        |                       | ToolchainFailed​(Strin |                       |
        |                       | g toolchainName,      |                       |
        |                       |              TargetCo |                       |
        |                       | nfiguration toolchain |                       |
        |                       | TargetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isTo                 |                       |
        |                       | olchainPresent​(String |                       |
        |                       |  toolchainName,       |                       |
        |                       |              TargetCo |                       |
        |                       | nfiguration toolchain |                       |
        |                       | TargetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getByName(java.lang.String,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getByName

            ``` methodSignature
            Toolchain getByName​(String toolchainName,
                                TargetConfiguration toolchainTargetConfiguration)
            ```

            [Throws:]{.throwsLabel}
            :   `ToolchainInstantiationException` - when a toolchain
                cannot be created

        []{#getByName(java.lang.String,com.facebook.buck.core.model.TargetConfiguration,java.lang.Class)}

        -   #### getByName

            ``` methodSignature
            <T extends Toolchain> T getByName​(String toolchainName,
                                              TargetConfiguration toolchainTargetConfiguration,
                                              Class<T> toolchainClass)
            ```

            [Throws:]{.throwsLabel}
            :   `ToolchainInstantiationException` - when a toolchain
                cannot be created

        []{#getByNameIfPresent(java.lang.String,com.facebook.buck.core.model.TargetConfiguration,java.lang.Class)}

        -   #### getByNameIfPresent

            ``` methodSignature
            <T extends Toolchain> Optional<T> getByNameIfPresent​(String toolchainName,
                                                                 TargetConfiguration toolchainTargetConfiguration,
                                                                 Class<T> toolchainClass)
            ```

        []{#isToolchainPresent(java.lang.String,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### isToolchainPresent

            ``` methodSignature
            boolean isToolchainPresent​(String toolchainName,
                                       TargetConfiguration toolchainTargetConfiguration)
            ```

            [Returns:]{.returnLabel}
            :   `true` if toolchain exists (triggering instantiation if
                needed)

        []{#isToolchainCreated(java.lang.String,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### isToolchainCreated

            ``` methodSignature
            boolean isToolchainCreated​(String toolchainName,
                                       TargetConfiguration toolchainTargetConfiguration)
            ```

            [Returns:]{.returnLabel}
            :   `true` if toolchain has already been created (without
                triggering instantiation)

        []{#isToolchainFailed(java.lang.String,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### isToolchainFailed

            ``` methodSignature
            boolean isToolchainFailed​(String toolchainName,
                                      TargetConfiguration toolchainTargetConfiguration)
            ```

            [Returns:]{.returnLabel}
            :   `true` if toolchain failed to instantiate (without
                triggering instantiation)

        []{#getToolchainsWithCapability(java.lang.Class)}

        -   #### getToolchainsWithCapability

            ``` methodSignature
            <T extends ToolchainWithCapability> Collection<String> getToolchainsWithCapability​(Class<T> capability)
            ```

            ::: block
            Provides access to all known toolchains that support the
            provided capability.
            The toolchains are not created during the execution of this
            method.
            :::

            [Returns:]{.returnLabel}
            :   a collection of toolchain names that support the
                provided capability.

        []{#getToolchainInstantiationException(java.lang.String,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getToolchainInstantiationException

            ``` methodSignature
            Optional<ToolchainInstantiationException> getToolchainInstantiationException​(String toolchainName,
                                                                                         TargetConfiguration toolchainTargetConfiguration)
            ```

            [Returns:]{.returnLabel}
            :   the exception that was thrown during toolchain
                instantiation
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
-   Field \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

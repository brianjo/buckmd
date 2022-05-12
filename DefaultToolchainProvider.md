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
-   Field \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.core.toolchain.impl](package-summary.html)
:::

## Class DefaultToolchainProvider {#class-defaulttoolchainprovider .title title="Class DefaultToolchainProvider"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.toolchain.BaseToolchainProvider](../BaseToolchainProvider.html "class in com.facebook.buck.core.toolchain")

    -   -   com.facebook.buck.core.toolchain.impl.DefaultToolchainProvider

::: description
-   

    All Implemented Interfaces:
    :   `ToolchainProvider`

    ------------------------------------------------------------------------

        public class DefaultToolchainProvider
        extends BaseToolchainProvider
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                      Description
          ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `DefaultToolchainProvider​(org.pf4j.PluginManager pluginManager,                         com.google.common.collect.ImmutableMap<String,​String> environment,                         BuckConfig buckConfig,                         ProjectFilesystem projectFilesystem,                         ProcessExecutor processExecutor,                         ExecutableFinder executableFinder,                         RuleKeyConfiguration ruleKeyConfiguration)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
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
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.toolchain.BaseToolchainProvider}

            ### Methods inherited from class com.facebook.buck.core.toolchain.[BaseToolchainProvider](../BaseToolchainProvider.html "class in com.facebook.buck.core.toolchain")

            `getByName, getByNameIfPresent`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(org.pf4j.PluginManager,com.google.common.collect.ImmutableMap,com.facebook.buck.core.config.BuckConfig,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.util.ProcessExecutor,com.facebook.buck.io.ExecutableFinder,com.facebook.buck.rules.keys.config.RuleKeyConfiguration)}

        -   #### DefaultToolchainProvider

                public DefaultToolchainProvider​(org.pf4j.PluginManager pluginManager,
                                                com.google.common.collect.ImmutableMap<String,​String> environment,
                                                BuckConfig buckConfig,
                                                ProjectFilesystem projectFilesystem,
                                                ProcessExecutor processExecutor,
                                                ExecutableFinder executableFinder,
                                                RuleKeyConfiguration ruleKeyConfiguration)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getByName(java.lang.String,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getByName

            ``` methodSignature
            public Toolchain getByName​(String toolchainName,
                                       TargetConfiguration toolchainTargetConfiguration)
            ```

        []{#isToolchainPresent(java.lang.String,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### isToolchainPresent

            ``` methodSignature
            public boolean isToolchainPresent​(String toolchainName,
                                              TargetConfiguration toolchainTargetConfiguration)
            ```

            [Returns:]{.returnLabel}
            :   `true` if toolchain exists (triggering instantiation if
                needed)

        []{#isToolchainCreated(java.lang.String,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### isToolchainCreated

            ``` methodSignature
            public boolean isToolchainCreated​(String toolchainName,
                                              TargetConfiguration toolchainTargetConfiguration)
            ```

            [Returns:]{.returnLabel}
            :   `true` if toolchain has already been created (without
                triggering instantiation)

        []{#isToolchainFailed(java.lang.String,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### isToolchainFailed

            ``` methodSignature
            public boolean isToolchainFailed​(String toolchainName,
                                             TargetConfiguration toolchainTargetConfiguration)
            ```

            [Returns:]{.returnLabel}
            :   `true` if toolchain failed to instantiate (without
                triggering instantiation)

        []{#getToolchainsWithCapability(java.lang.Class)}

        -   #### getToolchainsWithCapability

            ``` methodSignature
            public <T extends ToolchainWithCapability> Collection<String> getToolchainsWithCapability​(Class<T> capability)
            ```

            ::: block
            [Description copied from
            interface: `ToolchainProvider`]{.descfrmTypeLabel}
            :::

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
            public Optional<ToolchainInstantiationException> getToolchainInstantiationException​(String toolchainName,
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
-   Field \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

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
[Package]{.packageLabelInType} [com.facebook.buck.features.python.toolchain.impl](package-summary.html)
:::

## Class PythonPlatformsProviderFactory {#class-pythonplatformsproviderfactory .title title="Class PythonPlatformsProviderFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.python.toolchain.impl.PythonPlatformsProviderFactory

::: description
-   

    All Implemented Interfaces:
    :   `ToolchainFactory<PythonPlatformsProvider>`

    ------------------------------------------------------------------------

        public class PythonPlatformsProviderFactory
        extends Object
        implements ToolchainFactory<PythonPlatformsProvider>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                          Description
          ------------------------------------ -------------
          `PythonPlatformsProviderFactory()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Optional<Pyth        | `createToolchain​(Tool |                       |
        | onPlatformsProvider>` | chainProvider toolcha |                       |
        |                       | inProvider,           |                       |
        |                       |       ToolchainCreati |                       |
        |                       | onContext context,    |                       |
        |                       |              TargetCo |                       |
        |                       | nfiguration toolchain |                       |
        |                       | TargetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `prot                 | `getDe                |                       |
        | ected PythonPlatform` | faultPythonPlatform​(T |                       |
        |                       | oolchainProvider tool |                       |
        |                       | chainProvider,        |                       |
        |                       |                   Pyt |                       |
        |                       | honBuckConfig pythonB |                       |
        |                       | uckConfig,            |                       |
        |                       |               Process |                       |
        |                       | Executor executor,    |                       |
        |                       |                       |                       |
        |                       |  TargetConfiguration  |                       |
        |                       | targetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.com       | `getPython            | ::: block             |
        | mon.collect.Immutable | Platforms​(ToolchainPr | Constructs set of     |
        | List<PythonPlatform>` | ovider toolchainProvi | Python platform       |
        |                       | der,                  | flavors given in a    |
        |                       |   PythonBuckConfig py | .buckconfig file, as  |
        |                       | thonBuckConfig,       | is specified by       |
        |                       |              ProcessE | section names of the  |
        |                       | xecutor processExecut | form python#{flavor   |
        |                       | or,                   | name}.                |
        |                       |  TargetConfiguration  | :::                   |
        |                       | targetConfiguration)` |                       |
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### PythonPlatformsProviderFactory

                public PythonPlatformsProviderFactory()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#createToolchain(com.facebook.buck.core.toolchain.ToolchainProvider,com.facebook.buck.core.toolchain.ToolchainCreationContext,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### createToolchain

            ``` methodSignature
            public Optional<PythonPlatformsProvider> createToolchain​(ToolchainProvider toolchainProvider,
                                                                     ToolchainCreationContext context,
                                                                     TargetConfiguration toolchainTargetConfiguration)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `createToolchain` in
                interface `ToolchainFactory<PythonPlatformsProvider>`

        []{#getPythonPlatforms(com.facebook.buck.core.toolchain.ToolchainProvider,com.facebook.buck.features.python.PythonBuckConfig,com.facebook.buck.util.ProcessExecutor,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getPythonPlatforms

            ``` methodSignature
            public com.google.common.collect.ImmutableList<PythonPlatform> getPythonPlatforms​(ToolchainProvider toolchainProvider,
                                                                                              PythonBuckConfig pythonBuckConfig,
                                                                                              ProcessExecutor processExecutor,
                                                                                              TargetConfiguration targetConfiguration)
            ```

            ::: block
            Constructs set of Python platform flavors given in a
            .buckconfig file, as is specified by section names of the
            form python#{flavor name}.
            :::

        []{#getDefaultPythonPlatform(com.facebook.buck.core.toolchain.ToolchainProvider,com.facebook.buck.features.python.PythonBuckConfig,com.facebook.buck.util.ProcessExecutor,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getDefaultPythonPlatform

            ``` methodSignature
            protected PythonPlatform getDefaultPythonPlatform​(ToolchainProvider toolchainProvider,
                                                              PythonBuckConfig pythonBuckConfig,
                                                              ProcessExecutor executor,
                                                              TargetConfiguration targetConfiguration)
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

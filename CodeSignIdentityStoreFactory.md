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
[Package]{.packageLabelInType} [com.facebook.buck.apple.toolchain.impl](package-summary.html)
:::

## Class CodeSignIdentityStoreFactory {#class-codesignidentitystorefactory .title title="Class CodeSignIdentityStoreFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.toolchain.impl.CodeSignIdentityStoreFactory

::: description
-   

    All Implemented Interfaces:
    :   `ToolchainFactory<CodeSignIdentityStore>`

    ------------------------------------------------------------------------

        public class CodeSignIdentityStoreFactory
        extends Object
        implements ToolchainFactory<CodeSignIdentityStore>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                        Description
          ---------------------------------- -------------
          `CodeSignIdentityStoreFactory()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Optional<Co          | `createToolchain​(Tool |                       |
        | deSignIdentityStore>` | chainProvider toolcha |                       |
        |                       | inProvider,           |                       |
        |                       |       ToolchainCreati |                       |
        |                       | onContext context,    |                       |
        |                       |              TargetCo |                       |
        |                       | nfiguration toolchain |                       |
        |                       | TargetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static C             | `fromSy               | ::: block             |
        | odeSignIdentityStore` | stem​(ProcessExecutor  | Construct a store by  |
        |                       | processExecutor,      | asking the system     |
        |                       |       com.google.comm | keychain for all      |
        |                       | on.collect.ImmutableL | stored code sign      |
        |                       | ist<String> command)` | identities.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
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

        -   #### CodeSignIdentityStoreFactory

                public CodeSignIdentityStoreFactory()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#fromSystem(com.facebook.buck.util.ProcessExecutor,com.google.common.collect.ImmutableList)}

        -   #### fromSystem

            ``` methodSignature
            public static CodeSignIdentityStore fromSystem​(ProcessExecutor processExecutor,
                                                           com.google.common.collect.ImmutableList<String> command)
            ```

            ::: block
            Construct a store by asking the system keychain for all
            stored code sign identities.
            The loading process is deferred till first access.
            :::

        []{#createToolchain(com.facebook.buck.core.toolchain.ToolchainProvider,com.facebook.buck.core.toolchain.ToolchainCreationContext,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### createToolchain

            ``` methodSignature
            public Optional<CodeSignIdentityStore> createToolchain​(ToolchainProvider toolchainProvider,
                                                                   ToolchainCreationContext context,
                                                                   TargetConfiguration toolchainTargetConfiguration)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `createToolchain` in
                interface `ToolchainFactory<CodeSignIdentityStore>`
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

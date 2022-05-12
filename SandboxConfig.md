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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.sandbox](package-summary.html)
:::

## Class SandboxConfig {#class-sandboxconfig .title title="Class SandboxConfig"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.sandbox.SandboxConfig

::: description
-   

    All Implemented Interfaces:
    :   `ConfigView<BuckConfig>`

    ------------------------------------------------------------------------

        public abstract class SandboxConfig
        extends Object
        implements ConfigView<BuckConfig>

    ::: block
    Config section responsible for sandbox features.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor         Description
          ------------------- -------------
          `SandboxConfig()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `abstract BuckConfig` | `getDelegate()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isDa                 | ::: block             |
        |                       | rwinSandboxEnabled()` | Whether sandboxing is |
        |                       |                       | enabled on Darwin (OS |
        |                       |                       | X).                   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isGen                | ::: block             |
        |                       | ruleSandboxEnabled()` | Whether \`genrule\`   |
        |                       |                       | should use            |
        |                       |                       | sandboxing.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isSandboxEnabled     | ::: block             |
        |                       | ForCurrentPlatform()` | Whether sandboxing is |
        |                       |                       | enabled on the        |
        |                       |                       | current platform.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `of​(                  |                       |
        | static SandboxConfig` | BuckConfig delegate)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
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

        -   #### SandboxConfig

                public SandboxConfig()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getDelegate()}

        -   #### getDelegate

            ``` methodSignature
            public abstract BuckConfig getDelegate()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDelegate` in interface `ConfigView<BuckConfig>`

        []{#of(com.facebook.buck.core.config.BuckConfig)}

        -   #### of

            ``` methodSignature
            public static SandboxConfig of​(BuckConfig delegate)
            ```

        []{#isGenruleSandboxEnabled()}

        -   #### isGenruleSandboxEnabled

            ``` methodSignature
            @Lazy
            public boolean isGenruleSandboxEnabled()
            ```

            ::: block
            Whether \`genrule\` should use sandboxing.
            \`genrule\` sandboxing can be enabled or disabled for
            particular targets using `  enable_sandbox` parameter.
            :::

        []{#isDarwinSandboxEnabled()}

        -   #### isDarwinSandboxEnabled

            ``` methodSignature
            @Lazy
            public boolean isDarwinSandboxEnabled()
            ```

            ::: block
            Whether sandboxing is enabled on Darwin (OS X).
            :::

        []{#isSandboxEnabledForCurrentPlatform()}

        -   #### isSandboxEnabledForCurrentPlatform

            ``` methodSignature
            @Lazy
            public boolean isSandboxEnabledForCurrentPlatform()
            ```

            ::: block
            Whether sandboxing is enabled on the current platform.
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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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

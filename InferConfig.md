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
[Package]{.packageLabelInType} [com.facebook.buck.infer](package-summary.html)
:::

## Class InferConfig {#class-inferconfig .title title="Class InferConfig"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.infer.InferConfig

::: description
-   

    All Implemented Interfaces:
    :   `ConfigView<BuckConfig>`

    ------------------------------------------------------------------------

        public abstract class InferConfig
        extends Object
        implements ConfigView<BuckConfig>

    ::: block
    Infer specific buck config
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor       Description
          ----------------- -------------
          `InferConfig()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Boolean`             | `executeRemotely()`   |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Op                   | `getBinary()`         |                       |
        | tional<ToolProvider>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getConfigFile        |                       |
        | Optional<SourcePath>` | ​(TargetConfiguration  |                       |
        |                       | targetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract BuckConfig` | `getDelegate()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Op                   | `getDist()`           | ::: block             |
        | tional<ToolProvider>` |                       | Depending on the type |
        |                       |                       | of dist (plain path   |
        |                       |                       | vs target) either     |
        |                       |                       | return a              |
        |                       |                       | [`                    |
        |                       |                       | ConstantToolProvider` |
        |                       |                       | ](../core/toolchain/t |
        |                       |                       | oolprovider/impl/Cons |
        |                       |                       | tantToolProvider.html |
        |                       |                       |  "class in com.facebo |
        |                       |                       | ok.buck.core.toolchai |
        |                       |                       | n.toolprovider.impl") |
        |                       |                       | or                    |
        |                       |                       | [`InferDistFromT      |
        |                       |                       | argetProvider`](Infer |
        |                       |                       | DistFromTargetProvide |
        |                       |                       | r.html "class in com. |
        |                       |                       | facebook.buck.infer") |
        |                       |                       | with properly set up  |
        |                       |                       | parse time deps.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getDistBinary()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getNullsafeArgs()`   |                       |
        | ogle.common.collect.I |                       |                       |
        | mmutableList<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getNullsaf           | ::: block             |
        | Optional<SourcePath>` | eThirdPartySignatures | Directory with third  |
        |                       | ​(TargetConfiguration  | party signatures for  |
        |                       | targetConfiguration)` | nullsafe.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Boolean`             | `getPrettyPrint()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getVersion()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static InferConfig`  | `of​(                  |                       |
        |                       | BuckConfig delegate)` |                       |
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

        -   #### InferConfig

                public InferConfig()
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
            public static InferConfig of​(BuckConfig delegate)
            ```

        []{#getBinary()}

        -   #### getBinary

            ``` methodSignature
            @Lazy
            public Optional<ToolProvider> getBinary()
            ```

        []{#getDist()}

        -   #### getDist

            ``` methodSignature
            @Lazy
            public Optional<ToolProvider> getDist()
            ```

            ::: block
            Depending on the type of dist (plain path vs target) either
            return a
            [`ConstantToolProvider`](../core/toolchain/toolprovider/impl/ConstantToolProvider.html "class in com.facebook.buck.core.toolchain.toolprovider.impl")
            or
            [`InferDistFromTargetProvider`](InferDistFromTargetProvider.html "class in com.facebook.buck.infer")
            with properly set up parse time deps.
            :::

        []{#getDistBinary()}

        -   #### getDistBinary

            ``` methodSignature
            @Lazy
            public String getDistBinary()
            ```

        []{#getVersion()}

        -   #### getVersion

            ``` methodSignature
            @Lazy
            public Optional<String> getVersion()
            ```

        []{#getConfigFile(com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getConfigFile

            ``` methodSignature
            @Lazy
            public Optional<SourcePath> getConfigFile​(TargetConfiguration targetConfiguration)
            ```

        []{#getNullsafeArgs()}

        -   #### getNullsafeArgs

            ``` methodSignature
            @Lazy
            public com.google.common.collect.ImmutableList<String> getNullsafeArgs()
            ```

        []{#getNullsafeThirdPartySignatures(com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getNullsafeThirdPartySignatures

            ``` methodSignature
            @Lazy
            public Optional<SourcePath> getNullsafeThirdPartySignatures​(TargetConfiguration targetConfiguration)
            ```

            ::: block
            Directory with third party signatures for nullsafe.
            :::

        []{#getPrettyPrint()}

        -   #### getPrettyPrint

            ``` methodSignature
            @Lazy
            public Boolean getPrettyPrint()
            ```

        []{#executeRemotely()}

        -   #### executeRemotely

            ``` methodSignature
            @Lazy
            public Boolean executeRemotely()
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

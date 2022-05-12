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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.android.toolchain.ndk](package-summary.html)
:::

## Class NdkCxxPlatformsProvider {#class-ndkcxxplatformsprovider .title title="Class NdkCxxPlatformsProvider"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.toolchain.BaseToolchain](../../../core/toolchain/BaseToolchain.html "class in com.facebook.buck.core.toolchain")

    -   -   com.facebook.buck.android.toolchain.ndk.NdkCxxPlatformsProvider

::: description
-   

    All Implemented Interfaces:
    :   `Toolchain`, `ToolchainWithCapability`, `CxxPlatformsSupplier`

    ------------------------------------------------------------------------

        public abstract class NdkCxxPlatformsProvider
        extends BaseToolchain
        implements CxxPlatformsSupplier

    ::: block
    Provides all
    [`NdkCxxPlatform`](NdkCxxPlatform.html "interface in com.facebook.buck.android.toolchain.ndk")s
    by
    [`TargetCpuType`](TargetCpuType.html "enum in com.facebook.buck.android.toolchain.ndk").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field            Description
          ------------------- ---------------- -------------
          `static String`     `DEFAULT_NAME`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                   Description
          ----------------------------- -------------
          `NdkCxxPlatformsProvider()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                                           Method                                                                        Description
          ------------------------------------------------------------------------------------------- ----------------------------------------------------------------------------- -------------
          `String`                                                                                    `getName()`                                                                    
          `abstract com.google.common.collect.ImmutableMap<TargetCpuType,​UnresolvedNdkCxxPlatform>`   `getNdkCxxPlatforms()`                                                         
          `com.google.common.collect.ImmutableMap<TargetCpuType,​NdkCxxPlatform>`                      `getResolvedNdkCxxPlatforms​(BuildRuleResolver resolver)`                       
          `com.google.common.collect.ImmutableMap<Flavor,​UnresolvedCxxPlatform>`                      `getUnresolvedCxxPlatforms()`                                                  
          `static NdkCxxPlatformsProvider`                                                            `of​(Map<TargetCpuType,​? extends UnresolvedNdkCxxPlatform> ndkCxxPlatforms)`    

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
    -   []{#field.detail}

        ### Field Detail

        []{#DEFAULT_NAME}

        -   #### DEFAULT_NAME

                public static final String DEFAULT_NAME

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.android.toolchain.ndk.NdkCxxPlatformsProvider.DEFAULT_NAME)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### NdkCxxPlatformsProvider

                public NdkCxxPlatformsProvider()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getNdkCxxPlatforms()}

        -   #### getNdkCxxPlatforms

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableMap<TargetCpuType,​UnresolvedNdkCxxPlatform> getNdkCxxPlatforms()
            ```

            [Returns:]{.returnLabel}
            :   all
                [`UnresolvedNdkCxxPlatform`](UnresolvedNdkCxxPlatform.html "interface in com.facebook.buck.android.toolchain.ndk")s
                by
                [`TargetCpuType`](TargetCpuType.html "enum in com.facebook.buck.android.toolchain.ndk").

        []{#getResolvedNdkCxxPlatforms(com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### getResolvedNdkCxxPlatforms

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<TargetCpuType,​NdkCxxPlatform> getResolvedNdkCxxPlatforms​(BuildRuleResolver resolver)
            ```

            [Returns:]{.returnLabel}
            :   all resolved
                [`NdkCxxPlatform`](NdkCxxPlatform.html "interface in com.facebook.buck.android.toolchain.ndk")s
                by
                [`TargetCpuType`](TargetCpuType.html "enum in com.facebook.buck.android.toolchain.ndk").

        []{#getUnresolvedCxxPlatforms()}

        -   #### getUnresolvedCxxPlatforms

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<Flavor,​UnresolvedCxxPlatform> getUnresolvedCxxPlatforms()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getUnresolvedCxxPlatforms` in
                interface `CxxPlatformsSupplier`

            [Returns:]{.returnLabel}
            :   [`CxxPlatform`](../../../cxx/toolchain/CxxPlatform.html "interface in com.facebook.buck.cxx.toolchain")
                of all
                [`NdkCxxPlatform`](NdkCxxPlatform.html "interface in com.facebook.buck.android.toolchain.ndk")s

        []{#getName()}

        -   #### getName

            ``` methodSignature
            public String getName()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getName` in interface `Toolchain`

        []{#of(java.util.Map)}

        -   #### of

            ``` methodSignature
            public static NdkCxxPlatformsProvider of​(Map<TargetCpuType,​? extends UnresolvedNdkCxxPlatform> ndkCxxPlatforms)
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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

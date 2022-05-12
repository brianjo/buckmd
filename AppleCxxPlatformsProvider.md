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
[Package]{.packageLabelInType} [com.facebook.buck.apple.toolchain](package-summary.html)
:::

## Class AppleCxxPlatformsProvider {#class-applecxxplatformsprovider .title title="Class AppleCxxPlatformsProvider"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.toolchain.AppleCxxPlatformsProvider

::: description
-   

    All Implemented Interfaces:
    :   `Toolchain`, `ToolchainWithCapability`, `CxxPlatformsSupplier`

    ------------------------------------------------------------------------

        public abstract class AppleCxxPlatformsProvider
        extends Object
        implements CxxPlatformsSupplier
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

          Constructor                     Description
          ------------------------------- -------------
          `AppleCxxPlatformsProvider()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                        Method                                                             Description
          ------------------------------------------------------------------------ ------------------------------------------------------------------ -------------
          `String`                                                                 `getName()`                                                         
          `abstract FlavorDomain<UnresolvedAppleCxxPlatform>`                      `getUnresolvedAppleCxxPlatforms()`                                  
          `com.google.common.collect.ImmutableMap<Flavor,​UnresolvedCxxPlatform>`   `getUnresolvedCxxPlatforms()`                                       
          `static AppleCxxPlatformsProvider`                                       `of​(FlavorDomain<UnresolvedAppleCxxPlatform> appleCxxPlatforms)`    

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
                Values](../../../../../constant-values.html#com.facebook.buck.apple.toolchain.AppleCxxPlatformsProvider.DEFAULT_NAME)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### AppleCxxPlatformsProvider

                public AppleCxxPlatformsProvider()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getUnresolvedAppleCxxPlatforms()}

        -   #### getUnresolvedAppleCxxPlatforms

            ``` methodSignature
            public abstract FlavorDomain<UnresolvedAppleCxxPlatform> getUnresolvedAppleCxxPlatforms()
            ```

        []{#getUnresolvedCxxPlatforms()}

        -   #### getUnresolvedCxxPlatforms

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<Flavor,​UnresolvedCxxPlatform> getUnresolvedCxxPlatforms()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getUnresolvedCxxPlatforms` in
                interface `CxxPlatformsSupplier`

            [Returns:]{.returnLabel}
            :   [`UnresolvedCxxPlatform`](../../cxx/toolchain/UnresolvedCxxPlatform.html "interface in com.facebook.buck.cxx.toolchain")
                of all
                [`UnresolvedAppleCxxPlatform`](UnresolvedAppleCxxPlatform.html "interface in com.facebook.buck.apple.toolchain")s

        []{#getName()}

        -   #### getName

            ``` methodSignature
            public String getName()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getName` in interface `Toolchain`

        []{#of(com.facebook.buck.core.model.FlavorDomain)}

        -   #### of

            ``` methodSignature
            public static AppleCxxPlatformsProvider of​(FlavorDomain<UnresolvedAppleCxxPlatform> appleCxxPlatforms)
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

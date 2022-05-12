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

## Class ProvisioningProfileStore {#class-provisioningprofilestore .title title="Class ProvisioningProfileStore"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.toolchain.ProvisioningProfileStore

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`, `Toolchain`

    ------------------------------------------------------------------------

        public abstract class ProvisioningProfileStore
        extends Object
        implements AddsToRuleKey, Toolchain

    ::: block
    A collection of provisioning profiles.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                                                                         Field                     Description
          ----------------------------------------------------------------------------------------- ------------------------- -------------
          `static String`                                                                           `DEFAULT_NAME`             
          `static Optional<com.google.common.collect.ImmutableMap<String,​com.dd.plist.NSObject>>`   `MATCH_ANY_ENTITLEMENT`    
          `static Optional<com.google.common.collect.ImmutableList<CodeSignIdentity>>`              `MATCH_ANY_IDENTITY`       

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                    Description
          ------------------------------ -------------
          `ProvisioningProfileStore()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                                                              Method                                                                                                                                                                                                                                                                                                                                                                  Description
          -------------------------------------------------------------------------------------------------------------- ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `static ProvisioningProfileStore`                                                                              `empty()`                                                                                                                                                                                                                                                                                                                                                                
          `Optional<ProvisioningProfileMetadata>`                                                                        `getBestProvisioningProfile​(String bundleID,                           ApplePlatform platform,                           Optional<com.google.common.collect.ImmutableMap<String,​com.dd.plist.NSObject>> entitlements,                           Optional<? extends Iterable<CodeSignIdentity>> identities,                           StringBuffer diagnosticsBuffer)`    
          `String`                                                                                                       `getName()`                                                                                                                                                                                                                                                                                                                                                              
          `Optional<ProvisioningProfileMetadata>`                                                                        `getProvisioningProfileByUUID​(String provisioningProfileUUID)`                                                                                                                                                                                                                                                                                                           
          `com.google.common.collect.ImmutableList<ProvisioningProfileMetadata>`                                         `getProvisioningProfiles()`                                                                                                                                                                                                                                                                                                                                              
          `abstract java.util.function.Supplier<com.google.common.collect.ImmutableList<ProvisioningProfileMetadata>>`   `getProvisioningProfilesSupplier()`                                                                                                                                                                                                                                                                                                                                      
          `static ProvisioningProfileStore`                                                                              `of​(java.util.function.Supplier<com.google.common.collect.ImmutableList<ProvisioningProfileMetadata>> provisioningProfilesSupplier)`                                                                                                                                                                                                                                     

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

        []{#MATCH_ANY_ENTITLEMENT}

        -   #### MATCH_ANY_ENTITLEMENT

                public static final Optional<com.google.common.collect.ImmutableMap<String,​com.dd.plist.NSObject>> MATCH_ANY_ENTITLEMENT

        []{#MATCH_ANY_IDENTITY}

        -   #### MATCH_ANY_IDENTITY

                public static final Optional<com.google.common.collect.ImmutableList<CodeSignIdentity>> MATCH_ANY_IDENTITY

        []{#DEFAULT_NAME}

        -   #### DEFAULT_NAME

                public static final String DEFAULT_NAME

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.apple.toolchain.ProvisioningProfileStore.DEFAULT_NAME)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### ProvisioningProfileStore

                public ProvisioningProfileStore()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getProvisioningProfilesSupplier()}

        -   #### getProvisioningProfilesSupplier

            ``` methodSignature
            public abstract java.util.function.Supplier<com.google.common.collect.ImmutableList<ProvisioningProfileMetadata>> getProvisioningProfilesSupplier()
            ```

        []{#getProvisioningProfiles()}

        -   #### getProvisioningProfiles

            ``` methodSignature
            public com.google.common.collect.ImmutableList<ProvisioningProfileMetadata> getProvisioningProfiles()
            ```

        []{#getProvisioningProfileByUUID(java.lang.String)}

        -   #### getProvisioningProfileByUUID

            ``` methodSignature
            public Optional<ProvisioningProfileMetadata> getProvisioningProfileByUUID​(String provisioningProfileUUID)
            ```

        []{#getBestProvisioningProfile(java.lang.String,com.facebook.buck.apple.toolchain.ApplePlatform,java.util.Optional,java.util.Optional,java.lang.StringBuffer)}

        -   #### getBestProvisioningProfile

            ``` methodSignature
            public Optional<ProvisioningProfileMetadata> getBestProvisioningProfile​(String bundleID,
                                                                                    ApplePlatform platform,
                                                                                    Optional<com.google.common.collect.ImmutableMap<String,​com.dd.plist.NSObject>> entitlements,
                                                                                    Optional<? extends Iterable<CodeSignIdentity>> identities,
                                                                                    StringBuffer diagnosticsBuffer)
            ```

        []{#empty()}

        -   #### empty

            ``` methodSignature
            public static ProvisioningProfileStore empty()
            ```

        []{#getName()}

        -   #### getName

            ``` methodSignature
            public String getName()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getName` in interface `Toolchain`

        []{#of(java.util.function.Supplier)}

        -   #### of

            ``` methodSignature
            public static ProvisioningProfileStore of​(java.util.function.Supplier<com.google.common.collect.ImmutableList<ProvisioningProfileMetadata>> provisioningProfilesSupplier)
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

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
-   [Nested](#nested.class.summary) \| 
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

## Class ApplePlatform {#class-appleplatform .title title="Class ApplePlatform"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.toolchain.ApplePlatform

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`, `Comparable<ApplePlatform>`

    ------------------------------------------------------------------------

        public abstract class ApplePlatform
        extends Object
        implements Comparable<ApplePlatform>, AddsToRuleKey
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                     Description
          ------------------- ------------------------- -------------
          `static class `     `ApplePlatform.Builder`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                                                 Field                    Description
          ----------------------------------------------------------------- ------------------------ -------------
          `static com.google.common.collect.ImmutableList<Flavor>`          `ALL_PLATFORM_FLAVORS`    
          `static com.google.common.collect.ImmutableList<ApplePlatform>`   `ALL_PLATFORMS`           
          `static ApplePlatform`                                            `APPLETVOS`               
          `static ApplePlatform`                                            `APPLETVSIMULATOR`        
          `static ApplePlatform`                                            `DRIVERKIT`               
          `static ApplePlatform`                                            `IPHONEOS`                
          `static ApplePlatform`                                            `IPHONESIMULATOR`         
          `static ApplePlatform`                                            `MACOSX`                  
          `static ApplePlatform`                                            `WATCHOS`                 
          `static ApplePlatform`                                            `WATCHSIMULATOR`          

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor         Description
          ------------------- -------------
          `ApplePlatform()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static boolean`      | `adHocCodeSignIsSuf   |                       |
        |                       | ficient​(String name)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static A             | `builder()`           |                       |
        | pplePlatform.Builder` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `compareTo​(           |                       |
        |                       | ApplePlatform other)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `findAppleSd          |                       |
        | tic Optional<String>` | kName​(Flavor flavor)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `findArchite          |                       |
        | tic Optional<String>` | cture​(Flavor flavor)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `fromF                |                       |
        | static ApplePlatform` | lavor​(Flavor flavor)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getApp               |                       |
        |                       | IncludesFrameworks()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getArchitectures()`  |                       |
        | ogle.common.collect.I |                       |                       |
        | mmutableList<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getIsSimulator()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getMi                |                       |
        |                       | nVersionFlagPrefix()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract String`     | `getName()`           | ::: block             |
        |                       |                       | The full name of the  |
        |                       |                       | platform.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getPlatformName()`   |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstr                | `getProvi             | ::: block             |
        | act Optional<String>` | sioningProfileName()` | The platform name     |
        |                       |                       | used to match         |
        |                       |                       | provisioning          |
        |                       |                       | profiles.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstr                | `getStubBinaryPath()` |                       |
        | act Optional<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstr                | `getSwiftName()`      | ::: block             |
        | act Optional<String>` |                       | The Swift name for    |
        |                       |                       | the platform.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ApplePlatformType`   | `getType()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `isPlatformF          |                       |
        |                       | lavor​(Flavor flavor)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `isSi                 |                       |
        |                       | mulator​(String name)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `needsC               |                       |
        |                       | odeSign​(String name)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `needsEntitlementsI   |                       |
        |                       | nBinary​(String name)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `needsInstal          |                       |
        |                       | lHelper​(String name)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `of​(String name)`     |                       |
        | static ApplePlatform` |                       |                       |
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
    -   []{#field.detail}

        ### Field Detail

        []{#IPHONEOS}

        -   #### IPHONEOS

                public static final ApplePlatform IPHONEOS

        []{#IPHONESIMULATOR}

        -   #### IPHONESIMULATOR

                public static final ApplePlatform IPHONESIMULATOR

        []{#WATCHOS}

        -   #### WATCHOS

                public static final ApplePlatform WATCHOS

        []{#WATCHSIMULATOR}

        -   #### WATCHSIMULATOR

                public static final ApplePlatform WATCHSIMULATOR

        []{#APPLETVOS}

        -   #### APPLETVOS

                public static final ApplePlatform APPLETVOS

        []{#APPLETVSIMULATOR}

        -   #### APPLETVSIMULATOR

                public static final ApplePlatform APPLETVSIMULATOR

        []{#MACOSX}

        -   #### MACOSX

                public static final ApplePlatform MACOSX

        []{#DRIVERKIT}

        -   #### DRIVERKIT

                public static final ApplePlatform DRIVERKIT

        []{#ALL_PLATFORMS}

        -   #### ALL_PLATFORMS

                public static final com.google.common.collect.ImmutableList<ApplePlatform> ALL_PLATFORMS

        []{#ALL_PLATFORM_FLAVORS}

        -   #### ALL_PLATFORM_FLAVORS

                public static final com.google.common.collect.ImmutableList<Flavor> ALL_PLATFORM_FLAVORS
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### ApplePlatform

                public ApplePlatform()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getName()}

        -   #### getName

            ``` methodSignature
            public abstract String getName()
            ```

            ::: block
            The full name of the platform. For example: `macosx`.
            :::

        []{#getSwiftName()}

        -   #### getSwiftName

            ``` methodSignature
            public abstract Optional<String> getSwiftName()
            ```

            ::: block
            The Swift name for the platform. For example: `ios`. If
            absent, use [`getName()`](#getName()) instead.
            :::

        []{#getProvisioningProfileName()}

        -   #### getProvisioningProfileName

            ``` methodSignature
            public abstract Optional<String> getProvisioningProfileName()
            ```

            ::: block
            The platform name used to match provisioning profiles. For
            example: `iOS`.
            Not all platforms use provisioning profiles; these will
            return absent.
            :::

        []{#getArchitectures()}

        -   #### getArchitectures

            ``` methodSignature
            @Default
            public com.google.common.collect.ImmutableList<String> getArchitectures()
            ```

        []{#getMinVersionFlagPrefix()}

        -   #### getMinVersionFlagPrefix

            ``` methodSignature
            @Default
            public String getMinVersionFlagPrefix()
            ```

        []{#getStubBinaryPath()}

        -   #### getStubBinaryPath

            ``` methodSignature
            public abstract Optional<String> getStubBinaryPath()
            ```

        []{#getAppIncludesFrameworks()}

        -   #### getAppIncludesFrameworks

            ``` methodSignature
            @Default
            public boolean getAppIncludesFrameworks()
            ```

        []{#getType()}

        -   #### getType

            ``` methodSignature
            public ApplePlatformType getType()
            ```

        []{#getIsSimulator()}

        -   #### getIsSimulator

            ``` methodSignature
            public boolean getIsSimulator()
            ```

        []{#needsCodeSign(java.lang.String)}

        -   #### needsCodeSign

            ``` methodSignature
            public static boolean needsCodeSign​(String name)
            ```

        []{#adHocCodeSignIsSufficient(java.lang.String)}

        -   #### adHocCodeSignIsSufficient

            ``` methodSignature
            public static boolean adHocCodeSignIsSufficient​(String name)
            ```

        []{#needsInstallHelper(java.lang.String)}

        -   #### needsInstallHelper

            ``` methodSignature
            public static boolean needsInstallHelper​(String name)
            ```

        []{#needsEntitlementsInBinary(java.lang.String)}

        -   #### needsEntitlementsInBinary

            ``` methodSignature
            public static boolean needsEntitlementsInBinary​(String name)
            ```

        []{#isSimulator(java.lang.String)}

        -   #### isSimulator

            ``` methodSignature
            public static boolean isSimulator​(String name)
            ```

        []{#of(java.lang.String)}

        -   #### of

            ``` methodSignature
            public static ApplePlatform of​(String name)
            ```

        []{#isPlatformFlavor(com.facebook.buck.core.model.Flavor)}

        -   #### isPlatformFlavor

            ``` methodSignature
            public static boolean isPlatformFlavor​(Flavor flavor)
            ```

        []{#findAppleSdkName(com.facebook.buck.core.model.Flavor)}

        -   #### findAppleSdkName

            ``` methodSignature
            public static Optional<String> findAppleSdkName​(Flavor flavor)
            ```

        []{#findArchitecture(com.facebook.buck.core.model.Flavor)}

        -   #### findArchitecture

            ``` methodSignature
            public static Optional<String> findArchitecture​(Flavor flavor)
            ```

        []{#fromFlavor(com.facebook.buck.core.model.Flavor)}

        -   #### fromFlavor

            ``` methodSignature
            public static ApplePlatform fromFlavor​(Flavor flavor)
            ```

        []{#compareTo(com.facebook.buck.apple.toolchain.ApplePlatform)}

        -   #### compareTo

            ``` methodSignature
            public int compareTo​(ApplePlatform other)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `compareTo` in interface `Comparable<ApplePlatform>`

        []{#getPlatformName()}

        -   #### getPlatformName

            ``` methodSignature
            public final String getPlatformName()
            ```

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static ApplePlatform.Builder builder()
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
-   [Nested](#nested.class.summary) \| 
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

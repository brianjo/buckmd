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
[Package]{.packageLabelInType} [com.facebook.buck.apple.toolchain](package-summary.html)
:::

## Class AppleSdk {#class-applesdk .title title="Class AppleSdk"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.toolchain.AppleSdk

::: description
-   

    ------------------------------------------------------------------------

        public abstract class AppleSdk
        extends Object

    ::: block
    Metadata about an Apple SDK.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                Description
          ------------------- -------------------- -------------
          `static class `     `AppleSdk.Builder`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor    Description
          -------------- -------------
          `AppleSdk()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `sta                  | `builder()`           |                       |
        | tic AppleSdk.Builder` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ab                   | `getApplePlatform()`  | ::: block             |
        | stract ApplePlatform` |                       | The platform of the   |
        |                       |                       | SDK.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getArchitectures()`  | ::: block             |
        | abstract Set<String>` |                       | The architectures     |
        |                       |                       | supported by the SDK. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract String`     | `getName()`           | ::: block             |
        |                       |                       | The full name of the  |
        |                       |                       | SDK.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ab                   | `getToolchains()`     | ::: block             |
        | stract com.google.com |                       | The toolchains used   |
        | mon.collect.Immutable |                       | by the SDK.           |
        | List<AppleToolchain>` |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract String`     | `getVersion()`        | ::: block             |
        |                       |                       | The version number of |
        |                       |                       | the SDK.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleSdk`            | `w                    |                       |
        |                       | ithName​(String name)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `AppleSdk`            | `withVer              |                       |
        |                       | sion​(String version)` |                       |
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

        -   #### AppleSdk

                public AppleSdk()
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
            The full name of the SDK. For example: `iphonesimulator8.0`.
            :::

        []{#getVersion()}

        -   #### getVersion

            ``` methodSignature
            public abstract String getVersion()
            ```

            ::: block
            The version number of the SDK. For example: `8.0`.
            :::

        []{#getApplePlatform()}

        -   #### getApplePlatform

            ``` methodSignature
            public abstract ApplePlatform getApplePlatform()
            ```

            ::: block
            The platform of the SDK. For example, `iphoneos`.
            :::

        []{#getArchitectures()}

        -   #### getArchitectures

            ``` methodSignature
            public abstract Set<String> getArchitectures()
            ```

            ::: block
            The architectures supported by the SDK. For example:
            `[i386, x86_64]`.
            :::

        []{#getToolchains()}

        -   #### getToolchains

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<AppleToolchain> getToolchains()
            ```

            ::: block
            The toolchains used by the SDK. For example:
            `["com.apple.dt.toolchain.XcodeDefault"]`
            :::

        []{#withName(java.lang.String)}

        -   #### withName

            ``` methodSignature
            public AppleSdk withName​(String name)
            ```

        []{#withVersion(java.lang.String)}

        -   #### withVersion

            ``` methodSignature
            public AppleSdk withVersion​(String version)
            ```

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static AppleSdk.Builder builder()
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

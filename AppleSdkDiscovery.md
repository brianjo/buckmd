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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
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

## Class AppleSdkDiscovery {#class-applesdkdiscovery .title title="Class AppleSdkDiscovery"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.toolchain.impl.AppleSdkDiscovery

::: description
-   

    ------------------------------------------------------------------------

        public class AppleSdkDiscovery
        extends Object

    ::: block
    Utility class to discover the location of SDKs contained inside an
    Xcode installation.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static               | `di                   | ::: block             |
        | com.google.common.col | scoverAppleSdkPaths​(O | Given a path to an    |
        | lect.ImmutableMap<App | ptional<Path> develop | Xcode developer       |
        | leSdk,​AppleSdkPaths>` | erDir,                | directory and a map   |
        |                       |        com.google.com | of (xctoolchain ID:   |
        |                       | mon.collect.Immutable | path) pairs as        |
        |                       | List<Path> extraDirs, | returned by           |
        |                       |                       | [`A                   |
        |                       |  com.google.common.co | ppleToolchainDiscover |
        |                       | llect.ImmutableMap<St | y`](AppleToolchainDis |
        |                       | ring,​AppleToolchain>  | covery.html "class in |
        |                       | xcodeToolchains,      |  com.facebook.buck.ap |
        |                       |                  Appl | ple.toolchain.impl"), |
        |                       | eConfig appleConfig)` | walks through the     |
        |                       |                       | platforms and builds  |
        |                       |                       | a map of              |
        |                       |                       | ([`AppleSdk`](        |
        |                       |                       | ../AppleSdk.html "cla |
        |                       |                       | ss in com.facebook.bu |
        |                       |                       | ck.apple.toolchain"): |
        |                       |                       | [`                    |
        |                       |                       | AppleSdkPaths`](../Ap |
        |                       |                       | pleSdkPaths.html "cla |
        |                       |                       | ss in com.facebook.bu |
        |                       |                       | ck.apple.toolchain")) |
        |                       |                       | objects describing    |
        |                       |                       | the paths to the SDKs |
        |                       |                       | inside.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#discoverAppleSdkPaths(java.util.Optional,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableMap,com.facebook.buck.apple.AppleConfig)}

        -   #### discoverAppleSdkPaths

            ``` methodSignature
            public static com.google.common.collect.ImmutableMap<AppleSdk,​AppleSdkPaths> discoverAppleSdkPaths​(Optional<Path> developerDir,
                                                                                                                     com.google.common.collect.ImmutableList<Path> extraDirs,
                                                                                                                     com.google.common.collect.ImmutableMap<String,​AppleToolchain> xcodeToolchains,
                                                                                                                     AppleConfig appleConfig)
                                                                                                              throws IOException
            ```

            ::: block
            Given a path to an Xcode developer directory and a map of
            (xctoolchain ID: path) pairs as returned by
            [`AppleToolchainDiscovery`](AppleToolchainDiscovery.html "class in com.facebook.buck.apple.toolchain.impl"),
            walks through the platforms and builds a map of
            ([`AppleSdk`](../AppleSdk.html "class in com.facebook.buck.apple.toolchain"):
            [`AppleSdkPaths`](../AppleSdkPaths.html "class in com.facebook.buck.apple.toolchain"))
            objects describing the paths to the SDKs inside.
            The [`AppleSdk.getName()`](../AppleSdk.html#getName())
            strings match the ones displayed by `xcodebuild  -showsdks`
            and look like `macosx10.9`, `iphoneos8.0`,
            `iphonesimulator8.0`, etc.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`
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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

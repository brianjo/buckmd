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
[Package]{.packageLabelInType} [com.facebook.buck.cxx.toolchain.nativelink](package-summary.html)
:::

## Class NativeLinkableInfo.Configuration {#class-nativelinkableinfo.configuration .title title="Class NativeLinkableInfo.Configuration"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.toolchain.nativelink.NativeLinkableInfo.Configuration

::: description
-   

    Enclosing class:
    :   [NativeLinkableInfo](NativeLinkableInfo.html "class in com.facebook.buck.cxx.toolchain.nativelink")

    ------------------------------------------------------------------------

        public static class NativeLinkableInfo.Configuration
        extends Object

    ::: block
    Configuration is used for configuring the less-commonly changed
    parts of the \@{link NativeLinkableInfo}. Most cases can just use
    the default values.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                    Method                                                                                                                                                Description
          ------------------------------------ ----------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `NativeLinkableInfo.Configuration`   `setExportedLinkerFlags​(com.google.common.collect.ImmutableList<? extends Arg> exportedLinkerFlags)`                                                   
          `NativeLinkableInfo.Configuration`   `setExportedPostLinkerFlags​(com.google.common.collect.ImmutableList<? extends Arg> exportedPostLinkerFlags)`                                           
          `NativeLinkableInfo.Configuration`   `setHaskellOmnibusLinkingOptions​(boolean supportsOmnibusLinkingForHaskell,                                boolean forceLinkWholeForHaskellOmnibus)`    
          `NativeLinkableInfo.Configuration`   `setNativeLinkTarget​(Optional<? extends NativeLinkTarget> nativeLinkTarget)`                                                                           
          `NativeLinkableInfo.Configuration`   `setShouldBeLinkedInAppleTestAndHost​(boolean shouldBeLinkedInAppleTestAndHost)`                                                                        
          `NativeLinkableInfo.Configuration`   `setSupportsOmnibusLinking​(boolean supportsOmnibusLinking)`                                                                                            

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
    -   []{#method.detail}

        ### Method Detail

        []{#setExportedLinkerFlags(com.google.common.collect.ImmutableList)}

        -   #### setExportedLinkerFlags

            ``` methodSignature
            public NativeLinkableInfo.Configuration setExportedLinkerFlags​(com.google.common.collect.ImmutableList<? extends Arg> exportedLinkerFlags)
            ```

        []{#setExportedPostLinkerFlags(com.google.common.collect.ImmutableList)}

        -   #### setExportedPostLinkerFlags

            ``` methodSignature
            public NativeLinkableInfo.Configuration setExportedPostLinkerFlags​(com.google.common.collect.ImmutableList<? extends Arg> exportedPostLinkerFlags)
            ```

        []{#setSupportsOmnibusLinking(boolean)}

        -   #### setSupportsOmnibusLinking

            ``` methodSignature
            public NativeLinkableInfo.Configuration setSupportsOmnibusLinking​(boolean supportsOmnibusLinking)
            ```

        []{#setHaskellOmnibusLinkingOptions(boolean,boolean)}

        -   #### setHaskellOmnibusLinkingOptions

            ``` methodSignature
            public NativeLinkableInfo.Configuration setHaskellOmnibusLinkingOptions​(boolean supportsOmnibusLinkingForHaskell,
                                                                                    boolean forceLinkWholeForHaskellOmnibus)
            ```

        []{#setNativeLinkTarget(java.util.Optional)}

        -   #### setNativeLinkTarget

            ``` methodSignature
            public NativeLinkableInfo.Configuration setNativeLinkTarget​(Optional<? extends NativeLinkTarget> nativeLinkTarget)
            ```

        []{#setShouldBeLinkedInAppleTestAndHost(boolean)}

        -   #### setShouldBeLinkedInAppleTestAndHost

            ``` methodSignature
            public NativeLinkableInfo.Configuration setShouldBeLinkedInAppleTestAndHost​(boolean shouldBeLinkedInAppleTestAndHost)
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

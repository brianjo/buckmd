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
[Package]{.packageLabelInType} [com.facebook.buck.android.toolchain.impl](package-summary.html)
:::

## Class AndroidSdkDirectoryResolver {#class-androidsdkdirectoryresolver .title title="Class AndroidSdkDirectoryResolver"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.android.toolchain.common.BaseAndroidToolchainResolver](../common/BaseAndroidToolchainResolver.html "class in com.facebook.buck.android.toolchain.common")

    -   -   com.facebook.buck.android.toolchain.impl.AndroidSdkDirectoryResolver

::: description
-   

    ------------------------------------------------------------------------

        public class AndroidSdkDirectoryResolver
        extends BaseAndroidToolchainResolver

    ::: block
    Utility class used for resolving the location of Android specific
    directories.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.android.toolchain.common.BaseAndroidToolchainResolver}

            ### Fields inherited from class com.facebook.buck.android.toolchain.common.[BaseAndroidToolchainResolver](../common/BaseAndroidToolchainResolver.html "class in com.facebook.buck.android.toolchain.common")

            `environment, fileSystem, INVALID_DIRECTORY_MESSAGE_TEMPLATE`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                               Description
          --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `AndroidSdkDirectoryResolver​(FileSystem fileSystem,                            com.google.common.collect.ImmutableMap<String,​String> environment,                            AndroidBuckConfig config)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method              Description
          ------------------- ------------------- -------------
          `Path`              `getSdkOrThrow()`    
          `String`            `toString()`         

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.android.toolchain.common.BaseAndroidToolchainResolver}

            ### Methods inherited from class com.facebook.buck.android.toolchain.common.[BaseAndroidToolchainResolver](../common/BaseAndroidToolchainResolver.html "class in com.facebook.buck.android.toolchain.common")

            `findFirstDirectory, getEnvironmentVariable`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.nio.file.FileSystem,com.google.common.collect.ImmutableMap,com.facebook.buck.android.AndroidBuckConfig)}

        -   #### AndroidSdkDirectoryResolver

                public AndroidSdkDirectoryResolver​(FileSystem fileSystem,
                                                   com.google.common.collect.ImmutableMap<String,​String> environment,
                                                   AndroidBuckConfig config)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getSdkOrThrow()}

        -   #### getSdkOrThrow

            ``` methodSignature
            public Path getSdkOrThrow()
            ```

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`
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
-   Field \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
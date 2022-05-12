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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.android.toolchain.ndk.impl](package-summary.html)
:::

## Class AndroidNdkResolver {#class-androidndkresolver .title title="Class AndroidNdkResolver"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.android.toolchain.common.BaseAndroidToolchainResolver](../../common/BaseAndroidToolchainResolver.html "class in com.facebook.buck.android.toolchain.common")

    -   -   com.facebook.buck.android.toolchain.ndk.impl.AndroidNdkResolver

::: description
-   

    ------------------------------------------------------------------------

        public class AndroidNdkResolver
        extends BaseAndroidToolchainResolver
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.android.toolchain.common.BaseAndroidToolchainResolver}

            ### Fields inherited from class com.facebook.buck.android.toolchain.common.[BaseAndroidToolchainResolver](../../common/BaseAndroidToolchainResolver.html "class in com.facebook.buck.android.toolchain.common")

            `environment, fileSystem, INVALID_DIRECTORY_MESSAGE_TEMPLATE`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                    Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `AndroidNdkResolver​(FileSystem fileSystem,                   com.google.common.collect.ImmutableMap<String,​String> environment,                   AndroidBuckConfig config)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `boolean`             | `                     |                       |
        |                       | equals​(Object other)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `findNdkVersio        |                       |
        |                       | n​(Path ndkDirectory)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `findN                | ::: block             |
        | tic Optional<String>` | dkVersionFromDirector | The method returns    |
        |                       | y​(Path ndkDirectory)` | the NDK version of a  |
        |                       |                       | path.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getNdkOrThrow()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getNdkVersion()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.android.toolchain.common.BaseAndroidToolchainResolver}

            ### Methods inherited from class com.facebook.buck.android.toolchain.common.[BaseAndroidToolchainResolver](../../common/BaseAndroidToolchainResolver.html "class in com.facebook.buck.android.toolchain.common")

            `findFirstDirectory, getEnvironmentVariable`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.nio.file.FileSystem,com.google.common.collect.ImmutableMap,com.facebook.buck.android.AndroidBuckConfig)}

        -   #### AndroidNdkResolver

                public AndroidNdkResolver​(FileSystem fileSystem,
                                          com.google.common.collect.ImmutableMap<String,​String> environment,
                                          AndroidBuckConfig config)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getNdkOrThrow()}

        -   #### getNdkOrThrow

            ``` methodSignature
            public Path getNdkOrThrow()
            ```

        []{#getNdkVersion()}

        -   #### getNdkVersion

            ``` methodSignature
            public Optional<String> getNdkVersion()
            ```

        []{#findNdkVersionFromDirectory(java.nio.file.Path)}

        -   #### findNdkVersionFromDirectory

            ``` methodSignature
            public static Optional<String> findNdkVersionFromDirectory​(Path ndkDirectory)
            ```

            ::: block
            The method returns the NDK version of a path.
            :::

            [Parameters:]{.paramLabel}
            :   `ndkDirectory` - Path to the folder that contains the
                NDK.

            [Returns:]{.returnLabel}
            :   A string containing the NDK version or absent.

        []{#findNdkVersion(java.nio.file.Path)}

        -   #### findNdkVersion

            ``` methodSignature
            public Optional<String> findNdkVersion​(Path ndkDirectory)
            ```

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(Object other)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `Object`

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `Object`
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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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

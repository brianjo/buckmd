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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.android.exopackage](package-summary.html)
:::

## Class NativeExoHelper {#class-nativeexohelper .title title="Class NativeExoHelper"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.exopackage.NativeExoHelper

::: description
-   

    ------------------------------------------------------------------------

        public class NativeExoHelper
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field               Description
          ------------------- ------------------- -------------
          `static Path`       `NATIVE_LIBS_DIR`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                   Method                                                                                                                                                                                                                                                          Description
          ------------------------------------------------------------------- --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `static com.google.common.collect.ImmutableMultimap<String,​Path>`   `filterLibrariesForAbi​(Path nativeLibsDir,                      com.google.common.collect.ImmutableMultimap<String,​Path> allLibraries,                      String abi,                      com.google.common.collect.ImmutableSet<String> ignoreLibraries)`    
          `com.google.common.collect.ImmutableMap<Path,​Path>`                 `getFilesToInstall()`                                                                                                                                                                                                                                            
          `com.google.common.collect.ImmutableMap<Path,​String>`               `getMetadataToInstall()`                                                                                                                                                                                                                                         

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
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
    -   []{#field.detail}

        ### Field Detail

        []{#NATIVE_LIBS_DIR}

        -   #### NATIVE_LIBS_DIR

                public static final Path NATIVE_LIBS_DIR
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getFilesToInstall()}

        -   #### getFilesToInstall

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<Path,​Path> getFilesToInstall()
                                                                                      throws IOException
            ```

            [Returns:]{.returnLabel}
            :   a mapping from destinationPathOnDevice -\> localPath

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getMetadataToInstall()}

        -   #### getMetadataToInstall

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<Path,​String> getMetadataToInstall()
                                                                                           throws IOException
            ```

            [Returns:]{.returnLabel}
            :   a mapping from destinationPathOnDevice -\> contents of
                file for all native-libs metadata files (one per abi)

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#filterLibrariesForAbi(java.nio.file.Path,com.google.common.collect.ImmutableMultimap,java.lang.String,com.google.common.collect.ImmutableSet)}

        -   #### filterLibrariesForAbi

            ``` methodSignature
            public static com.google.common.collect.ImmutableMultimap<String,​Path> filterLibrariesForAbi​(Path nativeLibsDir,
                                                                                                               com.google.common.collect.ImmutableMultimap<String,​Path> allLibraries,
                                                                                                               String abi,
                                                                                                               com.google.common.collect.ImmutableSet<String> ignoreLibraries)
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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

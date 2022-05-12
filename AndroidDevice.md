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
[Package]{.packageLabelInType} [com.facebook.buck.android.exopackage](package-summary.html)
:::

## Interface AndroidDevice {#interface-androiddevice .title title="Interface AndroidDevice"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `RealAndroidDevice`

    ------------------------------------------------------------------------

        public interface AndroidDevice
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                      Method                                                                                                                                                  Description
          ------------------------------------------------------ ------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `AutoCloseable`                                        `createForward()`                                                                                                                                        
          `List<String>`                                         `getDeviceAbis()`                                                                                                                                        
          `Optional<PackageInfo>`                                `getPackageInfo​(String packageName)`                                                                                                                     
          `String`                                               `getProperty​(String name)`                                                                                                                               
          `String`                                               `getSerialNumber()`                                                                                                                                      
          `String`                                               `getSignature​(String packagePath)`                                                                                                                       
          `default boolean`                                      `installApkOnDevice​(File apk,                   boolean installViaSd,                   boolean quiet)`                                                  
          `boolean`                                              `installApkOnDevice​(File apk,                   boolean installViaSd,                   boolean quiet,                   boolean verifyTempWritable)`    
          `void`                                                 `installFiles​(String filesType,             Map<Path,​Path> installPaths)`                                                                                
          `void`                                                 `killProcess​(String processName)`                                                                                                                        
          `com.google.common.collect.ImmutableSortedSet<Path>`   `listDirRecursive​(Path dirPath)`                                                                                                                         
          `void`                                                 `mkDirP​(String dirpath)`                                                                                                                                 
          `void`                                                 `rmFiles​(String dirPath,        Iterable<String> filesToDelete)`                                                                                         
          `void`                                                 `sendBroadcast​(String action,              Map<String,​String> stringExtras)`                                                                             
          `void`                                                 `stopPackage​(String packageName)`                                                                                                                        
          `void`                                                 `uninstallPackage​(String packageName)`                                                                                                                   

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
          .tableTab}[[Default
          Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#installApkOnDevice(java.io.File,boolean,boolean)}

        -   #### installApkOnDevice

            ``` methodSignature
            default boolean installApkOnDevice​(File apk,
                                               boolean installViaSd,
                                               boolean quiet)
            ```

        []{#installApkOnDevice(java.io.File,boolean,boolean,boolean)}

        -   #### installApkOnDevice

            ``` methodSignature
            boolean installApkOnDevice​(File apk,
                                       boolean installViaSd,
                                       boolean quiet,
                                       boolean verifyTempWritable)
            ```

        []{#stopPackage(java.lang.String)}

        -   #### stopPackage

            ``` methodSignature
            void stopPackage​(String packageName)
                      throws Exception
            ```

            [Throws:]{.throwsLabel}
            :   `Exception`

        []{#getPackageInfo(java.lang.String)}

        -   #### getPackageInfo

            ``` methodSignature
            Optional<PackageInfo> getPackageInfo​(String packageName)
                                          throws Exception
            ```

            [Throws:]{.throwsLabel}
            :   `Exception`

        []{#uninstallPackage(java.lang.String)}

        -   #### uninstallPackage

            ``` methodSignature
            void uninstallPackage​(String packageName)
                           throws com.android.ddmlib.InstallException
            ```

            [Throws:]{.throwsLabel}
            :   `com.android.ddmlib.InstallException`

        []{#getSignature(java.lang.String)}

        -   #### getSignature

            ``` methodSignature
            String getSignature​(String packagePath)
                         throws Exception
            ```

            [Throws:]{.throwsLabel}
            :   `Exception`

        []{#listDirRecursive(java.nio.file.Path)}

        -   #### listDirRecursive

            ``` methodSignature
            com.google.common.collect.ImmutableSortedSet<Path> listDirRecursive​(Path dirPath)
                                                                         throws Exception
            ```

            [Throws:]{.throwsLabel}
            :   `Exception`

        []{#rmFiles(java.lang.String,java.lang.Iterable)}

        -   #### rmFiles

            ``` methodSignature
            void rmFiles​(String dirPath,
                         Iterable<String> filesToDelete)
            ```

        []{#createForward()}

        -   #### createForward

            ``` methodSignature
            AutoCloseable createForward()
                                 throws Exception
            ```

            [Throws:]{.throwsLabel}
            :   `Exception`

        []{#installFiles(java.lang.String,java.util.Map)}

        -   #### installFiles

            ``` methodSignature
            void installFiles​(String filesType,
                              Map<Path,​Path> installPaths)
                       throws Exception
            ```

            [Throws:]{.throwsLabel}
            :   `Exception`

        []{#mkDirP(java.lang.String)}

        -   #### mkDirP

            ``` methodSignature
            void mkDirP​(String dirpath)
                 throws Exception
            ```

            [Throws:]{.throwsLabel}
            :   `Exception`

        []{#getProperty(java.lang.String)}

        -   #### getProperty

            ``` methodSignature
            String getProperty​(String name)
                        throws Exception
            ```

            [Throws:]{.throwsLabel}
            :   `Exception`

        []{#getDeviceAbis()}

        -   #### getDeviceAbis

            ``` methodSignature
            List<String> getDeviceAbis()
                                throws Exception
            ```

            [Throws:]{.throwsLabel}
            :   `Exception`

        []{#killProcess(java.lang.String)}

        -   #### killProcess

            ``` methodSignature
            void killProcess​(String processName)
                      throws Exception
            ```

            [Throws:]{.throwsLabel}
            :   `Exception`

        []{#sendBroadcast(java.lang.String,java.util.Map)}

        -   #### sendBroadcast

            ``` methodSignature
            void sendBroadcast​(String action,
                               Map<String,​String> stringExtras)
                        throws Exception
            ```

            [Throws:]{.throwsLabel}
            :   `Exception`

        []{#getSerialNumber()}

        -   #### getSerialNumber

            ``` methodSignature
            String getSerialNumber()
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

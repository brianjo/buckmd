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
[Package]{.packageLabelInType} [com.facebook.buck.android.exopackage](package-summary.html)
:::

## Class RealAndroidDevice {#class-realandroiddevice .title title="Class RealAndroidDevice"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.exopackage.RealAndroidDevice

::: description
-   

    All Implemented Interfaces:
    :   `AndroidDevice`

    ------------------------------------------------------------------------

        public class RealAndroidDevice
        extends Object
        implements AndroidDevice
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `RealAndroidDevice.   | ::: block             |
        |                       | ErrorParsingReceiver` | Implementation of     |
        |                       |                       | `                     |
        |                       |                       | IShellOutputReceiver` |
        |                       |                       | with helper functions |
        |                       |                       | to parse output lines |
        |                       |                       | and figure out if a   |
        |                       |                       | call to               |
        |                       |                       | `IDevice.execute      |
        |                       |                       | ShellCommand(String,  |
        |                       |                       |  com.android.ddmlib.I |
        |                       |                       | ShellOutputReceiver)` |
        |                       |                       | succeeded.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `RealAndroidDevice​(BuckEventBus buckEventBus,                  com.android.ddmlib.IDevice device,                  Console console)`                                                                                                                                                        
          `RealAndroidDevice​(BuckEventBus eventBus,                  com.android.ddmlib.IDevice device,                  Console console,                  Path agentApkPath,                  int agentPort,                  com.google.common.collect.ImmutableList<String> rapidInstallTypes)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static com.g         | `chunkArgs​(Itera      | ::: block             |
        | oogle.common.collect. | ble<String> args,     | Breaks a list of      |
        | ImmutableList<com.goo |       int sizeLimit)` | strings into groups   |
        | gle.common.collect.Im |                       | whose total size is   |
        | mutableList<String>>` |                       | within some limit.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AutoCloseable`       | `createForward()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `de                   |                       |
        |                       | viceStartActivity​(Str |                       |
        |                       | ing activityToRun,    |                       |
        |                       |                  bool |                       |
        |                       | ean waitForDebugger)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `List<String>`        | `getDeviceAbis()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `O                    | `getPackageInfo       |                       |
        | ptional<PackageInfo>` | ​(String packageName)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getP                 |                       |
        |                       | roperty​(String name)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getSerialNumber()`   |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getSignature         |                       |
        |                       | ​(String packagePath)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `i                    |                       |
        |                       | nstallApkOnDevice​(Fil |                       |
        |                       | e apk,                |                       |
        |                       |     boolean installVi |                       |
        |                       | aSd,                  |                       |
        |                       |   boolean quiet,      |                       |
        |                       |               boolean |                       |
        |                       |  verifyTempWritable)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `installFi            |                       |
        |                       | les​(String filesType, |                       |
        |                       |              Map<Path |                       |
        |                       | ,​Path> installPaths)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isEmulator()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `killProcess          |                       |
        |                       | ​(String processName)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `listDir              |                       |
        | e.common.collect.Immu | Recursive​(Path root)` |                       |
        | tableSortedSet<Path>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `mk                   |                       |
        |                       | DirP​(String dirpath)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static O             | `p                    |                       |
        | ptional<PackageInfo>` | arsePathAndPackageInf |                       |
        |                       | o​(String packageName, |                       |
        |                       |                       |                       |
        |                       |    String rawOutput)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `                     |                       |
        |                       | rmFiles​(String dirPat |                       |
        |                       | h,        Iterable<St |                       |
        |                       | ring> filesToDelete)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `sendBroadcas         |                       |
        |                       | t​(String action,      |                       |
        |                       |          Map<String,​S |                       |
        |                       | tring> stringExtras)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `stopPackage          |                       |
        |                       | ​(String packageName)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `uninstallApkFromDevi | ::: block             |
        |                       | ce​(String packageName | Uninstalls apk from   |
        |                       | ,                     | specific device.      |
        |                       |    boolean keepData)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `uninstallPackage     |                       |
        |                       | ​(String packageName)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.android.exopackage.AndroidDevice}

            ### Methods inherited from interface com.facebook.buck.android.exopackage.[AndroidDevice](AndroidDevice.html "interface in com.facebook.buck.android.exopackage")

            `installApkOnDevice`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.event.BuckEventBus,com.android.ddmlib.IDevice,com.facebook.buck.util.Console,java.nio.file.Path,int,com.google.common.collect.ImmutableList)}

        -   #### RealAndroidDevice

                public RealAndroidDevice​(BuckEventBus eventBus,
                                         com.android.ddmlib.IDevice device,
                                         Console console,
                                         @Nullable
                                         Path agentApkPath,
                                         int agentPort,
                                         com.google.common.collect.ImmutableList<String> rapidInstallTypes)

        []{#<init>(com.facebook.buck.event.BuckEventBus,com.android.ddmlib.IDevice,com.facebook.buck.util.Console)}

        -   #### RealAndroidDevice

                public RealAndroidDevice​(BuckEventBus buckEventBus,
                                         com.android.ddmlib.IDevice device,
                                         Console console)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#chunkArgs(java.lang.Iterable,int)}

        -   #### chunkArgs

            ``` methodSignature
            public static com.google.common.collect.ImmutableList<com.google.common.collect.ImmutableList<String>> chunkArgs​(Iterable<String> args,
                                                                                                                             int sizeLimit)
            ```

            ::: block
            Breaks a list of strings into groups whose total size is
            within some limit. Kind of like the xargs command that
            groups arguments to avoid maximum argument length limits.
            Except that the limit in adb is about 1k instead of 512k or
            2M on Linux.
            :::

        []{#parsePathAndPackageInfo(java.lang.String,java.lang.String)}

        -   #### parsePathAndPackageInfo

            ``` methodSignature
            public static Optional<PackageInfo> parsePathAndPackageInfo​(String packageName,
                                                                        String rawOutput)
            ```

        []{#deviceStartActivity(java.lang.String,boolean)}

        -   #### deviceStartActivity

            ``` methodSignature
            @Nullable
            public String deviceStartActivity​(String activityToRun,
                                              boolean waitForDebugger)
            ```

        []{#uninstallApkFromDevice(java.lang.String,boolean)}

        -   #### uninstallApkFromDevice

            ``` methodSignature
            public boolean uninstallApkFromDevice​(String packageName,
                                                  boolean keepData)
            ```

            ::: block
            Uninstalls apk from specific device. Reports success or
            failure to console. It\'s currently here because it\'s used
            both by
            [`InstallCommand`](../../cli/InstallCommand.html "class in com.facebook.buck.cli")
            and
            [`UninstallCommand`](../../cli/UninstallCommand.html "class in com.facebook.buck.cli").
            :::

        []{#isEmulator()}

        -   #### isEmulator

            ``` methodSignature
            public boolean isEmulator()
            ```

        []{#installApkOnDevice(java.io.File,boolean,boolean,boolean)}

        -   #### installApkOnDevice

            ``` methodSignature
            public boolean installApkOnDevice​(File apk,
                                              boolean installViaSd,
                                              boolean quiet,
                                              boolean verifyTempWritable)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `installApkOnDevice` in interface `AndroidDevice`

        []{#stopPackage(java.lang.String)}

        -   #### stopPackage

            ``` methodSignature
            public void stopPackage​(String packageName)
                             throws Exception
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `stopPackage` in interface `AndroidDevice`

            [Throws:]{.throwsLabel}
            :   `Exception`

        []{#getPackageInfo(java.lang.String)}

        -   #### getPackageInfo

            ``` methodSignature
            public Optional<PackageInfo> getPackageInfo​(String packageName)
                                                 throws Exception
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPackageInfo` in interface `AndroidDevice`

            [Throws:]{.throwsLabel}
            :   `Exception`

        []{#uninstallPackage(java.lang.String)}

        -   #### uninstallPackage

            ``` methodSignature
            public void uninstallPackage​(String packageName)
                                  throws com.android.ddmlib.InstallException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `uninstallPackage` in interface `AndroidDevice`

            [Throws:]{.throwsLabel}
            :   `com.android.ddmlib.InstallException`

        []{#getSignature(java.lang.String)}

        -   #### getSignature

            ``` methodSignature
            public String getSignature​(String packagePath)
                                throws Exception
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSignature` in interface `AndroidDevice`

            [Throws:]{.throwsLabel}
            :   `Exception`

        []{#getSerialNumber()}

        -   #### getSerialNumber

            ``` methodSignature
            public String getSerialNumber()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSerialNumber` in interface `AndroidDevice`

        []{#listDirRecursive(java.nio.file.Path)}

        -   #### listDirRecursive

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<Path> listDirRecursive​(Path root)
                                                                                throws Exception
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `listDirRecursive` in interface `AndroidDevice`

            [Throws:]{.throwsLabel}
            :   `Exception`

        []{#rmFiles(java.lang.String,java.lang.Iterable)}

        -   #### rmFiles

            ``` methodSignature
            public void rmFiles​(String dirPath,
                                Iterable<String> filesToDelete)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `rmFiles` in interface `AndroidDevice`

        []{#createForward()}

        -   #### createForward

            ``` methodSignature
            public AutoCloseable createForward()
                                        throws Exception
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `createForward` in interface `AndroidDevice`

            [Throws:]{.throwsLabel}
            :   `Exception`

        []{#installFiles(java.lang.String,java.util.Map)}

        -   #### installFiles

            ``` methodSignature
            public void installFiles​(String filesType,
                                     Map<Path,​Path> installPaths)
                              throws Exception
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `installFiles` in interface `AndroidDevice`

            [Throws:]{.throwsLabel}
            :   `Exception`

        []{#mkDirP(java.lang.String)}

        -   #### mkDirP

            ``` methodSignature
            public void mkDirP​(String dirpath)
                        throws Exception
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `mkDirP` in interface `AndroidDevice`

            [Throws:]{.throwsLabel}
            :   `Exception`

        []{#getProperty(java.lang.String)}

        -   #### getProperty

            ``` methodSignature
            public String getProperty​(String name)
                               throws Exception
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getProperty` in interface `AndroidDevice`

            [Throws:]{.throwsLabel}
            :   `Exception`

        []{#getDeviceAbis()}

        -   #### getDeviceAbis

            ``` methodSignature
            public List<String> getDeviceAbis()
                                       throws Exception
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDeviceAbis` in interface `AndroidDevice`

            [Throws:]{.throwsLabel}
            :   `Exception`

        []{#killProcess(java.lang.String)}

        -   #### killProcess

            ``` methodSignature
            public void killProcess​(String processName)
                             throws Exception
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `killProcess` in interface `AndroidDevice`

            [Throws:]{.throwsLabel}
            :   `Exception`

        []{#sendBroadcast(java.lang.String,java.util.Map)}

        -   #### sendBroadcast

            ``` methodSignature
            public void sendBroadcast​(String action,
                                      Map<String,​String> stringExtras)
                               throws Exception
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `sendBroadcast` in interface `AndroidDevice`

            [Throws:]{.throwsLabel}
            :   `Exception`
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

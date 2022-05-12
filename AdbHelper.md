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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.android](package-summary.html)
:::

## Class AdbHelper {#class-adbhelper .title title="Class AdbHelper"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.AdbHelper

::: description
-   

    All Implemented Interfaces:
    :   `AndroidDevicesHelper`, `Closeable`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class AdbHelper
        extends Object
        implements AndroidDevicesHelper

    ::: block
    Helper for executing commands over ADB, especially for multiple
    devices.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `AdbHelper.Co         | ::: block             |
        |                       | mmandFailedException` | An exception that     |
        |                       |                       | indicates that an     |
        |                       |                       | executed command      |
        |                       |                       | returned an           |
        |                       |                       | unsuccessful exit     |
        |                       |                       | code.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.android.exopackage.AndroidDevicesHelper}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.android.exopackage.[AndroidDevicesHelper](exopackage/AndroidDevicesHelper.html "interface in com.facebook.buck.android.exopackage")

            `AndroidDevicesHelper.AdbDeviceCallable`
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Field                 | Description           |
        +=======================+=======================+=======================+
        | `static Pattern`      | `                     | ::: block             |
        |                       | PACKAGE_NAME_PATTERN` | Pattern that matches  |
        |                       |                       | safe package names.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                              Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `AdbHelper​(AdbOptions adbOptions,          TargetDeviceOptions deviceOptions,          ToolchainProvider toolchainProvider,          java.util.function.Supplier<ExecutionContext> contextSupplier,          boolean restartAdbOnFailure,          com.google.common.collect.ImmutableList<String> rapidInstallTypes)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `adbCall​(String des   | ::: block             |
        |                       | cription,        Andr | Execute an            |
        |                       | oidDevicesHelper.AdbD | [`A                   |
        |                       | eviceCallable func,   | ndroidDevicesHelper.A |
        |                       |       boolean quiet)` | dbDeviceCallable`](ex |
        |                       |                       | opackage/AndroidDevic |
        |                       |                       | esHelper.AdbDeviceCal |
        |                       |                       | lable.html "interface |
        |                       |                       |  in com.facebook.buck |
        |                       |                       | .android.exopackage") |
        |                       |                       | for all matching      |
        |                       |                       | devices.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `close()`             |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.co        | `getDe                |                       |
        | mmon.collect.Immutabl | vices​(boolean quiet)` |                       |
        | eList<AndroidDevice>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `installApk​(Source    | ::: block             |
        |                       | PathResolverAdapter p | Install apk on all    |
        |                       | athResolver,          | matching devices.     |
        |                       |   HasInstallableApk h | :::                   |
        |                       | asInstallableApk,     |                       |
        |                       |        boolean instal |                       |
        |                       | lViaSd,           boo |                       |
        |                       | lean quiet,           |                       |
        |                       |  String processName)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `setDevicesSupplierFo |                       |
        |                       | rTests​(Optional<java. |                       |
        |                       | util.function.Supplie |                       |
        |                       | r<com.google.common.c |                       |
        |                       | ollect.ImmutableList< |                       |
        |                       | AndroidDevice>>> devi |                       |
        |                       | cesSupplierForTests)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `star                 |                       |
        |                       | tActivity​(SourcePathR |                       |
        |                       | esolverAdapter pathRe |                       |
        |                       | solver,               |                       |
        |                       | HasInstallableApk has |                       |
        |                       | InstallableApk,       |                       |
        |                       |         String activi |                       |
        |                       | ty,              bool |                       |
        |                       | ean waitForDebugger)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `tryToExtractPackageN |                       |
        |                       | ameFromManifest​(Sourc |                       |
        |                       | ePathResolverAdapter  |                       |
        |                       | pathResolver,         |                       |
        |                       |                       |                       |
        |                       |        HasInstallable |                       |
        |                       | Apk.ApkInfo apkInfo)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `uninstallA           | ::: block             |
        |                       | pp​(String packageName | Uninstall apk from    |
        |                       | ,             boolean | all matching devices. |
        |                       |  shouldKeepUserData)` | :::                   |
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
        -   []{#methods.inherited.from.class.com.facebook.buck.android.exopackage.AndroidDevicesHelper}

            ### Methods inherited from interface com.facebook.buck.android.exopackage.[AndroidDevicesHelper](exopackage/AndroidDevicesHelper.html "interface in com.facebook.buck.android.exopackage")

            `adbCallOrThrow`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#PACKAGE_NAME_PATTERN}

        -   #### PACKAGE_NAME_PATTERN

                public static final Pattern PACKAGE_NAME_PATTERN

            ::: block
            Pattern that matches safe package names. (Must be a full
            string match).
            :::
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.step.AdbOptions,com.facebook.buck.android.device.TargetDeviceOptions,com.facebook.buck.core.toolchain.ToolchainProvider,java.util.function.Supplier,boolean,com.google.common.collect.ImmutableList)}

        -   #### AdbHelper

                public AdbHelper​(AdbOptions adbOptions,
                                 TargetDeviceOptions deviceOptions,
                                 ToolchainProvider toolchainProvider,
                                 java.util.function.Supplier<ExecutionContext> contextSupplier,
                                 boolean restartAdbOnFailure,
                                 com.google.common.collect.ImmutableList<String> rapidInstallTypes)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#setDevicesSupplierForTests(java.util.Optional)}

        -   #### setDevicesSupplierForTests

            ``` methodSignature
            public static void setDevicesSupplierForTests​(Optional<java.util.function.Supplier<com.google.common.collect.ImmutableList<AndroidDevice>>> devicesSupplierForTests)
            ```

        []{#getDevices(boolean)}

        -   #### getDevices

            ``` methodSignature
            public com.google.common.collect.ImmutableList<AndroidDevice> getDevices​(boolean quiet)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDevices` in interface `AndroidDevicesHelper`

        []{#adbCall(java.lang.String,com.facebook.buck.android.exopackage.AndroidDevicesHelper.AdbDeviceCallable,boolean)}

        -   #### adbCall

            ``` methodSignature
            public void adbCall​(String description,
                                AndroidDevicesHelper.AdbDeviceCallable func,
                                boolean quiet)
                         throws InterruptedException
            ```

            ::: block
            Execute an
            [`AndroidDevicesHelper.AdbDeviceCallable`](exopackage/AndroidDevicesHelper.AdbDeviceCallable.html "interface in com.facebook.buck.android.exopackage")
            for all matching devices. This functions performs device
            filtering based on three possible arguments:
            -e (emulator-only) - only emulators are passing the filter
            -d (device-only) - only real devices are passing the filter
            -s (serial) - only device/emulator with specific serial
            number are passing the filter

            If more than one device matches the filter this function
            will fail unless multi-install mode is enabled (-x). This
            flag is used as a marker that user understands that multiple
            devices will be used to install the apk if needed.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `adbCall` in interface `AndroidDevicesHelper`

            [Throws:]{.throwsLabel}
            :   `InterruptedException`

        []{#installApk(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,com.facebook.buck.android.HasInstallableApk,boolean,boolean,java.lang.String)}

        -   #### installApk

            ``` methodSignature
            public void installApk​(SourcePathResolverAdapter pathResolver,
                                   HasInstallableApk hasInstallableApk,
                                   boolean installViaSd,
                                   boolean quiet,
                                   @Nullable
                                   String processName)
                            throws InterruptedException
            ```

            ::: block
            [Description copied from
            interface: `AndroidDevicesHelper`]{.descfrmTypeLabel}
            :::

            ::: block
            Install apk on all matching devices. This functions performs
            device filtering based on three possible arguments:
            -e (emulator-only) - only emulators are passing the filter
            -d (device-only) - only real devices are passing the filter
            -s (serial) - only device/emulator with specific serial
            number are passing the filter

            If more than one device matches the filter this function
            will fail unless multi-install mode is enabled (-x). This
            flag is used as a marker that user understands that multiple
            devices will be used to install the apk if needed.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `installApk` in interface `AndroidDevicesHelper`

            [Throws:]{.throwsLabel}
            :   `InterruptedException`

        []{#startActivity(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,com.facebook.buck.android.HasInstallableApk,java.lang.String,boolean)}

        -   #### startActivity

            ``` methodSignature
            public void startActivity​(SourcePathResolverAdapter pathResolver,
                                      HasInstallableApk hasInstallableApk,
                                      @Nullable
                                      String activity,
                                      boolean waitForDebugger)
                               throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `startActivity` in interface `AndroidDevicesHelper`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#uninstallApp(java.lang.String,boolean)}

        -   #### uninstallApp

            ``` methodSignature
            public void uninstallApp​(String packageName,
                                     boolean shouldKeepUserData)
                              throws InterruptedException
            ```

            ::: block
            Uninstall apk from all matching devices.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `uninstallApp` in interface `AndroidDevicesHelper`

            [Throws:]{.throwsLabel}
            :   `InterruptedException`

            [See Also:]{.seeLabel}
            :   [`installApk(SourcePathResolverAdapter, HasInstallableApk, boolean, boolean, String)`](#installApk(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,com.facebook.buck.android.HasInstallableApk,boolean,boolean,java.lang.String))

        []{#tryToExtractPackageNameFromManifest(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,com.facebook.buck.android.HasInstallableApk.ApkInfo)}

        -   #### tryToExtractPackageNameFromManifest

            ``` methodSignature
            public static String tryToExtractPackageNameFromManifest​(SourcePathResolverAdapter pathResolver,
                                                                     HasInstallableApk.ApkInfo apkInfo)
            ```

        []{#close()}

        -   #### close

            ``` methodSignature
            public void close()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `Closeable`
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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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

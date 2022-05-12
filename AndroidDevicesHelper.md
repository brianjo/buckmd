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

## Interface AndroidDevicesHelper {#interface-androiddeviceshelper .title title="Interface AndroidDevicesHelper"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `AutoCloseable`, `Closeable`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `AdbHelper`

    ------------------------------------------------------------------------

        public interface AndroidDevicesHelper
        extends Closeable

    ::: block
    AndroidDevicesHelper provides a way to interact with multiple
    devices as AndroidDevices (rather than IDevices).
    All of ExopackageInstaller\'s interaction with devices and adb goes
    through this class and AndroidDevice making it easy to provide
    different implementations in tests.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Interface             | Description           |
        +=======================+=======================+=======================+
        | `static interface `   | `AndroidDevicesHelp   | ::: block             |
        |                       | er.AdbDeviceCallable` | This is basically the |
        |                       |                       | same as               |
        |                       |                       | AdbHelper.AdbCallable |
        |                       |                       | except that it takes  |
        |                       |                       | an AndroidDevice      |
        |                       |                       | instead of an         |
        |                       |                       | IDevice.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `adbCall​(String des   |                       |
        |                       | cription,        Andr |                       |
        |                       | oidDevicesHelper.AdbD |                       |
        |                       | eviceCallable func,   |                       |
        |                       |       boolean quiet)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default void`        | `adbCallOrThrow​(Str   | ::: block             |
        |                       | ing description,      | A simple wrapper      |
        |                       |           AndroidDevi | around adbCall that   |
        |                       | cesHelper.AdbDeviceCa | will throw if adbCall |
        |                       | llable func,          | returns false.        |
        |                       |       boolean quiet)` | :::                   |
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
        |                       |  String packageName)` |                       |
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
        | `void`                | `uninstallA           | ::: block             |
        |                       | pp​(String packageName | Uninstall apk from    |
        |                       | ,             boolean | all matching devices. |
        |                       |  shouldKeepUserData)` | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Default
        Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}

        -   []{#methods.inherited.from.class.java.io.Closeable}

            ### Methods inherited from interface java.io.[Closeable](http://docs.oracle.com/javase/7/docs/api/java/io/Closeable.html?is-external=true "class or interface in java.io"){.externalLink}

            `close`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#adbCallOrThrow(java.lang.String,com.facebook.buck.android.exopackage.AndroidDevicesHelper.AdbDeviceCallable,boolean)}

        -   #### adbCallOrThrow

            ``` methodSignature
            default void adbCallOrThrow​(String description,
                                        AndroidDevicesHelper.AdbDeviceCallable func,
                                        boolean quiet)
                                 throws InterruptedException
            ```

            ::: block
            A simple wrapper around adbCall that will throw if adbCall
            returns false.
            :::

            [Throws:]{.throwsLabel}
            :   `InterruptedException`

        []{#adbCall(java.lang.String,com.facebook.buck.android.exopackage.AndroidDevicesHelper.AdbDeviceCallable,boolean)}

        -   #### adbCall

            ``` methodSignature
            void adbCall​(String description,
                         AndroidDevicesHelper.AdbDeviceCallable func,
                         boolean quiet)
                  throws InterruptedException
            ```

            [Throws:]{.throwsLabel}
            :   `InterruptedException`

        []{#getDevices(boolean)}

        -   #### getDevices

            ``` methodSignature
            com.google.common.collect.ImmutableList<AndroidDevice> getDevices​(boolean quiet)
            ```

        []{#installApk(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,com.facebook.buck.android.HasInstallableApk,boolean,boolean,java.lang.String)}

        -   #### installApk

            ``` methodSignature
            void installApk​(SourcePathResolverAdapter pathResolver,
                            HasInstallableApk hasInstallableApk,
                            boolean installViaSd,
                            boolean quiet,
                            @Nullable
                            String packageName)
                     throws InterruptedException
            ```

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

            [Throws:]{.throwsLabel}
            :   `InterruptedException`

        []{#uninstallApp(java.lang.String,boolean)}

        -   #### uninstallApp

            ``` methodSignature
            void uninstallApp​(String packageName,
                              boolean shouldKeepUserData)
                       throws InterruptedException
            ```

            ::: block
            Uninstall apk from all matching devices.
            :::

            [Throws:]{.throwsLabel}
            :   `InterruptedException`

            [See Also:]{.seeLabel}
            :   [`installApk(SourcePathResolverAdapter, HasInstallableApk, boolean, boolean, String)`](#installApk(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,com.facebook.buck.android.HasInstallableApk,boolean,boolean,java.lang.String))

        []{#startActivity(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,com.facebook.buck.android.HasInstallableApk,java.lang.String,boolean)}

        -   #### startActivity

            ``` methodSignature
            void startActivity​(SourcePathResolverAdapter pathResolver,
                               HasInstallableApk hasInstallableApk,
                               @Nullable
                               String activity,
                               boolean waitForDebugger)
                        throws IOException
            ```

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

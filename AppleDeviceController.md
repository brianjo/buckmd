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
[Package]{.packageLabelInType} [com.facebook.buck.apple.simulator](package-summary.html)
:::

## Class AppleDeviceController {#class-appledevicecontroller .title title="Class AppleDeviceController"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.simulator.AppleDeviceController

::: description
-   

    ------------------------------------------------------------------------

        public class AppleDeviceController
        extends Object

    ::: block
    Utility class to control Apple Devices (both simulators and physical
    devices). Examples include booting them, installing and launching
    bundles inside of the devices.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `                     | ::: block             |
        |                       | AppleDeviceController | Enum indicating the   |
        |                       | .AppleDeviceKindEnum` | different kinds of    |
        |                       |                       | devices possible      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `AppleDeviceContr     | ::: block             |
        |                       | oller.LaunchBehavior` | Enum for the          |
        |                       |                       | different ways to     |
        |                       |                       | launch the simulator  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                   Description
          --------------------------------------------------------------------------------------------- -------------
          `AppleDeviceController​(ProcessExecutor processExecutor,                      Path idbPath)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `boolean`             | `bootSimulator​(S      | ::: block             |
        |                       | tring simulatorUdid)` | Starts up the iOS     |
        |                       |                       | simulator using idb,  |
        |                       |                       | which waits until the |
        |                       |                       | simulator is          |
        |                       |                       | completely booted.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `br                   | ::: block             |
        |                       | ingSimulatorToFront​(S | Brings the desired    |
        |                       | tring simulatorUdid)` | simulator to the      |
        |                       |                       | front                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.g                | `getBoo               |                       |
        | oogle.common.collect. | tedSimulatorsUdids()` |                       |
        | ImmutableSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getDeviceKind        |                       |
        | AppleDeviceController | ​(AppleDevice device)` |                       |
        | .AppleDeviceKindEnum` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `                     |                       |
        | .common.collect.Immut | getPhysicalDevices()` |                       |
        | ableSet<AppleDevice>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `getSimulators()`     |                       |
        | .common.collect.Immut |                       |                       |
        | ableSet<AppleDevice>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getSi                | ::: block             |
        |                       | mulatorUdidForTest()` | Picks the simulator   |
        |                       |                       | to be used for        |
        |                       |                       | testing               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getUdidFromDev       |                       |
        |                       | iceName​(String name)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `                     | ::: block             |
        |                       | installBundle​(String  | Installs a bundle in  |
        |                       | deviceUdid,           | a previously-started  |
        |                       |     Path bundlePath)` | simulator or physical |
        |                       |                       | device.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `i                    |                       |
        |                       | sSimulatorAvailable​(S |                       |
        |                       | tring simulatorUdid)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `launchInstalledB     | ::: block             |
        |                       | undle​(String deviceUd | Launches an installed |
        |                       | id,                   | bundle in a device    |
        |                       |     String bundleID)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `startD               | ::: block             |
        |                       | ebugServer​(String dev | Starts the            |
        |                       | iceUdid,              | debugserver of the    |
        |                       |     String bundleID)` | installed app         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.util.ProcessExecutor,java.nio.file.Path)}

        -   #### AppleDeviceController

                public AppleDeviceController​(ProcessExecutor processExecutor,
                                             Path idbPath)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getSimulators()}

        -   #### getSimulators

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<AppleDevice> getSimulators()
            ```

            [Returns:]{.returnLabel}
            :   the set of Apple simulators

        []{#getPhysicalDevices()}

        -   #### getPhysicalDevices

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<AppleDevice> getPhysicalDevices()
            ```

            [Returns:]{.returnLabel}
            :   the set of Apple physical devices

        []{#getBootedSimulatorsUdids()}

        -   #### getBootedSimulatorsUdids

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<String> getBootedSimulatorsUdids()
            ```

            [Returns:]{.returnLabel}
            :   set of udids of the booted devices

        []{#getUdidFromDeviceName(java.lang.String)}

        -   #### getUdidFromDeviceName

            ``` methodSignature
            public Optional<String> getUdidFromDeviceName​(String name)
            ```

            [Returns:]{.returnLabel}
            :   the udid of the device that has the determined name. If
                no device is found with that name, will return optional
                empty

        []{#getSimulatorUdidForTest()}

        -   #### getSimulatorUdidForTest

            ``` methodSignature
            public Optional<String> getSimulatorUdidForTest()
            ```

            ::: block
            Picks the simulator to be used for testing
            :::

            [Returns:]{.returnLabel}
            :   the udid of any booted simulator (iphone) and if there
                are none returns any simulator. If there are none,
                returns optional empty

        []{#bootSimulator(java.lang.String)}

        -   #### bootSimulator

            ``` methodSignature
            public boolean bootSimulator​(String simulatorUdid)
                                  throws IOException,
                                         InterruptedException
            ```

            ::: block
            Starts up the iOS simulator using idb, which waits until the
            simulator is completely booted.
            Call
            [`isSimulatorAvailable(String)`](#isSimulatorAvailable(java.lang.String))
            before invoking this method to ensure the simulator is
            available.
            :::

            [Returns:]{.returnLabel}
            :   true if idb was able to boot the simulator, false
                otherwise

            [Throws:]{.throwsLabel}
            :   `IOException`
            :   `InterruptedException`

        []{#isSimulatorAvailable(java.lang.String)}

        -   #### isSimulatorAvailable

            ``` methodSignature
            public boolean isSimulatorAvailable​(String simulatorUdid)
            ```

            [Parameters:]{.paramLabel}
            :   `simulatorUdid` - of the simulator is available

            [Returns:]{.returnLabel}
            :   true if the simulator is available, false otherwise

        []{#installBundle(java.lang.String,java.nio.file.Path)}

        -   #### installBundle

            ``` methodSignature
            public Optional<String> installBundle​(String deviceUdid,
                                                  Path bundlePath)
                                           throws IOException,
                                                  InterruptedException
            ```

            ::: block
            Installs a bundle in a previously-started simulator or
            physical device.
            :::

            [Returns:]{.returnLabel}
            :   true if the bundle was installed, false otherwise.

            [Throws:]{.throwsLabel}
            :   `IOException`
            :   `InterruptedException`

        []{#bringSimulatorToFront(java.lang.String)}

        -   #### bringSimulatorToFront

            ``` methodSignature
            public boolean bringSimulatorToFront​(String simulatorUdid)
                                          throws IOException,
                                                 InterruptedException
            ```

            ::: block
            Brings the desired simulator to the front
            :::

            [Returns:]{.returnLabel}
            :   true if it managed to do so, false otherwise

            [Throws:]{.throwsLabel}
            :   `IOException`
            :   `InterruptedException`

        []{#launchInstalledBundle(java.lang.String,java.lang.String)}

        -   #### launchInstalledBundle

            ``` methodSignature
            public boolean launchInstalledBundle​(String deviceUdid,
                                                 String bundleID)
                                          throws IOException,
                                                 InterruptedException
            ```

            ::: block
            Launches an installed bundle in a device
            :::

            [Returns:]{.returnLabel}
            :   true if it was able to launch and false otherwise

            [Throws:]{.throwsLabel}
            :   `IOException`
            :   `InterruptedException`

        []{#startDebugServer(java.lang.String,java.lang.String)}

        -   #### startDebugServer

            ``` methodSignature
            public Optional<String> startDebugServer​(String deviceUdid,
                                                     String bundleID)
                                              throws IOException,
                                                     InterruptedException
            ```

            ::: block
            Starts the debugserver of the installed app
            :::

            [Returns:]{.returnLabel}
            :   the command to be run in lldb

            [Throws:]{.throwsLabel}
            :   `IOException`
            :   `InterruptedException`

        []{#getDeviceKind(com.facebook.buck.apple.simulator.AppleDevice)}

        -   #### getDeviceKind

            ``` methodSignature
            public AppleDeviceController.AppleDeviceKindEnum getDeviceKind​(AppleDevice device)
            ```

            [Parameters:]{.paramLabel}
            :   `device` - to be analized

            [Returns:]{.returnLabel}
            :   the enum indicating the kind of device it is
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

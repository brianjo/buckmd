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
[Package]{.packageLabelInType} [com.facebook.buck.apple.device](package-summary.html)
:::

## Class AppleDeviceHelper {#class-appledevicehelper .title title="Class AppleDeviceHelper"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.device.AppleDeviceHelper

::: description
-   

    ------------------------------------------------------------------------

        public class AppleDeviceHelper
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                    Description
          ---------------------------------------------------------------------------------------------- -------------
          `AppleDeviceHelper​(ProcessExecutor processExecutor,                  Path deviceHelperPath)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.google.c         | `g                    | ::: block             |
        | ommon.collect.Immutab | etConnectedDevices()` | Runs the helper       |
        | leMap<String,​String>` |                       | program to enumerate  |
        |                       |                       | all                   |
        |                       |                       | currently-connected   |
        |                       |                       | devices.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `installBun           | ::: block             |
        |                       | dleOnDevice​(String ud | Attempts to install a |
        |                       | id,                   | bundle on the device. |
        |                       |     Path bundlePath)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `ru                   | ::: block             |
        |                       | nBundleOnDevice​(Strin | Attempts to run a     |
        |                       | g udid,               | bundle on the device. |
        |                       |     String bundleID)` | :::                   |
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

        -   #### AppleDeviceHelper

                public AppleDeviceHelper​(ProcessExecutor processExecutor,
                                         Path deviceHelperPath)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getConnectedDevices()}

        -   #### getConnectedDevices

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​String> getConnectedDevices()
            ```

            ::: block
            Runs the helper program to enumerate all currently-connected
            devices.
            :::

            [Returns:]{.returnLabel}
            :   A ImmutableMap with entries where the key is the UDID of
                the device, and the value is a human readable
                description (e.g. \"iPhone (iPhone 5S) (USB)\")

            [Throws:]{.throwsLabel}
            :   `IOException`
            :   `InterruptedException`

        []{#installBundleOnDevice(java.lang.String,java.nio.file.Path)}

        -   #### installBundleOnDevice

            ``` methodSignature
            public boolean installBundleOnDevice​(String udid,
                                                 Path bundlePath)
            ```

            ::: block
            Attempts to install a bundle on the device. The bundle must
            be code-signed already.
            :::

            [Parameters:]{.paramLabel}
            :   `udid` - The identifier of the device
            :   `bundlePath` - The path to the bundle root (e.g.
                `/path/to/Example.app/`)

            [Returns:]{.returnLabel}
            :   true if successful, false otherwise.

        []{#runBundleOnDevice(java.lang.String,java.lang.String)}

        -   #### runBundleOnDevice

            ``` methodSignature
            public boolean runBundleOnDevice​(String udid,
                                             String bundleID)
            ```

            ::: block
            Attempts to run a bundle on the device. The bundle must be
            installed already.
            :::

            [Parameters:]{.paramLabel}
            :   `udid` - The identifier of the device
            :   `bundleID` - The bundle ID (e.g. `com.example.DemoApp`)

            [Returns:]{.returnLabel}
            :   true if successful, false otherwise.
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

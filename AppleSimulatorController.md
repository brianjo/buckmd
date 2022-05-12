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

## Class AppleSimulatorController {#class-applesimulatorcontroller .title title="Class AppleSimulatorController"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.simulator.AppleSimulatorController

::: description
-   

    ------------------------------------------------------------------------

        public class AppleSimulatorController
        extends Object

    ::: block
    Utility class to manage starting the iOS simulator as well as
    installing and running applications inside it.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                                       Description
          ------------------- ------------------------------------------- -------------
          `static class `     `AppleSimulatorController.LaunchBehavior`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                           Description
          ----------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `AppleSimulatorController​(ProcessExecutor processExecutor,                         Path simctlPath,                         Path iosSimulatorPath)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `boolean`             | `canStartSimulator​(S  |                       |
        |                       | tring simulatorUdid)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `inst                 | ::: block             |
        |                       | allBundleInSimulator​( | Installs a bundle in  |
        |                       | String simulatorUdid, | a previously-started  |
        |                       |                       | simulator.            |
        |                       |     Path bundlePath)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Long>`      | `launchInstal         | ::: block             |
        |                       | ledBundleInSimulator​( | Launches a            |
        |                       | String simulatorUdid, | previously-installed  |
        |                       |                       | bundle in a started   |
        |                       |             String bu | simulator.            |
        |                       | ndleID,               | :::                   |
        |                       |                    Ap |                       |
        |                       | pleSimulatorControlle |                       |
        |                       | r.LaunchBehavior laun |                       |
        |                       | chBehavior,           |                       |
        |                       |                       |                       |
        |                       |   List<String> args)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Long>`      | `startSim             | ::: block             |
        |                       | ulator​(String simulat | Starts up the iOS     |
        |                       | orUdid,               | simulator, blocking   |
        |                       |  long timeoutMillis)` | the calling thread    |
        |                       |                       | until the simulator   |
        |                       |                       | boots or              |
        |                       |                       | `  timeoutMillis`     |
        |                       |                       | passes, whichever     |
        |                       |                       | happens first.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Long>`      | `waitFo               | ::: block             |
        |                       | rSimulatorsToShutdown | Waits up to           |
        |                       | ​(long timeoutMillis)` | `timeoutMillis` for   |
        |                       |                       | all simulators to     |
        |                       |                       | shut down.            |
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

        []{#<init>(com.facebook.buck.util.ProcessExecutor,java.nio.file.Path,java.nio.file.Path)}

        -   #### AppleSimulatorController

                public AppleSimulatorController​(ProcessExecutor processExecutor,
                                                Path simctlPath,
                                                Path iosSimulatorPath)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#startSimulator(java.lang.String,long)}

        -   #### startSimulator

            ``` methodSignature
            public Optional<Long> startSimulator​(String simulatorUdid,
                                                 long timeoutMillis)
                                          throws IOException,
                                                 InterruptedException
            ```

            ::: block
            Starts up the iOS simulator, blocking the calling thread
            until the simulator boots or `  timeoutMillis` passes,
            whichever happens first.
            Call
            [`canStartSimulator(String)`](#canStartSimulator(java.lang.String))
            before invoking this method to ensure the simulator can be
            started.
            :::

            [Returns:]{.returnLabel}
            :   The number of milliseconds waited if the simulator
                booted successfully, `      Optional.empty()` otherwise.

            [Throws:]{.throwsLabel}
            :   `IOException`
            :   `InterruptedException`

        []{#canStartSimulator(java.lang.String)}

        -   #### canStartSimulator

            ``` methodSignature
            public boolean canStartSimulator​(String simulatorUdid)
                                      throws IOException,
                                             InterruptedException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`
            :   `InterruptedException`

        []{#waitForSimulatorsToShutdown(long)}

        -   #### waitForSimulatorsToShutdown

            ``` methodSignature
            public Optional<Long> waitForSimulatorsToShutdown​(long timeoutMillis)
                                                       throws IOException,
                                                              InterruptedException
            ```

            ::: block
            Waits up to `timeoutMillis` for all simulators to shut down.
            :::

            [Returns:]{.returnLabel}
            :   The number of milliseconds waited if all simulators have
                shut down, `      Optional.empty()` otherwise.

            [Throws:]{.throwsLabel}
            :   `IOException`
            :   `InterruptedException`

        []{#installBundleInSimulator(java.lang.String,java.nio.file.Path)}

        -   #### installBundleInSimulator

            ``` methodSignature
            public boolean installBundleInSimulator​(String simulatorUdid,
                                                    Path bundlePath)
                                             throws IOException,
                                                    InterruptedException
            ```

            ::: block
            Installs a bundle in a previously-started simulator.
            :::

            [Returns:]{.returnLabel}
            :   true if the bundle was installed, false otherwise.

            [Throws:]{.throwsLabel}
            :   `IOException`
            :   `InterruptedException`

        []{#launchInstalledBundleInSimulator(java.lang.String,java.lang.String,com.facebook.buck.apple.simulator.AppleSimulatorController.LaunchBehavior,java.util.List)}

        -   #### launchInstalledBundleInSimulator

            ``` methodSignature
            public Optional<Long> launchInstalledBundleInSimulator​(String simulatorUdid,
                                                                   String bundleID,
                                                                   AppleSimulatorController.LaunchBehavior launchBehavior,
                                                                   List<String> args)
                                                            throws IOException,
                                                                   InterruptedException
            ```

            ::: block
            Launches a previously-installed bundle in a started
            simulator.
            :::

            [Returns:]{.returnLabel}
            :   the process ID of the newly-launched process if
                successful, an absent value otherwise.

            [Throws:]{.throwsLabel}
            :   `IOException`
            :   `InterruptedException`
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

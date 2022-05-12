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
[Package]{.packageLabelInType} [com.facebook.buck.apple.simulator](package-summary.html)
:::

## Class AppleSimulatorDiscovery {#class-applesimulatordiscovery .title title="Class AppleSimulatorDiscovery"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.simulator.AppleSimulatorDiscovery

::: description
-   

    ------------------------------------------------------------------------

        public class AppleSimulatorDiscovery
        extends Object

    ::: block
    Utilty class to discover state about Apple simulators installed on
    the host system.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static Opt           | `discoverAppleSimula  | ::: block             |
        | ional<com.facebook.bu | torProfile​(AppleSimul | Given a simulators,   |
        | ck.apple.simulator.Ap | ator appleSimulator,  | looks up metadata on  |
        | pleSimulatorProfile>` |                       | the supported         |
        |                       |         Path iphonesi | architectures and     |
        |                       | mulatorPlatformRoot)` | product families for  |
        |                       |                       | that simulator (if    |
        |                       |                       | present).             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static com.google.co | `discoverApple        |                       |
        | mmon.collect.Immutabl | Simulators​(ProcessExe |                       |
        | eSet<AppleSimulator>` | cutor processExecutor |                       |
        |                       | ,                     |                       |
        |                       |     Path simctlPath)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#discoverAppleSimulators(com.facebook.buck.util.ProcessExecutor,java.nio.file.Path)}

        -   #### discoverAppleSimulators

            ``` methodSignature
            public static com.google.common.collect.ImmutableSet<AppleSimulator> discoverAppleSimulators​(ProcessExecutor processExecutor,
                                                                                                         Path simctlPath)
                                                                                                  throws InterruptedException,
                                                                                                         IOException
            ```

            [Throws:]{.throwsLabel}
            :   `InterruptedException`
            :   `IOException`

        []{#discoverAppleSimulatorProfile(com.facebook.buck.apple.simulator.AppleSimulator,java.nio.file.Path)}

        -   #### discoverAppleSimulatorProfile

            ``` methodSignature
            public static Optional<com.facebook.buck.apple.simulator.AppleSimulatorProfile> discoverAppleSimulatorProfile​(AppleSimulator appleSimulator,
                                                                                                                          Path iphonesimulatorPlatformRoot)
                                                                                                                   throws IOException
            ```

            ::: block
            Given a simulators, looks up metadata on the supported
            architectures and product families for that simulator (if
            present).
            :::

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

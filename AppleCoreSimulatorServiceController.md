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
[Package]{.packageLabelInType} [com.facebook.buck.apple.simulator](package-summary.html)
:::

## Class AppleCoreSimulatorServiceController {#class-applecoresimulatorservicecontroller .title title="Class AppleCoreSimulatorServiceController"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.simulator.AppleCoreSimulatorServiceController

::: description
-   

    ------------------------------------------------------------------------

        public class AppleCoreSimulatorServiceController
        extends Object

    ::: block
    Launches, queries, and kills Apple\'s `CoreSimulator` and related
    `launchd` services.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                              Description
          ------------------------------------------------------------------------ -------------
          `AppleCoreSimulatorServiceController​(ProcessExecutor processExecutor)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Optional<Path>`      | `getCoreSimulato      | ::: block             |
        |                       | rServicePath​(UserIdFe | Returns the path on   |
        |                       | tcher userIdFetcher)` | disk to the running   |
        |                       |                       | Core Simulator        |
        |                       |                       | service, if any.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `kill                 | ::: block             |
        |                       | SimulatorProcesses()` | Kills any running     |
        |                       |                       | simulator processes   |
        |                       |                       | or services.          |
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

        []{#<init>(com.facebook.buck.util.ProcessExecutor)}

        -   #### AppleCoreSimulatorServiceController

                public AppleCoreSimulatorServiceController​(ProcessExecutor processExecutor)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getCoreSimulatorServicePath(com.facebook.buck.util.UserIdFetcher)}

        -   #### getCoreSimulatorServicePath

            ``` methodSignature
            public Optional<Path> getCoreSimulatorServicePath​(UserIdFetcher userIdFetcher)
                                                       throws IOException,
                                                              InterruptedException
            ```

            ::: block
            Returns the path on disk to the running Core Simulator
            service, if any. Returns `  Optional.empty()` unless exactly
            one Core Simulator service is running.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`
            :   `InterruptedException`

        []{#killSimulatorProcesses()}

        -   #### killSimulatorProcesses

            ``` methodSignature
            public boolean killSimulatorProcesses()
                                           throws IOException,
                                                  InterruptedException
            ```

            ::: block
            Kills any running simulator processes or services.
            :::

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

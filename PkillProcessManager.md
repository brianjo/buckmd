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
[Package]{.packageLabelInType} [com.facebook.buck.util](package-summary.html)
:::

## Class PkillProcessManager {#class-pkillprocessmanager .title title="Class PkillProcessManager"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.PkillProcessManager

::: description
-   

    All Implemented Interfaces:
    :   `ProcessManager`

    ------------------------------------------------------------------------

        public class PkillProcessManager
        extends Object
        implements ProcessManager

    ::: block
    Checks for and kills processes by name.
    Only supported on non-Windows platforms (depends on `pkill` binary).
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                              Description
          -------------------------------------------------------- -------------
          `PkillProcessManager​(ProcessExecutor processExecutor)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `boolean`             | `isProcessRunning     | ::: block             |
        |                       | ​(String processName)` | Returns true if the   |
        |                       |                       | named process is      |
        |                       |                       | running, false        |
        |                       |                       | otherwise.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `killProcess          | ::: block             |
        |                       | ​(String processName)` | Kills the process if  |
        |                       |                       | it\'s running.        |
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

        -   #### PkillProcessManager

                public PkillProcessManager​(ProcessExecutor processExecutor)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#isProcessRunning(java.lang.String)}

        -   #### isProcessRunning

            ``` methodSignature
            public boolean isProcessRunning​(String processName)
                                     throws InterruptedException,
                                            IOException
            ```

            ::: block
            [Description copied from
            interface: `ProcessManager`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns true if the named process is running, false
            otherwise.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `isProcessRunning` in interface `ProcessManager`

            [Throws:]{.throwsLabel}
            :   `InterruptedException`
            :   `IOException`

        []{#killProcess(java.lang.String)}

        -   #### killProcess

            ``` methodSignature
            public void killProcess​(String processName)
                             throws InterruptedException,
                                    IOException
            ```

            ::: block
            [Description copied from
            interface: `ProcessManager`]{.descfrmTypeLabel}
            :::

            ::: block
            Kills the process if it\'s running.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `killProcess` in interface `ProcessManager`

            [Throws:]{.throwsLabel}
            :   `InterruptedException`
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

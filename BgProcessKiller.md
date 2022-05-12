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
[Package]{.packageLabelInType} [com.facebook.buck.util](package-summary.html)
:::

## Class BgProcessKiller {#class-bgprocesskiller .title title="Class BgProcessKiller"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.BgProcessKiller

::: description
-   

    ------------------------------------------------------------------------

        public class BgProcessKiller
        extends Object

    ::: block
    Safely kill background processes on nailgun client exit. All process
    creation must synchronize on the class object\'s monitor lock to
    make sure children inherit the correct signal handler set.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static void`         | `disarm()`            |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `init()`              |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `in                   | ::: block             |
        |                       | terruptBgProcesses()` | Sends SIGINT to all   |
        |                       |                       | background processes  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static com.zaxxer    | `startProcess​(        | ::: block             |
        | .nuprocess.NuProcess` | com.zaxxer.nuprocess. | Use this method       |
        |                       | NuProcessBuilder pb)` | instead of            |
        |                       |                       | `NuPr                 |
        |                       |                       | ocessBuilder.start()` |
        |                       |                       | in order to properly  |
        |                       |                       | synchronize with      |
        |                       |                       | signal handling.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Process`      | `startProces          | ::: block             |
        |                       | s​(ProcessBuilder pb)` | Use this method       |
        |                       |                       | instead of            |
        |                       |                       | [`Pr                  |
        |                       |                       | ocessBuilder.start()` |
        |                       |                       | ](http://docs.oracle. |
        |                       |                       | com/javase/7/docs/api |
        |                       |                       | /java/lang/ProcessBui |
        |                       |                       | lder.html?is-external |
        |                       |                       | =true#start() "class  |
        |                       |                       | or interface in java. |
        |                       |                       | lang"){.externalLink} |
        |                       |                       | in order to properly  |
        |                       |                       | synchronize with      |
        |                       |                       | signal handling.      |
        |                       |                       | :::                   |
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

        []{#init()}

        -   #### init

            ``` methodSignature
            public static void init()
            ```

        []{#disarm()}

        -   #### disarm

            ``` methodSignature
            public static void disarm()
            ```

        []{#interruptBgProcesses()}

        -   #### interruptBgProcesses

            ``` methodSignature
            public static void interruptBgProcesses()
            ```

            ::: block
            Sends SIGINT to all background processes
            :::

        []{#startProcess(java.lang.ProcessBuilder)}

        -   #### startProcess

            ``` methodSignature
            public static Process startProcess​(ProcessBuilder pb)
                                        throws IOException
            ```

            ::: block
            Use this method instead of
            [`ProcessBuilder.start()`](http://docs.oracle.com/javase/7/docs/api/java/lang/ProcessBuilder.html?is-external=true#start() "class or interface in java.lang"){.externalLink}
            in order to properly synchronize with signal handling.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#startProcess(com.zaxxer.nuprocess.NuProcessBuilder)}

        -   #### startProcess

            ``` methodSignature
            public static com.zaxxer.nuprocess.NuProcess startProcess​(com.zaxxer.nuprocess.NuProcessBuilder pb)
            ```

            ::: block
            Use this method instead of `NuProcessBuilder.start()` in
            order to properly synchronize with signal handling.
            :::
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

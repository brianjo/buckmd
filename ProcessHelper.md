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

## Class ProcessHelper {#class-processhelper .title title="Class ProcessHelper"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.ProcessHelper

::: description
-   

    ------------------------------------------------------------------------

        public class ProcessHelper
        extends Object

    ::: block
    A helper singleton that provides facilities such as extracting the
    native process id of a
    [`Process`](http://docs.oracle.com/javase/7/docs/api/java/lang/Process.html?is-external=true "class or interface in java.lang"){.externalLink}
    or gathering the process resource consumption.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `                     | `getInstance()`       | ::: block             |
        | static ProcessHelper` |                       | Gets the singleton    |
        |                       |                       | instance of this      |
        |                       |                       | class.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Long`                | `getPid()`            | ::: block             |
        |                       |                       | Gets the native       |
        |                       |                       | process identifier    |
        |                       |                       | for the current       |
        |                       |                       | process.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Long`                | `ge                   | ::: block             |
        |                       | tPid​(Object process)` | Gets the native       |
        |                       |                       | process identifier    |
        |                       |                       | for the given process |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Proces               | `getProcessResourceC  | ::: block             |
        | sResourceConsumption` | onsumption​(long pid)` | Gets resource         |
        |                       |                       | consumption of the    |
        |                       |                       | process with the      |
        |                       |                       | given pid.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Proces               | `getTotalResourceC    | ::: block             |
        | sResourceConsumption` | onsumption​(long pid)` | Gets resource         |
        |                       |                       | consumption of the    |
        |                       |                       | process subtree       |
        |                       |                       | rooted at the process |
        |                       |                       | with the given pid.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `hasProcessFini       |                       |
        |                       | shed​(Object process)` |                       |
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
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getInstance()}

        -   #### getInstance

            ``` methodSignature
            public static ProcessHelper getInstance()
            ```

            ::: block
            Gets the singleton instance of this class.
            :::

        []{#getTotalResourceConsumption(long)}

        -   #### getTotalResourceConsumption

            ``` methodSignature
            @Nullable
            public ProcessResourceConsumption getTotalResourceConsumption​(long pid)
            ```

            ::: block
            Gets resource consumption of the process subtree rooted at
            the process with the given pid.
            :::

        []{#getProcessResourceConsumption(long)}

        -   #### getProcessResourceConsumption

            ``` methodSignature
            @Nullable
            public ProcessResourceConsumption getProcessResourceConsumption​(long pid)
            ```

            ::: block
            Gets resource consumption of the process with the given pid.
            :::

        []{#hasProcessFinished(java.lang.Object)}

        -   #### hasProcessFinished

            ``` methodSignature
            public boolean hasProcessFinished​(Object process)
            ```

            [Returns:]{.returnLabel}
            :   whether the process has finished executing or not.

        []{#getPid()}

        -   #### getPid

            ``` methodSignature
            @Nullable
            public Long getPid()
            ```

            ::: block
            Gets the native process identifier for the current process.
            :::

        []{#getPid(java.lang.Object)}

        -   #### getPid

            ``` methodSignature
            @Nullable
            public Long getPid​(Object process)
            ```

            ::: block
            Gets the native process identifier for the given process
            instance.
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

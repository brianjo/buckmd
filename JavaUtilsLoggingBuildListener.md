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
[Package]{.packageLabelInType} [com.facebook.buck.event.listener](package-summary.html)
:::

## Class JavaUtilsLoggingBuildListener {#class-javautilsloggingbuildlistener .title title="Class JavaUtilsLoggingBuildListener"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.event.listener.JavaUtilsLoggingBuildListener

::: description
-   

    All Implemented Interfaces:
    :   `BuckEventListener`, `Closeable`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class JavaUtilsLoggingBuildListener
        extends Object
        implements BuckEventListener

    ::: block
    Logs build events to java.util.logging.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                     Description
          --------------------------------------------------------------- -------------
          `JavaUtilsLoggingBuildListener​(ProjectFilesystem filesystem)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `bu                   |                       |
        |                       | ildFinished​(BuildEven |                       |
        |                       | t.Finished finished)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `buildStarted​(BuildEv |                       |
        |                       | ent.Started started)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `close()`             | ::: block             |
        |                       |                       | Cleanup, output any   |
        |                       |                       | trace data collected  |
        |                       |                       | to the backing store. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `closeLogFile()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `ruleF                |                       |
        |                       | inished​(BuildRuleEven |                       |
        |                       | t.Finished finished)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `ru                   |                       |
        |                       | leResumed​(BuildRuleEv |                       |
        |                       | ent.Resumed resumed)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `ru                   |                       |
        |                       | leStarted​(BuildRuleEv |                       |
        |                       | ent.Started started)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `ruleSusp             |                       |
        |                       | ended​(BuildRuleEvent. |                       |
        |                       | Suspended suspended)` |                       |
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### JavaUtilsLoggingBuildListener

                public JavaUtilsLoggingBuildListener​(ProjectFilesystem filesystem)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#buildStarted(com.facebook.buck.core.build.event.BuildEvent.Started)}

        -   #### buildStarted

            ``` methodSignature
            public void buildStarted​(BuildEvent.Started started)
            ```

        []{#buildFinished(com.facebook.buck.core.build.event.BuildEvent.Finished)}

        -   #### buildFinished

            ``` methodSignature
            public void buildFinished​(BuildEvent.Finished finished)
            ```

        []{#ruleStarted(com.facebook.buck.core.build.event.BuildRuleEvent.Started)}

        -   #### ruleStarted

            ``` methodSignature
            public void ruleStarted​(BuildRuleEvent.Started started)
            ```

        []{#ruleFinished(com.facebook.buck.core.build.event.BuildRuleEvent.Finished)}

        -   #### ruleFinished

            ``` methodSignature
            public void ruleFinished​(BuildRuleEvent.Finished finished)
            ```

        []{#ruleResumed(com.facebook.buck.core.build.event.BuildRuleEvent.Resumed)}

        -   #### ruleResumed

            ``` methodSignature
            public void ruleResumed​(BuildRuleEvent.Resumed resumed)
            ```

        []{#ruleSuspended(com.facebook.buck.core.build.event.BuildRuleEvent.Suspended)}

        -   #### ruleSuspended

            ``` methodSignature
            public void ruleSuspended​(BuildRuleEvent.Suspended suspended)
            ```

        []{#close()}

        -   #### close

            ``` methodSignature
            public void close()
            ```

            ::: block
            [Description copied from
            interface: `BuckEventListener`]{.descfrmTypeLabel}
            :::

            ::: block
            Cleanup, output any trace data collected to the backing
            store.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `BuckEventListener`

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `Closeable`

        []{#closeLogFile()}

        -   #### closeLogFile

            ``` methodSignature
            public static void closeLogFile()
            ```
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

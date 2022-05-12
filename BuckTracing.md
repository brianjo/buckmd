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
[Package]{.packageLabelInType} [com.facebook.buck.event.api](package-summary.html)
:::

## Class BuckTracing {#class-bucktracing .title title="Class BuckTracing"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.event.api.BuckTracing

::: description
-   

    ------------------------------------------------------------------------

        public final class BuckTracing
        extends Object

    ::: block
    Allows annotation processors and other compiler plug-ins to output
    tracing information to Buck\'s trace files (when being run
    in-process in Buck). These methods do nothing if called within
    another build system.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `class `              | `Buck                 | ::: block             |
        |                       | Tracing.TraceSection` | An                    |
        |                       |                       | [`AutoC               |
        |                       |                       | loseable`](http://doc |
        |                       |                       | s.oracle.com/javase/7 |
        |                       |                       | /docs/api/java/lang/A |
        |                       |                       | utoCloseable.html?is- |
        |                       |                       | external=true "class  |
        |                       |                       | or interface in java. |
        |                       |                       | lang"){.externalLink} |
        |                       |                       | that can be used in a |
        |                       |                       | try-with-resources    |
        |                       |                       | block to ensure a     |
        |                       |                       | trace section is      |
        |                       |                       | ended properly when   |
        |                       |                       | exited.               |
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
        | `void`                | `beg                  | ::: block             |
        |                       | in​(String eventName)` | Records the beginning |
        |                       |                       | of a traced section.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `begin​(String         | ::: block             |
        |                       |  eventName,      Map< | Records the beginning |
        |                       | String,​String> args)` | of a traced section.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `clearCurre           | ::: block             |
        |                       | ntThreadTracingInterf | Used by Buck to       |
        |                       | aceFromJsr199Javac()` | disconnect this class |
        |                       |                       | from its tracing      |
        |                       |                       | mechanism.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `end()`               | ::: block             |
        |                       |                       | Records the end of    |
        |                       |                       | the traced section    |
        |                       |                       | started by the most   |
        |                       |                       | recent call to        |
        |                       |                       | [                     |
        |                       |                       | `begin(String,  Map)` |
        |                       |                       | ](#begin(java.lang.St |
        |                       |                       | ring,java.util.Map)), |
        |                       |                       | on *any*              |
        |                       |                       | [`BuckTra             |
        |                       |                       | cing`](BuckTracing.ht |
        |                       |                       | ml "class in com.face |
        |                       |                       | book.buck.event.api") |
        |                       |                       | object, on the        |
        |                       |                       | current thread.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `end​(Map<             | ::: block             |
        |                       | String,​String> args)` | Records the end of    |
        |                       |                       | the traced section    |
        |                       |                       | started by the most   |
        |                       |                       | recent call to        |
        |                       |                       | [                     |
        |                       |                       | `begin(String,  Map)` |
        |                       |                       | ](#begin(java.lang.St |
        |                       |                       | ring,java.util.Map)), |
        |                       |                       | on *any*              |
        |                       |                       | [`BuckTra             |
        |                       |                       | cing`](BuckTracing.ht |
        |                       |                       | ml "class in com.face |
        |                       |                       | book.buck.event.api") |
        |                       |                       | object, on the        |
        |                       |                       | current thread.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static BuckTracing`  | `getInstanc           | ::: block             |
        |                       | e​(String pluginName)` | Gets an instance of   |
        |                       |                       | [`BuckTra             |
        |                       |                       | cing`](BuckTracing.ht |
        |                       |                       | ml "class in com.face |
        |                       |                       | book.buck.event.api") |
        |                       |                       | for tracing in the    |
        |                       |                       | given plugin.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `setCurr              | ::: block             |
        |                       | entThreadTracingInter | Used by Buck to       |
        |                       | faceFromJsr199Javac​(B | connect this class to |
        |                       | uckTracingInterface b | its tracing           |
        |                       | uckTracingInterface)` | mechanism.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Buck                 | `traceSecti           |                       |
        | Tracing.TraceSection` | on​(String eventName)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Buck                 | `trace                | ::: block             |
        | Tracing.TraceSection` | Section​(String eventN | Records the beginning |
        |                       | ame,             Map< | of a traced section,  |
        |                       | String,​String> args)` | and returns an object |
        |                       |                       | that can be used      |
        |                       |                       | within a              |
        |                       |                       | try-with-resources    |
        |                       |                       | block to              |
        |                       |                       | automatically end the |
        |                       |                       | section.              |
        |                       |                       | :::                   |
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

        []{#getInstance(java.lang.String)}

        -   #### getInstance

            ``` methodSignature
            public static BuckTracing getInstance​(String pluginName)
            ```

            ::: block
            Gets an instance of
            [`BuckTracing`](BuckTracing.html "class in com.facebook.buck.event.api")
            for tracing in the given plugin. All
            [`BuckTracing`](BuckTracing.html "class in com.facebook.buck.event.api")
            instances are backed by the same trace buffer, so
            [`begin(String, Map)`](#begin(java.lang.String,java.util.Map))
            and [`end(Map)`](#end(java.util.Map))} calls on a given
            thread must nest across all instances.
            :::

        []{#traceSection(java.lang.String)}

        -   #### traceSection

            ``` methodSignature
            public BuckTracing.TraceSection traceSection​(String eventName)
            ```

        []{#traceSection(java.lang.String,java.util.Map)}

        -   #### traceSection

            ``` methodSignature
            public BuckTracing.TraceSection traceSection​(String eventName,
                                                         Map<String,​String> args)
            ```

            ::: block
            Records the beginning of a traced section, and returns an
            object that can be used within a try-with-resources block to
            automatically end the section. The section will appear in
            the trace labeled with eventName.
            :::

        []{#begin(java.lang.String)}

        -   #### begin

            ``` methodSignature
            public void begin​(String eventName)
            ```

            ::: block
            Records the beginning of a traced section. The section will
            appear in the trace labeled with eventName.
            For best results, this call should be immediately before a
            try block, and a corresponding call to
            [`end(Map)`](#end(java.util.Map)) should be in the finally
            block. Consider using
            [`traceSection(String)`](#traceSection(java.lang.String)) in
            a try-with-resources block instead.
            :::

        []{#begin(java.lang.String,java.util.Map)}

        -   #### begin

            ``` methodSignature
            public void begin​(String eventName,
                              Map<String,​String> args)
            ```

            ::: block
            Records the beginning of a traced section. The section will
            appear in the trace labeled with eventName, and the supplied
            arguments will be visible when the section is selected.
            For best results, this call should be immediately before a
            try block, and a corresponding call to
            [`end(Map)`](#end(java.util.Map)) should be in the finally
            block. Consider using
            [`traceSection(String, Map)`](#traceSection(java.lang.String,java.util.Map))
            in a try-with-resources block instead.
            :::

        []{#end()}

        -   #### end

            ``` methodSignature
            public void end()
            ```

            ::: block
            Records the end of the traced section started by the most
            recent call to
            [`begin(String,  Map)`](#begin(java.lang.String,java.util.Map)),
            on *any*
            [`BuckTracing`](BuckTracing.html "class in com.facebook.buck.event.api")
            object, on the current thread.
            For best results, this call should be in a finally block,
            with the corresponding
            [`begin(String, Map)`](#begin(java.lang.String,java.util.Map))
            call immediately before the try.
            :::

        []{#end(java.util.Map)}

        -   #### end

            ``` methodSignature
            public void end​(Map<String,​String> args)
            ```

            ::: block
            Records the end of the traced section started by the most
            recent call to
            [`begin(String,  Map)`](#begin(java.lang.String,java.util.Map)),
            on *any*
            [`BuckTracing`](BuckTracing.html "class in com.facebook.buck.event.api")
            object, on the current thread. Arguments supplied here will
            be added to those supplied to
            [`begin(String, Map)`](#begin(java.lang.String,java.util.Map));
            conflicting entries will be overwritten.
            For best results, this call should be in a finally block,
            with the corresponding
            [`begin(String, Map)`](#begin(java.lang.String,java.util.Map))
            call immediately before the try.
            :::

        []{#setCurrentThreadTracingInterfaceFromJsr199Javac(com.facebook.buck.event.api.BuckTracingInterface)}

        -   #### setCurrentThreadTracingInterfaceFromJsr199Javac

            ``` methodSignature
            public static void setCurrentThreadTracingInterfaceFromJsr199Javac​(BuckTracingInterface buckTracingInterface)
            ```

            ::: block
            Used by Buck to connect this class to its tracing mechanism.
            There is no need to call this method manually.
            :::

        []{#clearCurrentThreadTracingInterfaceFromJsr199Javac()}

        -   #### clearCurrentThreadTracingInterfaceFromJsr199Javac

            ``` methodSignature
            public static void clearCurrentThreadTracingInterfaceFromJsr199Javac()
            ```

            ::: block
            Used by Buck to disconnect this class from its tracing
            mechanism. There is no need to call this method manually.
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

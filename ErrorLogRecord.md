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
[Package]{.packageLabelInType} [com.facebook.buck.log](package-summary.html)
:::

## Class ErrorLogRecord {#class-errorlogrecord .title title="Class ErrorLogRecord"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.log.ErrorLogRecord

::: description
-   

    ------------------------------------------------------------------------

        public abstract class ErrorLogRecord
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                      Description
          ------------------- -------------------------- -------------
          `static class `     `ErrorLogRecord.Builder`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor          Description
          -------------------- -------------
          `ErrorLogRecord()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static Er            | `builder()`           |                       |
        | rorLogRecord.Builder` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getBuildUuid()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getCategory()`       | ::: block             |
        |                       |                       | Computes a category   |
        |                       |                       | key based on relevant |
        |                       |                       | LogRecord             |
        |                       |                       | information.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getErrorMessage()`   |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getInitialError()`   |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `                     |                       |
        |                       | getInitialErrorMsg()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Boolean>`   | `getIsDaemon()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Boolean>`   | `ge                   |                       |
        |                       | tIsRemoteExecution()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Boolean>`   | `getIsS               |                       |
        |                       | uperConsoleEnabled()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getLogger()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract com.go      | `getLogs()`           |                       |
        | ogle.common.collect.I |                       |                       |
        | mmutableList<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getMessage()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getOrigin()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract LogRecord`  | `getRecord()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<            | `getStack()`          |                       |
        | StackTraceElement[]>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `long`                | `getTime()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.c         | `getTraits()`         |                       |
        | ommon.collect.Immutab |                       |                       |
        | leMap<String,​String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
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

        []{#<init>()}

        -   #### ErrorLogRecord

                public ErrorLogRecord()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getRecord()}

        -   #### getRecord

            ``` methodSignature
            public abstract LogRecord getRecord()
            ```

        []{#getLogs()}

        -   #### getLogs

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<String> getLogs()
            ```

        []{#getTraits()}

        -   #### getTraits

            ``` methodSignature
            @Derived
            public com.google.common.collect.ImmutableMap<String,​String> getTraits()
            ```

        []{#getMessage()}

        -   #### getMessage

            ``` methodSignature
            @Derived
            public String getMessage()
            ```

        []{#getCategory()}

        -   #### getCategory

            ``` methodSignature
            @Default
            public String getCategory()
            ```

            ::: block
            Computes a category key based on relevant LogRecord
            information. If an exception is present, categorizes on the
            class + method that threw it. If no exception is found,
            categorizes on the logger name and the beginning of the
            message.
            :::

        []{#getTime()}

        -   #### getTime

            ``` methodSignature
            @Derived
            public long getTime()
            ```

        []{#getLogger()}

        -   #### getLogger

            ``` methodSignature
            @Derived
            public Optional<String> getLogger()
            ```

        []{#getBuildUuid()}

        -   #### getBuildUuid

            ``` methodSignature
            @Default
            public String getBuildUuid()
            ```

        []{#getIsSuperConsoleEnabled()}

        -   #### getIsSuperConsoleEnabled

            ``` methodSignature
            @Derived
            public Optional<Boolean> getIsSuperConsoleEnabled()
            ```

        []{#getIsDaemon()}

        -   #### getIsDaemon

            ``` methodSignature
            @Derived
            public Optional<Boolean> getIsDaemon()
            ```

        []{#getIsRemoteExecution()}

        -   #### getIsRemoteExecution

            ``` methodSignature
            @Derived
            public Optional<Boolean> getIsRemoteExecution()
            ```

        []{#getStack()}

        -   #### getStack

            ``` methodSignature
            @Derived
            public Optional<StackTraceElement[]> getStack()
            ```

        []{#getErrorMessage()}

        -   #### getErrorMessage

            ``` methodSignature
            @Derived
            public Optional<String> getErrorMessage()
            ```

        []{#getInitialError()}

        -   #### getInitialError

            ``` methodSignature
            @Derived
            public Optional<String> getInitialError()
            ```

        []{#getInitialErrorMsg()}

        -   #### getInitialErrorMsg

            ``` methodSignature
            @Derived
            public Optional<String> getInitialErrorMsg()
            ```

        []{#getOrigin()}

        -   #### getOrigin

            ``` methodSignature
            @Derived
            public Optional<String> getOrigin()
            ```

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static ErrorLogRecord.Builder builder()
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

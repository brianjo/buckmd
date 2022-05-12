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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.util.log](package-summary.html)
:::

## Class Logger {#class-logger .title title="Class Logger"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.util.log.Logger

::: description
-   

    ------------------------------------------------------------------------

        public class Logger
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `addHand              |                       |
        |                       | ler​(Handler handler)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `d                    | ::: block             |
        |                       | ebug​(String message)` | Logs a message at     |
        |                       |                       | DEBUG level.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `                     | ::: block             |
        |                       | debug​(String format,  | Logs a message at     |
        |                       |      Object... args)` | DEBUG level.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `debug​(               | ::: block             |
        |                       | Throwable exception,  | Logs a message at     |
        |                       |      String message)` | DEBUG level.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `debug                | ::: block             |
        |                       | ​(Throwable exception, | Logs a message at     |
        |                       |       String format,  | DEBUG level.          |
        |                       |      Object... args)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `e                    | ::: block             |
        |                       | rror​(String message)` | Logs a message at     |
        |                       |                       | ERROR level.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `                     | ::: block             |
        |                       | error​(String format,  | Logs a message at     |
        |                       |      Object... args)` | ERROR level.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `error​(               | ::: block             |
        |                       | Throwable exception)` | Logs a message at     |
        |                       |                       | ERROR level.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `error​(               | ::: block             |
        |                       | Throwable exception,  | Logs a message at     |
        |                       |      String message)` | ERROR level.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `error                | ::: block             |
        |                       | ​(Throwable exception, | Logs a message at     |
        |                       |       String format,  | ERROR level.          |
        |                       |      Object... args)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Logger`       | `get​(Class<?> clazz)` | ::: block             |
        |                       |                       | Gets a logger named   |
        |                       |                       | after a class\' fully |
        |                       |                       | qualified name.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Logger`       | `get​(String name)`    | ::: block             |
        |                       |                       | Gets a named logger   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Handler[]`           | `getHandlers()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Level`               | `getLevel()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `                     | ::: block             |
        |                       | info​(String message)` | Logs a message at     |
        |                       |                       | INFO level.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `info​(String format,  | ::: block             |
        |                       |      Object... args)` | Logs a message at     |
        |                       |                       | INFO level.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `in                   | ::: block             |
        |                       | fo​(Throwable exceptio | Logs a message at     |
        |                       | n,     String format, | INFO level.           |
        |                       |      Object... args)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isDebugEnabled()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isL                  |                       |
        |                       | oggable​(Level level)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isVerboseEnabled()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `setL                 |                       |
        |                       | evel​(Level newLevel)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `ver                  | ::: block             |
        |                       | bose​(String message)` | Logs a message at     |
        |                       |                       | VERBOSE level.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `verb                 | ::: block             |
        |                       | ose​(String format,    | Logs a message at     |
        |                       |      Object... args)` | VERBOSE level.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `verbose​(Th           | ::: block             |
        |                       | rowable exception,    | Logs a message at     |
        |                       |      String message)` | VERBOSE level.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `verbose​(Thr          | ::: block             |
        |                       | owable exception,     | Logs a message at     |
        |                       |     String format,    | VERBOSE level.        |
        |                       |      Object... args)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `                     | ::: block             |
        |                       | warn​(String message)` | Logs a message at     |
        |                       |                       | WARN level.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `warn​(String format,  | ::: block             |
        |                       |      Object... args)` | Logs a message at     |
        |                       |                       | WARN level.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `warn                 | ::: block             |
        |                       | ​(Throwable exception, | Logs a message at     |
        |                       |      String message)` | WARN level.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `wa                   | ::: block             |
        |                       | rn​(Throwable exceptio | Logs a message at     |
        |                       | n,     String format, | WARN level.           |
        |                       |      Object... args)` | :::                   |
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

        []{#get(java.lang.Class)}

        -   #### get

            ``` methodSignature
            public static Logger get​(Class<?> clazz)
            ```

            ::: block
            Gets a logger named after a class\' fully qualified name.
            :::

            [Parameters:]{.paramLabel}
            :   `clazz` - the class

            [Returns:]{.returnLabel}
            :   the named logger

        []{#get(java.lang.String)}

        -   #### get

            ``` methodSignature
            public static Logger get​(String name)
            ```

            ::: block
            Gets a named logger
            :::

            [Parameters:]{.paramLabel}
            :   `name` - the name of the logger

            [Returns:]{.returnLabel}
            :   the named logger

        []{#verbose(java.lang.Throwable,java.lang.String)}

        -   #### verbose

            ``` methodSignature
            public void verbose​(Throwable exception,
                                String message)
            ```

            ::: block
            Logs a message at VERBOSE level.
            :::

            [Parameters:]{.paramLabel}
            :   `exception` - an exception associated with the verbose
                message being logged
            :   `message` - a literal message to log

        []{#verbose(java.lang.String)}

        -   #### verbose

            ``` methodSignature
            public void verbose​(String message)
            ```

            ::: block
            Logs a message at VERBOSE level.
            :::

            [Parameters:]{.paramLabel}
            :   `message` - a literal message to log

        []{#verbose(java.lang.String,java.lang.Object...)}

        -   #### verbose

            ``` methodSignature
            public void verbose​(String format,
                                Object... args)
            ```

            ::: block
            Logs a message at VERBOSE level.\
            Usage example:
                    logger.verbose("value is %s (%d ms)", value, time);
                 

            If the format string is invalid or the arguments are
            insufficient, an error will be logged and execution will
            continue.
            :::

            [Parameters:]{.paramLabel}
            :   `format` - a format string compatible with
                String.format()
            :   `args` - arguments for the format string

        []{#verbose(java.lang.Throwable,java.lang.String,java.lang.Object...)}

        -   #### verbose

            ``` methodSignature
            public void verbose​(@Nullable
                                Throwable exception,
                                String format,
                                Object... args)
            ```

            ::: block
            Logs a message at VERBOSE level.\
            Usage example:
                    logger.verbose(e, "value is %s (%d ms)", value, time);
                 

            If the format string is invalid or the arguments are
            insufficient, an error will be logged and execution will
            continue.
            :::

            [Parameters:]{.paramLabel}
            :   `exception` - an exception associated with the verbose
                message being logged
            :   `format` - a format string compatible with
                String.format()
            :   `args` - arguments for the format string

        []{#debug(java.lang.Throwable,java.lang.String)}

        -   #### debug

            ``` methodSignature
            public void debug​(Throwable exception,
                              String message)
            ```

            ::: block
            Logs a message at DEBUG level.
            :::

            [Parameters:]{.paramLabel}
            :   `exception` - an exception associated with the debug
                message being logged
            :   `message` - a literal message to log

        []{#debug(java.lang.String)}

        -   #### debug

            ``` methodSignature
            public void debug​(String message)
            ```

            ::: block
            Logs a message at DEBUG level.
            :::

            [Parameters:]{.paramLabel}
            :   `message` - a literal message to log

        []{#debug(java.lang.String,java.lang.Object...)}

        -   #### debug

            ``` methodSignature
            public void debug​(String format,
                              Object... args)
            ```

            ::: block
            Logs a message at DEBUG level.\
            Usage example:
                    logger.debug("value is %s (%d ms)", value, time);
                 

            If the format string is invalid or the arguments are
            insufficient, an error will be logged and execution will
            continue.
            :::

            [Parameters:]{.paramLabel}
            :   `format` - a format string compatible with
                String.format()
            :   `args` - arguments for the format string

        []{#debug(java.lang.Throwable,java.lang.String,java.lang.Object...)}

        -   #### debug

            ``` methodSignature
            public void debug​(@Nullable
                              Throwable exception,
                              String format,
                              Object... args)
            ```

            ::: block
            Logs a message at DEBUG level.\
            Usage example:
                    logger.debug(e, "value is %s (%d ms)", value, time);
                 

            If the format string is invalid or the arguments are
            insufficient, an error will be logged and execution will
            continue.
            :::

            [Parameters:]{.paramLabel}
            :   `exception` - an exception associated with the debug
                message being logged
            :   `format` - a format string compatible with
                String.format()
            :   `args` - arguments for the format string

        []{#info(java.lang.String)}

        -   #### info

            ``` methodSignature
            public void info​(String message)
            ```

            ::: block
            Logs a message at INFO level.
            :::

            [Parameters:]{.paramLabel}
            :   `message` - a literal message to log

        []{#info(java.lang.Throwable,java.lang.String,java.lang.Object...)}

        -   #### info

            ``` methodSignature
            public void info​(@Nullable
                             Throwable exception,
                             String format,
                             Object... args)
            ```

            ::: block
            Logs a message at INFO level.\
            Usage example:
                    logger.info("value is %s (%d ms)", value, time);
                 

            If the format string is invalid or the arguments are
            insufficient, an error will be logged and execution will
            continue.
            :::

            [Parameters:]{.paramLabel}
            :   `exception` - an exception associated with the warning
                being logged
            :   `format` - a format string compatible with
                String.format()
            :   `args` - arguments for the format string

        []{#info(java.lang.String,java.lang.Object...)}

        -   #### info

            ``` methodSignature
            public void info​(String format,
                             Object... args)
            ```

            ::: block
            Logs a message at INFO level.
            :::

            [Parameters:]{.paramLabel}
            :   `format` - a format string compatible with
                String.format()
            :   `args` - arguments for the format string

        []{#warn(java.lang.Throwable,java.lang.String)}

        -   #### warn

            ``` methodSignature
            public void warn​(Throwable exception,
                             String message)
            ```

            ::: block
            Logs a message at WARN level.
            :::

            [Parameters:]{.paramLabel}
            :   `exception` - an exception associated with the warning
                being logged
            :   `message` - a literal message to log

        []{#warn(java.lang.String)}

        -   #### warn

            ``` methodSignature
            public void warn​(String message)
            ```

            ::: block
            Logs a message at WARN level.
            :::

            [Parameters:]{.paramLabel}
            :   `message` - a literal message to log

        []{#warn(java.lang.Throwable,java.lang.String,java.lang.Object...)}

        -   #### warn

            ``` methodSignature
            public void warn​(@Nullable
                             Throwable exception,
                             String format,
                             Object... args)
            ```

            ::: block
            Logs a message at WARN level.\
            Usage example:
                    logger.warn(e, "something bad happened when connecting to %s:%d", host, port);
                 

            If the format string is invalid or the arguments are
            insufficient, an error will be logged and execution will
            continue.
            :::

            [Parameters:]{.paramLabel}
            :   `exception` - an exception associated with the warning
                being logged
            :   `format` - a format string compatible with
                String.format()
            :   `args` - arguments for the format string

        []{#warn(java.lang.String,java.lang.Object...)}

        -   #### warn

            ``` methodSignature
            public void warn​(String format,
                             Object... args)
            ```

            ::: block
            Logs a message at WARN level.\
            Usage example:
                    logger.warn("something bad happened when connecting to %s:%d", host, port);
                 

            If the format string is invalid or the arguments are
            insufficient, an error will be logged and execution will
            continue.
            :::

            [Parameters:]{.paramLabel}
            :   `format` - a format string compatible with
                String.format()
            :   `args` - arguments for the format string

        []{#error(java.lang.Throwable,java.lang.String)}

        -   #### error

            ``` methodSignature
            public void error​(Throwable exception,
                              String message)
            ```

            ::: block
            Logs a message at ERROR level.
            :::

            [Parameters:]{.paramLabel}
            :   `exception` - an exception associated with the error
                being logged
            :   `message` - a literal message to log

        []{#error(java.lang.String)}

        -   #### error

            ``` methodSignature
            public void error​(String message)
            ```

            ::: block
            Logs a message at ERROR level.
            :::

            [Parameters:]{.paramLabel}
            :   `message` - a literal message to log

        []{#error(java.lang.Throwable,java.lang.String,java.lang.Object...)}

        -   #### error

            ``` methodSignature
            public void error​(@Nullable
                              Throwable exception,
                              String format,
                              Object... args)
            ```

            ::: block
            Logs a message at ERROR level.\
            Usage example:
                    logger.error(e, "something really bad happened when connecting to %s:%d", host, port);
                 

            If the format string is invalid or the arguments are
            insufficient, an error will be logged and execution will
            continue.
            :::

            [Parameters:]{.paramLabel}
            :   `exception` - an exception associated with the error
                being logged
            :   `format` - a format string compatible with
                String.format()
            :   `args` - arguments for the format string

        []{#error(java.lang.Throwable)}

        -   #### error

            ``` methodSignature
            public void error​(Throwable exception)
            ```

            ::: block
            Logs a message at ERROR level. The value of
            `exception.getMessage()` will be used as the log message.\
            Usage example:
                    logger.error(e);
                 
            :::

            [Parameters:]{.paramLabel}
            :   `exception` - an exception associated with the error
                being logged

        []{#error(java.lang.String,java.lang.Object...)}

        -   #### error

            ``` methodSignature
            public void error​(String format,
                              Object... args)
            ```

            ::: block
            Logs a message at ERROR level.\
            Usage example:
                    logger.error("something really bad happened when connecting to %s:%d", host, port);
                 

            If the format string is invalid or the arguments are
            insufficient, an error will be logged and execution will
            continue.
            :::

            [Parameters:]{.paramLabel}
            :   `format` - a format string compatible with
                String.format()
            :   `args` - arguments for the format string

        []{#isVerboseEnabled()}

        -   #### isVerboseEnabled

            ``` methodSignature
            public boolean isVerboseEnabled()
            ```

        []{#isDebugEnabled()}

        -   #### isDebugEnabled

            ``` methodSignature
            public boolean isDebugEnabled()
            ```

        []{#getLevel()}

        -   #### getLevel

            ``` methodSignature
            public Level getLevel()
            ```

        []{#setLevel(java.util.logging.Level)}

        -   #### setLevel

            ``` methodSignature
            public void setLevel​(Level newLevel)
            ```

        []{#isLoggable(java.util.logging.Level)}

        -   #### isLoggable

            ``` methodSignature
            public boolean isLoggable​(Level level)
            ```

        []{#addHandler(java.util.logging.Handler)}

        -   #### addHandler

            ``` methodSignature
            public void addHandler​(Handler handler)
            ```

        []{#getHandlers()}

        -   #### getHandlers

            ``` methodSignature
            public Handler[] getHandlers()
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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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

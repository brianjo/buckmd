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
[Package]{.packageLabelInType} [com.facebook.buck.log](package-summary.html)
:::

## Class LogConfig {#class-logconfig .title title="Class LogConfig"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.log.LogConfig

::: description
-   

    ------------------------------------------------------------------------

        public class LogConfig
        extends Object

    ::: block
    Constructed by java.util.logging.LogManager via the system property
    java.util.logging.LogManager.config.
    Extends LogManager\'s support for a single logging.properties file
    to support a three-level config. Each existent property file is
    concatenated together and used as a single LogManager configuration,
    with later entries overriding earlier ones.

    1\) \$BUCK_DIRECTORY/config/logging.properties.st 2)
    \$PROJECT_ROOT/.bucklogging.properties 3)
    \$PROJECT_ROOT/.bucklogging.local.properties
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `LogConfig()`                     | ::: block                         |
        |                                   | Default constructor, called by    |
        |                                   | LogManager.                       |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+

        : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static void`         | `flushLogs()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `se                   | ::: block             |
        |                       | tupLogging​(LogConfigS | Creates the log       |
        |                       | etup logConfigSetup)` | output directory and  |
        |                       |                       | concatenates          |
        |                       |                       | logging.properties    |
        |                       |                       | files together to     |
        |                       |                       | configure or          |
        |                       |                       | re-configure          |
        |                       |                       | LogManager.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `setUseAsyn           |                       |
        |                       | cFileLogging​(boolean  |                       |
        |                       | useAsyncFileLogging)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `shouldU              |                       |
        |                       | seAsyncFileLogging()` |                       |
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### LogConfig

                public LogConfig()
                          throws IOException

            ::: block
            Default constructor, called by LogManager.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#setUseAsyncFileLogging(boolean)}

        -   #### setUseAsyncFileLogging

            ``` methodSignature
            public static void setUseAsyncFileLogging​(boolean useAsyncFileLogging)
            ```

        []{#shouldUseAsyncFileLogging()}

        -   #### shouldUseAsyncFileLogging

            ``` methodSignature
            public static boolean shouldUseAsyncFileLogging()
            ```

        []{#setupLogging(com.facebook.buck.log.LogConfigSetup)}

        -   #### setupLogging

            ``` methodSignature
            public static void setupLogging​(LogConfigSetup logConfigSetup)
                                     throws IOException
            ```

            ::: block
            Creates the log output directory and concatenates
            logging.properties files together to configure or
            re-configure LogManager.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#flushLogs()}

        -   #### flushLogs

            ``` methodSignature
            public static void flushLogs()
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

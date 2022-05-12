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
[Package]{.packageLabelInType} [com.facebook.buck.support.cli.config](package-summary.html)
:::

## Class BuckConfigWriter {#class-buckconfigwriter .title title="Class BuckConfigWriter"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.support.cli.config.BuckConfigWriter

::: description
-   

    ------------------------------------------------------------------------

        public class BuckConfigWriter
        extends Object

    ::: block
    Simple class that writes out the
    [`BuckConfig`](../../../core/config/BuckConfig.html "class in com.facebook.buck.core.config")
    to a file for a specific invocation
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static void`         | `write                | ::: block             |
        |                       | Config​(Path rootPath, | Writes the            |
        |                       |             Invocatio | configuration out to  |
        |                       | nInfo info,           | a standard location   |
        |                       |   BuckConfig config)` | as json for a         |
        |                       |                       | specific command      |
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

        []{#writeConfig(java.nio.file.Path,com.facebook.buck.log.InvocationInfo,com.facebook.buck.core.config.BuckConfig)}

        -   #### writeConfig

            ``` methodSignature
            public static void writeConfig​(Path rootPath,
                                           InvocationInfo info,
                                           BuckConfig config)
                                    throws IOException
            ```

            ::: block
            Writes the configuration out to a standard location as json
            for a specific command
            Currently this is of the form:

                   {
                     "settings": {
                       "section": {
                         "key": "value"
                         "key2": "value2"
                       },
                       "other_section": {
                         "key3": "value3",
                         "key4": "true"
                     }
                   }
                 

            In the future, the source of each setting will be visible
            with a structure like this:
                   {
                     "settings": {
                       "section": {
                         "key": "value"
                         "key2": "value2"
                       },
                       "other_section": {
                         "key3": "value3",
                         "key4": "true"
                     },
                     "sources": {
                       "$path_to_config_file": {
                         "section": {
                           "key": "value"
                           "key2": "value2"
                         }
                       }
                     }
                   }
                 
            :::

            [Parameters:]{.paramLabel}
            :   `rootPath` - The root of the project that contains
                buck-out
            :   `info` - The invocation info. Used to find the log
                directories to write into
            :   `config` - The configuration to write to disk

            [Throws:]{.throwsLabel}
            :   `IOException` - The file could not be written to
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

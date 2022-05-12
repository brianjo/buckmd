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
[Package]{.packageLabelInType} [com.facebook.buck.support.fix](package-summary.html)
:::

## Class BuckFixSpecWriter {#class-buckfixspecwriter .title title="Class BuckFixSpecWriter"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.support.fix.BuckFixSpecWriter

::: description
-   

    ------------------------------------------------------------------------

        public class BuckFixSpecWriter
        extends Object

    ::: block
    Simple class that writes a serialized to json
    [`BuckFixSpec`](BuckFixSpec.html "class in com.facebook.buck.support.fix")
    to the log directory
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static void`         | `writeSpec​(Pat        | ::: block             |
        |                       | h fixSpecPath,        | Writes the json       |
        |                       |    BuckFixSpec spec)` | representation of the |
        |                       |                       | fix spec to be        |
        |                       |                       | consumed by the fix   |
        |                       |                       | script, it\'s usually |
        |                       |                       | information found in  |
        |                       |                       | logs too but in a     |
        |                       |                       | much easier format    |
        |                       |                       | for the script to     |
        |                       |                       | consume, plus command |
        |                       |                       | data that might be    |
        |                       |                       | captured only in      |
        |                       |                       | runtime.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Path`         | `w                    | ::: block             |
        |                       | riteSpecToLogDir​(Path | Writes the json       |
        |                       |  rootPath,            | representation of the |
        |                       |        InvocationInfo | fix spec to the logs  |
        |                       |  info,                | directory, derived    |
        |                       |    BuckFixSpec spec)` | from the rootPath and |
        |                       |                       | the InvocationInfo    |
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

        []{#writeSpecToLogDir(java.nio.file.Path,com.facebook.buck.log.InvocationInfo,com.facebook.buck.support.fix.BuckFixSpec)}

        -   #### writeSpecToLogDir

            ``` methodSignature
            public static Path writeSpecToLogDir​(Path rootPath,
                                                 InvocationInfo info,
                                                 BuckFixSpec spec)
                                          throws IOException
            ```

            ::: block
            Writes the json representation of the fix spec to the logs
            directory, derived from the rootPath and the InvocationInfo
            :::

            [Parameters:]{.paramLabel}
            :   `rootPath` - The root of the project that contains
                buck-out
            :   `info` - The invocation info. Used to find the log
                directories to write into
            :   `spec` - the spec to write to disk

            [Returns:]{.returnLabel}
            :   the path to which the spec was written to

            [Throws:]{.throwsLabel}
            :   `IOException` - The file could not be written to

        []{#writeSpec(java.nio.file.Path,com.facebook.buck.support.fix.BuckFixSpec)}

        -   #### writeSpec

            ``` methodSignature
            public static void writeSpec​(Path fixSpecPath,
                                         BuckFixSpec spec)
                                  throws IOException
            ```

            ::: block
            Writes the json representation of the fix spec to be
            consumed by the fix script, it\'s usually information found
            in logs too but in a much easier format for the script to
            consume, plus command data that might be captured only in
            runtime.
            :::

            [Parameters:]{.paramLabel}
            :   `fixSpecPath` - a path to the file where the spec is to
                be written
            :   `spec` - the spec to write to disk

            [Throws:]{.throwsLabel}
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

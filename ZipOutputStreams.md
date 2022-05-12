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
[Package]{.packageLabelInType} [com.facebook.buck.util.zip](package-summary.html)
:::

## Class ZipOutputStreams {#class-zipoutputstreams .title title="Class ZipOutputStreams"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.zip.ZipOutputStreams

::: description
-   

    ------------------------------------------------------------------------

        public class ZipOutputStreams
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                                 Description
          ------------------- ------------------------------------- -------------
          `static class `     `ZipOutputStreams.HandleDuplicates`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `pr                   | `newImpl​(O            |                       |
        | otected static Custom | utputStream out,      |                       |
        | ZipOutputStream.Impl` |    ZipOutputStreams.H |                       |
        |                       | andleDuplicates mode, |                       |
        |                       |         Clock clock)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static C             | `newJarOutputStre     |                       |
        | ustomJarOutputStream` | am​(OutputStream out)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static C             | `newJarOutpu          |                       |
        | ustomJarOutputStream` | tStream​(OutputStream  |                       |
        |                       | out,                  |                       |
        |                       |   ZipOutputStreams.Ha |                       |
        |                       | ndleDuplicates mode)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static C             | `                     |                       |
        | ustomJarOutputStream` | newJarOutputStream​(Ou |                       |
        |                       | tputStream out,       |                       |
        |                       |              ZipOutpu |                       |
        |                       | tStreams.HandleDuplic |                       |
        |                       | ates mode,            |                       |
        |                       |         Clock clock)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static C             | `newJarO              |                       |
        | ustomJarOutputStream` | utputStream​(Path jarF |                       |
        |                       | ile,                  |                       |
        |                       |   ZipOutputStreams.Ha |                       |
        |                       | ndleDuplicates mode)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static C             | `newOutputStre        | ::: block             |
        | ustomZipOutputStream` | am​(OutputStream out)` | Create a new          |
        |                       |                       | [`Custo               |
        |                       |                       | mZipOutputStream`](Cu |
        |                       |                       | stomZipOutputStream.h |
        |                       |                       | tml "class in com.fac |
        |                       |                       | ebook.buck.util.zip") |
        |                       |                       | that will by default  |
        |                       |                       | act in the same way   |
        |                       |                       | as                    |
        |                       |                       | [`ZipOutputStream`](  |
        |                       |                       | http://docs.oracle.co |
        |                       |                       | m/javase/7/docs/api/j |
        |                       |                       | ava/util/zip/ZipOutpu |
        |                       |                       | tStream.html?is-exter |
        |                       |                       | nal=true "class or in |
        |                       |                       | terface in java.util. |
        |                       |                       | zip"){.externalLink}, |
        |                       |                       | notably by throwing   |
        |                       |                       | an exception if       |
        |                       |                       | duplicate entries are |
        |                       |                       | added.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static C             | `newOu                | ::: block             |
        | ustomZipOutputStream` | tputStream​(OutputStre | Create a new          |
        |                       | am out,               | [`Custo               |
        |                       |   ZipOutputStreams.Ha | mZipOutputStream`](Cu |
        |                       | ndleDuplicates mode)` | stomZipOutputStream.h |
        |                       |                       | tml "class in com.fac |
        |                       |                       | ebook.buck.util.zip") |
        |                       |                       | that handles          |
        |                       |                       | duplicate entries in  |
        |                       |                       | the way dictated by   |
        |                       |                       | `mode`.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static C             | `newOutputStr         |                       |
        | ustomZipOutputStream` | eam​(OutputStream out, |                       |
        |                       |                 ZipOu |                       |
        |                       | tputStreams.HandleDup |                       |
        |                       | licates mode,         |                       |
        |                       |         Clock clock)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static C             | `newOutput            | ::: block             |
        | ustomZipOutputStream` | Stream​(Path zipFile)` | Create a new          |
        |                       |                       | [`Custo               |
        |                       |                       | mZipOutputStream`](Cu |
        |                       |                       | stomZipOutputStream.h |
        |                       |                       | tml "class in com.fac |
        |                       |                       | ebook.buck.util.zip") |
        |                       |                       | that outputs to the   |
        |                       |                       | given `zipFile`.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static C             | `n                    | ::: block             |
        | ustomZipOutputStream` | ewOutputStream​(Path z | Create a new          |
        |                       | ipFile,               | [`Custo               |
        |                       |   ZipOutputStreams.Ha | mZipOutputStream`](Cu |
        |                       | ndleDuplicates mode)` | stomZipOutputStream.h |
        |                       |                       | tml "class in com.fac |
        |                       |                       | ebook.buck.util.zip") |
        |                       |                       | that handles          |
        |                       |                       | duplicate entries in  |
        |                       |                       | the way dictated by   |
        |                       |                       | `mode`.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static C             | `newSimpleOutputStre  |                       |
        | ustomZipOutputStream` | am​(OutputStream out)` |                       |
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

        []{#newOutputStream(java.nio.file.Path)}

        -   #### newOutputStream

            ``` methodSignature
            public static CustomZipOutputStream newOutputStream​(Path zipFile)
                                                         throws IOException
            ```

            ::: block
            Create a new
            [`CustomZipOutputStream`](CustomZipOutputStream.html "class in com.facebook.buck.util.zip")
            that outputs to the given `zipFile`. Note that the parent
            directory of the `zipFile` must exist already. The returned
            stream will throw an exception should duplicate entries be
            added.
            :::

            [Parameters:]{.paramLabel}
            :   `zipFile` - The file to write to.

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#newOutputStream(java.io.OutputStream)}

        -   #### newOutputStream

            ``` methodSignature
            public static CustomZipOutputStream newOutputStream​(OutputStream out)
            ```

            ::: block
            Create a new
            [`CustomZipOutputStream`](CustomZipOutputStream.html "class in com.facebook.buck.util.zip")
            that will by default act in the same way as
            [`ZipOutputStream`](http://docs.oracle.com/javase/7/docs/api/java/util/zip/ZipOutputStream.html?is-external=true "class or interface in java.util.zip"){.externalLink},
            notably by throwing an exception if duplicate entries are
            added.
            :::

            [Parameters:]{.paramLabel}
            :   `out` - The output stream to write to.

        []{#newJarOutputStream(java.io.OutputStream)}

        -   #### newJarOutputStream

            ``` methodSignature
            public static CustomJarOutputStream newJarOutputStream​(OutputStream out)
            ```

        []{#newOutputStream(java.nio.file.Path,com.facebook.buck.util.zip.ZipOutputStreams.HandleDuplicates)}

        -   #### newOutputStream

            ``` methodSignature
            public static CustomZipOutputStream newOutputStream​(Path zipFile,
                                                                ZipOutputStreams.HandleDuplicates mode)
                                                         throws IOException
            ```

            ::: block
            Create a new
            [`CustomZipOutputStream`](CustomZipOutputStream.html "class in com.facebook.buck.util.zip")
            that handles duplicate entries in the way dictated by
            `mode`.
            :::

            [Parameters:]{.paramLabel}
            :   `zipFile` - The file to write to.
            :   `mode` - How to handle duplicate entries.

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#newJarOutputStream(java.nio.file.Path,com.facebook.buck.util.zip.ZipOutputStreams.HandleDuplicates)}

        -   #### newJarOutputStream

            ``` methodSignature
            public static CustomJarOutputStream newJarOutputStream​(Path jarFile,
                                                                   ZipOutputStreams.HandleDuplicates mode)
                                                            throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#newOutputStream(java.io.OutputStream,com.facebook.buck.util.zip.ZipOutputStreams.HandleDuplicates)}

        -   #### newOutputStream

            ``` methodSignature
            public static CustomZipOutputStream newOutputStream​(OutputStream out,
                                                                ZipOutputStreams.HandleDuplicates mode)
            ```

            ::: block
            Create a new
            [`CustomZipOutputStream`](CustomZipOutputStream.html "class in com.facebook.buck.util.zip")
            that handles duplicate entries in the way dictated by
            `mode`.
            :::

            [Parameters:]{.paramLabel}
            :   `out` - The output stream to write to.
            :   `mode` - How to handle duplicate entries.

        []{#newJarOutputStream(java.io.OutputStream,com.facebook.buck.util.zip.ZipOutputStreams.HandleDuplicates)}

        -   #### newJarOutputStream

            ``` methodSignature
            public static CustomJarOutputStream newJarOutputStream​(OutputStream out,
                                                                   ZipOutputStreams.HandleDuplicates mode)
            ```

        []{#newOutputStream(java.io.OutputStream,com.facebook.buck.util.zip.ZipOutputStreams.HandleDuplicates,com.facebook.buck.util.timing.Clock)}

        -   #### newOutputStream

            ``` methodSignature
            public static CustomZipOutputStream newOutputStream​(OutputStream out,
                                                                ZipOutputStreams.HandleDuplicates mode,
                                                                Clock clock)
            ```

        []{#newSimpleOutputStream(java.io.OutputStream)}

        -   #### newSimpleOutputStream

            ``` methodSignature
            public static CustomZipOutputStream newSimpleOutputStream​(OutputStream out)
            ```

        []{#newJarOutputStream(java.io.OutputStream,com.facebook.buck.util.zip.ZipOutputStreams.HandleDuplicates,com.facebook.buck.util.timing.Clock)}

        -   #### newJarOutputStream

            ``` methodSignature
            public static CustomJarOutputStream newJarOutputStream​(OutputStream out,
                                                                   ZipOutputStreams.HandleDuplicates mode,
                                                                   Clock clock)
            ```

        []{#newImpl(java.io.OutputStream,com.facebook.buck.util.zip.ZipOutputStreams.HandleDuplicates,com.facebook.buck.util.timing.Clock)}

        -   #### newImpl

            ``` methodSignature
            protected static CustomZipOutputStream.Impl newImpl​(OutputStream out,
                                                                ZipOutputStreams.HandleDuplicates mode,
                                                                Clock clock)
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

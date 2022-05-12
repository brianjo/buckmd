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
[Package]{.packageLabelInType} [com.facebook.buck.cxx.toolchain.objectfile](package-summary.html)
:::

## Class LcUuidContentsScrubber {#class-lcuuidcontentsscrubber .title title="Class LcUuidContentsScrubber"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.toolchain.objectfile.LcUuidContentsScrubber

::: description
-   

    All Implemented Interfaces:
    :   `FileContentsScrubber`, `FileScrubber`

    ------------------------------------------------------------------------

        public class LcUuidContentsScrubber
        extends Object
        implements FileContentsScrubber
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.io.file.FileScrubber}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.io.file.[FileScrubber](../../../io/file/FileScrubber.html "interface in com.facebook.buck.io.file")

            `FileScrubber.ScrubException`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                           Description
          ----------------------------------------------------- -------------
          `LcUuidContentsScrubber​(boolean scrubConcurrently)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `p                    | `resetUuidIfPresent​(M | ::: block             |
        | rotected static void` | appedByteBuffer map)` | Sets the LC_UUID to   |
        |                       |                       | all zeroes if it\'s   |
        |                       |                       | part of the Mach-O    |
        |                       |                       | file.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `scrubFi              | ::: block             |
        |                       | le​(FileChannel file)` | Override this method  |
        |                       |                       | to perform the        |
        |                       |                       | content modification. |
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(boolean)}

        -   #### LcUuidContentsScrubber

                public LcUuidContentsScrubber​(boolean scrubConcurrently)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#scrubFile(java.nio.channels.FileChannel)}

        -   #### scrubFile

            ``` methodSignature
            public void scrubFile​(FileChannel file)
                           throws IOException,
                                  FileScrubber.ScrubException
            ```

            ::: block
            [Description copied from
            interface: `FileContentsScrubber`]{.descfrmTypeLabel}
            :::

            ::: block
            Override this method to perform the content modification.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `scrubFile` in interface `FileContentsScrubber`

            [Throws:]{.throwsLabel}
            :   `IOException`
            :   `FileScrubber.ScrubException`

        []{#resetUuidIfPresent(java.nio.MappedByteBuffer)}

        -   #### resetUuidIfPresent

            ``` methodSignature
            protected static void resetUuidIfPresent​(MappedByteBuffer map)
                                              throws FileScrubber.ScrubException
            ```

            ::: block
            Sets the LC_UUID to all zeroes if it\'s part of the Mach-O
            file.
            :::

            [Throws:]{.throwsLabel}
            :   `FileScrubber.ScrubException`
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

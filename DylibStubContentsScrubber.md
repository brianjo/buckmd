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

## Class DylibStubContentsScrubber {#class-dylibstubcontentsscrubber .title title="Class DylibStubContentsScrubber"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.toolchain.objectfile.DylibStubContentsScrubber

::: description

All Implemented Interfaces:
:   `FileContentsScrubber`, `FileScrubber`

------------------------------------------------------------------------

    public class DylibStubContentsScrubber
    extends Object
    implements FileContentsScrubber

::: block
Scrubs the contents of dylib stubs, so that they\'re independent of the
contents of the source dylib. That means that if the source dylib\'s ABI
does not change, it will produce the exact same dylib stub.

The linker itself does not actually care about the symbol addresses, it
just wants to ensure any referenced symbols exist. That means we can
reset the addresses to any value we would like. Note that the symbol
addresses themselves are already invalid in the dylib stub, as the
contents (i.e., binary instructions) have been stripped by \"strip\".

Dylib stubs produced by \"strip\" are still dependent on symbol
addresses and the UUID. To make them independent, we do the following:

-   Set the UUID to the same value each time
-   Update the \_LINKEDIT segment and remove any addresses for symbols
    -   Update the exports info
    -   Update the symbol table
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

          Constructor                     Description
          ------------------------------- -------------
          `DylibStubContentsScrubber()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `scrubFi              | ::: block             |
        |                       | le​(FileChannel file)` | Override this method  |
        |                       |                       | to perform the        |
        |                       |                       | content modification. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
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

        []{#<init>()}

        -   #### DylibStubContentsScrubber

                public DylibStubContentsScrubber()
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
:::
:::

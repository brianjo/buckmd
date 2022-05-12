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
[Package]{.packageLabelInType} [com.facebook.buck.remoteexecution.util](package-summary.html)
:::

## Class OutputsCollector {#class-outputscollector .title title="Class OutputsCollector"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.remoteexecution.util.OutputsCollector

::: description
-   

    ------------------------------------------------------------------------

        public class OutputsCollector
        extends Object

    ::: block
    A simple helper to collect remote execution outputs. Given a list of
    root output files/directories, it will construct all the
    [`Protocol.OutputFile`](../interfaces/Protocol.OutputFile.html "interface in com.facebook.buck.remoteexecution.interfaces")
    and
    [`Protocol.OutputDirectory`](../interfaces/Protocol.OutputDirectory.html "interface in com.facebook.buck.remoteexecution.interfaces")
    objects for the outputs offered by the delegate. It will also
    include a set of
    [`UploadDataSupplier`](../UploadDataSupplier.html "interface in com.facebook.buck.remoteexecution")
    for all the files and serialized data structures that are needed to
    expand the outputs on the client.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `OutputsCollec        | ::: block             |
        |                       | tor.CollectedOutputs` | The collected         |
        |                       |                       | outputs-related       |
        |                       |                       | information.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `                     | ::: block             |
        |                       | OutputsCollector.File | A simple delegate     |
        |                       | systemBackedDelegate` | that returns          |
        |                       |                       | information from the  |
        |                       |                       | filesystem.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                        Description
          ---------------------------------------------------------------------------------------------------------------------------------- -------------
          `OutputsCollector​(Protocol protocol,                 com.facebook.buck.remoteexecution.util.OutputsCollector.Delegate delegate)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `OutputsCollec        | `collect              | ::: block             |
        | tor.CollectedOutputs` | ​(Set<Path> outputs,   | Returns the collected |
        |                       |       Path buildDir)` | output information.   |
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

        []{#<init>(com.facebook.buck.remoteexecution.interfaces.Protocol,com.facebook.buck.remoteexecution.util.OutputsCollector.Delegate)}

        -   #### OutputsCollector

                public OutputsCollector​(Protocol protocol,
                                        com.facebook.buck.remoteexecution.util.OutputsCollector.Delegate delegate)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#collect(java.util.Set,java.nio.file.Path)}

        -   #### collect

            ``` methodSignature
            public OutputsCollector.CollectedOutputs collect​(Set<Path> outputs,
                                                             Path buildDir)
                                                      throws IOException
            ```

            ::: block
            Returns the collected output information.
            :::

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

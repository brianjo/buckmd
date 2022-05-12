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
[Package]{.packageLabelInType} [com.facebook.buck.cli](package-summary.html)
:::

## Class ThriftOutput\<T\> {#class-thriftoutputt .title title="Class ThriftOutput"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cli.ThriftOutput\<T\>

::: description
-   

    ------------------------------------------------------------------------

        public class ThriftOutput<T>
        extends Object

    ::: block
    Class responsible for serialization of DirectedAcyclicGraph into
    Thrift output format
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `Thr                  | ::: block             |
        |                       | iftOutput.Builder<T>` | Builder class for     |
        |                       |                       | Thrift output         |
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
        | `static <T> Thr       | `builder​(DirectedAc   |                       |
        | iftOutput.Builder<T>` | yclicGraph<T> graph)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `writeOutput​(Thri     | ::: block             |
        |                       | ftProtocol thriftProt | Writes out the graph  |
        |                       | ocol,            Prin | in thrift format to   |
        |                       | tStream printStream)` | the given             |
        |                       |                       | printStream.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `writeOutput​(Prin     | ::: block             |
        |                       | tStream printStream)` | Writes out the graph  |
        |                       |                       | in thrift binary      |
        |                       |                       | format to the given   |
        |                       |                       | printStream.          |
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

        []{#builder(com.facebook.buck.core.util.graph.DirectedAcyclicGraph)}

        -   #### builder

            ``` methodSignature
            public static <T> ThriftOutput.Builder<T> builder​(DirectedAcyclicGraph<T> graph)
            ```

        []{#writeOutput(java.io.PrintStream)}

        -   #### writeOutput

            ``` methodSignature
            public void writeOutput​(PrintStream printStream)
                             throws IOException
            ```

            ::: block
            Writes out the graph in thrift binary format to the given
            printStream.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#writeOutput(com.facebook.buck.slb.ThriftProtocol,java.io.PrintStream)}

        -   #### writeOutput

            ``` methodSignature
            public void writeOutput​(ThriftProtocol thriftProtocol,
                                    PrintStream printStream)
                             throws IOException
            ```

            ::: block
            Writes out the graph in thrift format to the given
            printStream.
            :::

            [Parameters:]{.paramLabel}
            :   `thriftProtocol` - specific thrift protocol

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

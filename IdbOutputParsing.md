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
[Package]{.packageLabelInType} [com.facebook.buck.apple](package-summary.html)
:::

## Class IdbOutputParsing {#class-idboutputparsing .title title="Class IdbOutputParsing"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.IdbOutputParsing

::: description
-   

    ------------------------------------------------------------------------

        public class IdbOutputParsing
        extends Object

    ::: block
    Utility class to parse the output from `idb`.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static interface `   | `IdbOutputParsi       | ::: block             |
        |                       | ng.IdbResultCallback` | Callbacks invoked     |
        |                       |                       | with events emitted   |
        |                       |                       | by `idb`.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor            Description
          ---------------------- -------------
          `IdbOutputParsing()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static void`         | `stream               | ::: block             |
        |                       | OutputFromReader​(Read | Decodes a stream of   |
        |                       | er reader,            | JSON objects as       |
        |                       |             IdbOutput | produced by           |
        |                       | Parsing.IdbResultCall | `xctool -             |
        |                       | back resultCallback)` | reporter json-stream` |
        |                       |                       | and invokes the       |
        |                       |                       | callbacks in          |
        |                       |                       | `eventCallback` with  |
        |                       |                       | each event in the     |
        |                       |                       | stream.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `stat                 | `te                   | ::: block             |
        | ic TestResultSummary` | stResultSummaryForTes | Function that will    |
        |                       | tResult​(com.facebook. | generate a            |
        |                       | buck.apple.ImmutableI | TestResultSummary     |
        |                       | dbTestResult result)` | from the result of a  |
        |                       |                       | test printed by idb   |
        |                       |                       | (Im                   |
        |                       |                       | mutableIdbTestResult) |
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### IdbOutputParsing

                public IdbOutputParsing()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#streamOutputFromReader(java.io.Reader,com.facebook.buck.apple.IdbOutputParsing.IdbResultCallback)}

        -   #### streamOutputFromReader

            ``` methodSignature
            public static void streamOutputFromReader​(Reader reader,
                                                      IdbOutputParsing.IdbResultCallback resultCallback)
            ```

            ::: block
            Decodes a stream of JSON objects as produced by
            `xctool -reporter json-stream` and invokes the callbacks in
            `eventCallback` with each event in the stream.
            :::

        []{#testResultSummaryForTestResult(com.facebook.buck.apple.ImmutableIdbTestResult)}

        -   #### testResultSummaryForTestResult

            ``` methodSignature
            public static TestResultSummary testResultSummaryForTestResult​(com.facebook.buck.apple.ImmutableIdbTestResult result)
            ```

            ::: block
            Function that will generate a TestResultSummary from the
            result of a test printed by idb (ImmutableIdbTestResult)
            :::
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

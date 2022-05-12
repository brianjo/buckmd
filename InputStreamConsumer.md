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
[Package]{.packageLabelInType} [com.facebook.buck.util](package-summary.html)
:::

## Class InputStreamConsumer {#class-inputstreamconsumer .title title="Class InputStreamConsumer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.InputStreamConsumer

::: description
-   

    All Implemented Interfaces:
    :   `Callable<Unit>`

    ------------------------------------------------------------------------

        public final class InputStreamConsumer
        extends Object
        implements Callable<Unit>

    ::: block
    An utility to process input stream with a list of line-by-line
    consumers
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static interface `   | `InputSt              | ::: block             |
        |                       | reamConsumer.Handler` | Interface to handle a |
        |                       |                       | line of input from    |
        |                       |                       | the stream.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                  Description
          ------------------------------------------------------------------------------------------------------------ -------------
          `InputStreamConsumer​(InputStream inputStream,                    InputStreamConsumer.Handler... handlers)`    
          `InputStreamConsumer​(Reader reader,                    InputStreamConsumer.Handler... handlers)`              

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                      Method                                                                                                                                                             Description
          -------------------------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `Unit`                                 `call()`                                                                                                                                                            
          `static InputStreamConsumer.Handler`   `createAnsiHighlightingHandler​(boolean flagOutputWrittenToStream,                              PrintStream printStream,                              Ansi ansi)`    

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

        []{#<init>(java.io.InputStream,com.facebook.buck.util.InputStreamConsumer.Handler...)}

        -   #### InputStreamConsumer

                public InputStreamConsumer​(InputStream inputStream,
                                           InputStreamConsumer.Handler... handlers)

        []{#<init>(java.io.Reader,com.facebook.buck.util.InputStreamConsumer.Handler...)}

        -   #### InputStreamConsumer

                public InputStreamConsumer​(Reader reader,
                                           InputStreamConsumer.Handler... handlers)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#call()}

        -   #### call

            ``` methodSignature
            public Unit call()
                      throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `call` in interface `Callable<Unit>`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#createAnsiHighlightingHandler(boolean,java.io.PrintStream,com.facebook.buck.util.Ansi)}

        -   #### createAnsiHighlightingHandler

            ``` methodSignature
            public static InputStreamConsumer.Handler createAnsiHighlightingHandler​(boolean flagOutputWrittenToStream,
                                                                                    PrintStream printStream,
                                                                                    Ansi ansi)
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

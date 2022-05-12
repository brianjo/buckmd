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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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

## Class ProcessExecutor.Result {#class-processexecutor.result .title title="Class ProcessExecutor.Result"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.ProcessExecutor.Result

::: description
-   

    Enclosing interface:
    :   [ProcessExecutor](ProcessExecutor.html "interface in com.facebook.buck.util")

    ------------------------------------------------------------------------

        public static class ProcessExecutor.Result
        extends Object

    ::: block
    Values from the result of
    [`ProcessExecutor.launchAndExecute(ProcessExecutorParams, Set,  Optional, Optional, Optional)`](ProcessExecutor.html#launchAndExecute(com.facebook.buck.util.ProcessExecutorParams,java.util.Set,java.util.Optional,java.util.Optional,java.util.Optional)).
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                                   Field       Description
          --------------------------------------------------- ----------- -------------
          `com.google.common.collect.ImmutableList<String>`   `command`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                   Description
          ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `Result​(int exitCode,       boolean timedOut,       Optional<String> stdout,       Optional<String> stderr,       com.google.common.collect.ImmutableList<String> command)`    
          `Result​(int exitCode,       com.google.common.collect.ImmutableList<String> command)`                                                                                          
          `Result​(int exitCode,       String stdout,       String stderr,       com.google.common.collect.ImmutableList<String> command)`                                                

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                   Method                                            Description
          --------------------------------------------------- ------------------------------------------------- -------------
          `com.google.common.collect.ImmutableList<String>`   `getCommand()`                                     
          `int`                                               `getExitCode()`                                    
          `String`                                            `getMessageForResult​(String message)`              
          `String`                                            `getMessageForUnexpectedResult​(String subject)`    
          `Optional<String>`                                  `getStderr()`                                      
          `Optional<String>`                                  `getStdout()`                                      
          `boolean`                                           `isTimedOut()`                                     

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
    -   []{#field.detail}

        ### Field Detail

        []{#command}

        -   #### command

                public final com.google.common.collect.ImmutableList<String> command
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(int,boolean,java.util.Optional,java.util.Optional,com.google.common.collect.ImmutableList)}

        -   #### Result

                public Result​(int exitCode,
                              boolean timedOut,
                              Optional<String> stdout,
                              Optional<String> stderr,
                              com.google.common.collect.ImmutableList<String> command)

        []{#<init>(int,java.lang.String,java.lang.String,com.google.common.collect.ImmutableList)}

        -   #### Result

                public Result​(int exitCode,
                              String stdout,
                              String stderr,
                              com.google.common.collect.ImmutableList<String> command)

        []{#<init>(int,com.google.common.collect.ImmutableList)}

        -   #### Result

                public Result​(int exitCode,
                              com.google.common.collect.ImmutableList<String> command)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getExitCode()}

        -   #### getExitCode

            ``` methodSignature
            public int getExitCode()
            ```

        []{#isTimedOut()}

        -   #### isTimedOut

            ``` methodSignature
            public boolean isTimedOut()
            ```

        []{#getStdout()}

        -   #### getStdout

            ``` methodSignature
            public Optional<String> getStdout()
            ```

        []{#getStderr()}

        -   #### getStderr

            ``` methodSignature
            public Optional<String> getStderr()
            ```

        []{#getCommand()}

        -   #### getCommand

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getCommand()
            ```

        []{#getMessageForUnexpectedResult(java.lang.String)}

        -   #### getMessageForUnexpectedResult

            ``` methodSignature
            public String getMessageForUnexpectedResult​(String subject)
            ```

        []{#getMessageForResult(java.lang.String)}

        -   #### getMessageForResult

            ``` methodSignature
            public String getMessageForResult​(String message)
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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

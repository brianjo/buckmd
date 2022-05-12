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
-   [Field](#field.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.rules.macros](package-summary.html)
:::

## Class WorkerMacroArg {#class-workermacroarg .title title="Class WorkerMacroArg"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.rules.args.ProxyArg](../args/ProxyArg.html "class in com.facebook.buck.rules.args")

    -   -   com.facebook.buck.rules.macros.WorkerMacroArg

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`, `Arg`

    ------------------------------------------------------------------------

        public class WorkerMacroArg
        extends ProxyArg

    ::: block
    Worker macro wrapper which extracts/verifies details from the an
    underlying
    [`WorkerTool`](../../shell/WorkerTool.html "interface in com.facebook.buck.shell").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.rules.args.ProxyArg}

            ### Fields inherited from class com.facebook.buck.rules.args.[ProxyArg](../args/ProxyArg.html "class in com.facebook.buck.rules.args")

            `arg`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                         Method                                                                                                                                                                     Description
          --------------------------------------------------------- -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `static WorkerMacroArg`                                   `fromStringWithMacros​(Arg arg,                     BuildTarget target,                     BuildRuleResolver resolver,                     StringWithMacros unexpanded)`    
          `com.google.common.collect.ImmutableMap<String,​String>`   `getEnvironment()`                                                                                                                                                          
          `String`                                                  `getJobArgs​(SourcePathResolverAdapter pathResolver)`                                                                                                                        
          `int`                                                     `getMaxWorkers()`                                                                                                                                                           
          `Optional<String>`                                        `getPersistentWorkerKey()`                                                                                                                                                  
          `com.google.common.collect.ImmutableList<String>`         `getStartupCommand()`                                                                                                                                                       
          `Path`                                                    `getTempDir()`                                                                                                                                                              
          `com.google.common.hash.HashCode`                         `getWorkerHash()`                                                                                                                                                           
          `boolean`                                                 `isAsync()`                                                                                                                                                                 

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.rules.args.ProxyArg}

            ### Methods inherited from class com.facebook.buck.rules.args.[ProxyArg](../args/ProxyArg.html "class in com.facebook.buck.rules.args")

            `appendToCommandLine, equals, hashCode, toString`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.rules.args.Arg}

            ### Methods inherited from interface com.facebook.buck.rules.args.[Arg](../args/Arg.html "interface in com.facebook.buck.rules.args")

            `singleCommandLineArg`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#fromStringWithMacros(com.facebook.buck.rules.args.Arg,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.BuildRuleResolver,com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### fromStringWithMacros

            ``` methodSignature
            public static WorkerMacroArg fromStringWithMacros​(Arg arg,
                                                              BuildTarget target,
                                                              BuildRuleResolver resolver,
                                                              StringWithMacros unexpanded)
            ```

            [Returns:]{.returnLabel}
            :   a
                [`WorkerMacroArg`](WorkerMacroArg.html "class in com.facebook.buck.rules.macros")
                which wraps the given
                [`StringWithMacros`](StringWithMacros.html "class in com.facebook.buck.rules.macros").

        []{#getStartupCommand()}

        -   #### getStartupCommand

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getStartupCommand()
            ```

        []{#getEnvironment()}

        -   #### getEnvironment

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​String> getEnvironment()
            ```

        []{#getTempDir()}

        -   #### getTempDir

            ``` methodSignature
            public Path getTempDir()
            ```

        []{#getPersistentWorkerKey()}

        -   #### getPersistentWorkerKey

            ``` methodSignature
            public Optional<String> getPersistentWorkerKey()
            ```

        []{#getWorkerHash()}

        -   #### getWorkerHash

            ``` methodSignature
            public com.google.common.hash.HashCode getWorkerHash()
            ```

        []{#getMaxWorkers()}

        -   #### getMaxWorkers

            ``` methodSignature
            public int getMaxWorkers()
            ```

        []{#isAsync()}

        -   #### isAsync

            ``` methodSignature
            public boolean isAsync()
            ```

        []{#getJobArgs(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### getJobArgs

            ``` methodSignature
            public String getJobArgs​(SourcePathResolverAdapter pathResolver)
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
-   Nested \| 
-   [Field](#field.summary) \| 
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

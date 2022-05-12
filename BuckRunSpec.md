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
[Package]{.packageLabelInType} [com.facebook.buck.support.fix](package-summary.html)
:::

## Class BuckRunSpec {#class-buckrunspec .title title="Class BuckRunSpec"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.support.fix.BuckRunSpec

::: description
-   

    ------------------------------------------------------------------------

        public abstract class BuckRunSpec
        extends Object

    ::: block
    Holds information to tell the python wrapper whether to run anything
    after executing the current command, and how to do it
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor       Description
          ----------------- -------------
          `BuckRunSpec()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `abstract com.go      | `getArgv()`           | ::: block             |
        | ogle.common.collect.I |                       | The arguments to      |
        | mmutableList<String>` |                       | invoke the command.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Path`       | `getCwd()`            | ::: block             |
        |                       |                       | The PWD where the     |
        |                       |                       | command should be run |
        |                       |                       | from                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getEnvp()`           | ::: block             |
        | abstract com.google.c |                       | A mapping of          |
        | ommon.collect.Immutab |                       | environment variables |
        | leMap<String,​String>` |                       | that should be set    |
        |                       |                       | when invoking the     |
        |                       |                       | command               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract boolean`    | `getIsFixScript()`    | ::: block             |
        |                       |                       | Whether the program   |
        |                       |                       | is a \'fix\' script   |
        |                       |                       | or not                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getPath()`           | ::: block             |
        |                       |                       | The path to the       |
        |                       |                       | binary to invoke      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static BuckRunSpec`  | `of​(com.              |                       |
        |                       | google.common.collect |                       |
        |                       | .ImmutableList<String |                       |
        |                       | > argv,   com.google. |                       |
        |                       | common.collect.Immuta |                       |
        |                       | bleMap<String,​String> |                       |
        |                       |  envp,   Path cwd,    |                       |
        |                       | boolean isFixScript)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
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

        -   #### BuckRunSpec

                public BuckRunSpec()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getPath()}

        -   #### getPath

            ``` methodSignature
            @Derived
            public Path getPath()
            ```

            ::: block
            The path to the binary to invoke
            :::

        []{#getArgv()}

        -   #### getArgv

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<String> getArgv()
            ```

            ::: block
            The arguments to invoke the command. The first element must
            be the binary to invoke
            :::

        []{#getEnvp()}

        -   #### getEnvp

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableMap<String,​String> getEnvp()
            ```

            ::: block
            A mapping of environment variables that should be set when
            invoking the command
            :::

        []{#getCwd()}

        -   #### getCwd

            ``` methodSignature
            public abstract Path getCwd()
            ```

            ::: block
            The PWD where the command should be run from
            :::

        []{#getIsFixScript()}

        -   #### getIsFixScript

            ``` methodSignature
            public abstract boolean getIsFixScript()
            ```

            ::: block
            Whether the program is a \'fix\' script or not
            This can affect things like signal handling, exit codes and
            how the program is actually executed in the wrapper
            :::

        []{#of(com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableMap,java.nio.file.Path,boolean)}

        -   #### of

            ``` methodSignature
            public static BuckRunSpec of​(com.google.common.collect.ImmutableList<String> argv,
                                         com.google.common.collect.ImmutableMap<String,​String> envp,
                                         Path cwd,
                                         boolean isFixScript)
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

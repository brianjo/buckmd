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
[Package]{.packageLabelInType} [com.facebook.buck.sandbox.darwin](package-summary.html)
:::

## Class DarwinSandbox {#class-darwinsandbox .title title="Class DarwinSandbox"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.sandbox.darwin.DarwinSandbox

::: description
-   

    ------------------------------------------------------------------------

        public class DarwinSandbox
        extends Object

    ::: block
    Provides an interface to OS X native sandbox capabilities.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                            Description
          ------------------------------------------------------ -------------
          `DarwinSandbox​(SandboxProperties sandboxProperties)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.go               | `createCo             | ::: block             |
        | ogle.common.collect.I | mmandLineArguments()` | Creates a list CL     |
        | mmutableList<String>` |                       | arguments that should |
        |                       |                       | be used to run a      |
        |                       |                       | process in this       |
        |                       |                       | sandbox               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `c                    | ::: block             |
        | ogle.common.collect.I | reateCommandLineArgum | Creates a list CL     |
        | mmutableList<String>` | entsForDescription()` | arguments that should |
        |                       |                       | be used to run a      |
        |                       |                       | process in this       |
        |                       |                       | sandbox               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static com.go        | `createVerificationCo | ::: block             |
        | ogle.common.collect.I | mmandLineArguments()` | Creates a list of CL  |
        | mmutableList<String>` |                       | arguments to run a    |
        |                       |                       | sandbox to verify     |
        |                       |                       | that sandbox is       |
        |                       |                       | functioning           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `init​(Proj            | ::: block             |
        |                       | ectFilesystem project | Performs              |
        |                       | Filesystem,     Sandb | initialization        |
        |                       | oxProperties addition | required by a sandbox |
        |                       | alSandboxProperties)` | :::                   |
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

        []{#<init>(com.facebook.buck.sandbox.SandboxProperties)}

        -   #### DarwinSandbox

                public DarwinSandbox​(SandboxProperties sandboxProperties)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#createVerificationCommandLineArguments()}

        -   #### createVerificationCommandLineArguments

            ``` methodSignature
            public static com.google.common.collect.ImmutableList<String> createVerificationCommandLineArguments()
            ```

            ::: block
            Creates a list of CL arguments to run a sandbox to verify
            that sandbox is functioning
            :::

        []{#createCommandLineArguments()}

        -   #### createCommandLineArguments

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> createCommandLineArguments()
            ```

            ::: block
            Creates a list CL arguments that should be used to run a
            process in this sandbox
            :::

        []{#createCommandLineArgumentsForDescription()}

        -   #### createCommandLineArgumentsForDescription

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> createCommandLineArgumentsForDescription()
            ```

            ::: block
            Creates a list CL arguments that should be used to run a
            process in this sandbox
            :::

        []{#init(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.sandbox.SandboxProperties)}

        -   #### init

            ``` methodSignature
            public void init​(ProjectFilesystem projectFilesystem,
                             SandboxProperties additionalSandboxProperties)
                      throws IOException
            ```

            ::: block
            Performs initialization required by a sandbox
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

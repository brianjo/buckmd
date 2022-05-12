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
[Package]{.packageLabelInType} [com.facebook.buck.support.fix](package-summary.html)
:::

## Class BuckFixSpecParser {#class-buckfixspecparser .title title="Class BuckFixSpecParser"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.support.fix.BuckFixSpecParser

::: description
-   

    ------------------------------------------------------------------------

        public class BuckFixSpecParser
        extends Object

    ::: block
    Creates a BuckFixSpec to pass to helper scripts from matching
    [`BuildLogEntry`](../../doctor/config/BuildLogEntry.html "interface in com.facebook.buck.doctor.config")
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `BuckFixSpecP         | ::: block             |
        |                       | arser.FixSpecFailure` | The various ways that |
        |                       |                       | trying to parse a     |
        |                       |                       | FixSpec can fail      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor             Description
          ----------------------- -------------
          `BuckFixSpecParser()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static Either<Buck   | `parseFro             | ::: block             |
        | FixSpec,​BuckFixSpecPa | mBuildId​(BuildLogHelp | Tries to construct a  |
        | rser.FixSpecFailure>` | er helper,            | [`BuckFixSp           |
        |                       |       FixBuckConfig f | ec`](BuckFixSpec.html |
        |                       | ixConfig,             |  "class in com.facebo |
        |                       |      BuildId buildId, | ok.buck.support.fix") |
        |                       |                  bool | from a specific       |
        |                       | ean manuallyInvoked)` | invocation of buck    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Either<Buck   | `parseFromBuildIdWi   | ::: block             |
        | FixSpec,​BuckFixSpecPa | thExitCode​(BuildLogHe | Tries to construct a  |
        | rser.FixSpecFailure>` | lper helper,          | [`BuckFixSp           |
        |                       |                     F | ec`](BuckFixSpec.html |
        |                       | ixBuckConfig fixConfi |  "class in com.facebo |
        |                       | g,                    | ok.buck.support.fix") |
        |                       |           BuildId bui | from a specific       |
        |                       | ldId,                 | invocation of buck    |
        |                       |              ExitCode | :::                   |
        |                       |  exitCode,            |                       |
        |                       |                   boo |                       |
        |                       | lean manuallyInvoked, |                       |
        |                       |                       |                       |
        |                       |         Optional<Exce |                       |
        |                       | ption> runException)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Either<Buck   | `parseFromFixSpecFi   | ::: block             |
        | FixSpec,​BuckFixSpecPa | le​(Path fixSpecPath)` | Tries to parse a      |
        | rser.FixSpecFailure>` |                       | [`BuckFixSp           |
        |                       |                       | ec`](BuckFixSpec.html |
        |                       |                       |  "class in com.facebo |
        |                       |                       | ok.buck.support.fix") |
        |                       |                       | from a file already   |
        |                       |                       | with the information  |
        |                       |                       | of a fix spec.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Either<Buck   | `parseLastCommand​(    | ::: block             |
        | FixSpec,​BuckFixSpecPa | BuildLogHelper helper | Tries to construct a  |
        | rser.FixSpecFailure>` | ,                 Fix | [`BuckFixSp           |
        |                       | BuckConfig fixConfig, | ec`](BuckFixSpec.html |
        |                       |                  bool |  "class in com.facebo |
        |                       | ean manuallyInvoked)` | ok.buck.support.fix") |
        |                       |                       | from the newest       |
        |                       |                       | invocation of buck    |
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

        -   #### BuckFixSpecParser

                public BuckFixSpecParser()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#parseLastCommand(com.facebook.buck.doctor.BuildLogHelper,com.facebook.buck.support.fix.FixBuckConfig,boolean)}

        -   #### parseLastCommand

            ``` methodSignature
            public static Either<BuckFixSpec,​BuckFixSpecParser.FixSpecFailure> parseLastCommand​(BuildLogHelper helper,
                                                                                                      FixBuckConfig fixConfig,
                                                                                                      boolean manuallyInvoked)
                                                                                               throws IOException
            ```

            ::: block
            Tries to construct a
            [`BuckFixSpec`](BuckFixSpec.html "class in com.facebook.buck.support.fix")
            from the newest invocation of buck
            This excludes commands like fix, server, doctor, etc (see
            [`BuildLogHelper`](../../doctor/BuildLogHelper.html "class in com.facebook.buck.doctor")),
            and will not return a spec if required fields were not able
            to be found in the logs (e.g. if exitCode is missing, a
            useful spec will not be able to be constructed)
            :::

            [Parameters:]{.paramLabel}
            :   `helper` - The helper used to find all build logs
            :   `fixConfig` - The configuration for this invocation of
                fix
            :   `manuallyInvoked` - Whether or not this spec will be
                used in a command that was manually invoked

            [Returns:]{.returnLabel}
            :   A
                [`BuckFixSpec`](BuckFixSpec.html "class in com.facebook.buck.support.fix")
                constructed from the build logs or an error if one could
                not be found or constructed

            [Throws:]{.throwsLabel}
            :   `IOException` - There was a problem reading the logs on
                disk

        []{#parseFromBuildId(com.facebook.buck.doctor.BuildLogHelper,com.facebook.buck.support.fix.FixBuckConfig,com.facebook.buck.core.model.BuildId,boolean)}

        -   #### parseFromBuildId

            ``` methodSignature
            public static Either<BuckFixSpec,​BuckFixSpecParser.FixSpecFailure> parseFromBuildId​(BuildLogHelper helper,
                                                                                                      FixBuckConfig fixConfig,
                                                                                                      BuildId buildId,
                                                                                                      boolean manuallyInvoked)
                                                                                               throws IOException
            ```

            ::: block
            Tries to construct a
            [`BuckFixSpec`](BuckFixSpec.html "class in com.facebook.buck.support.fix")
            from a specific invocation of buck
            A spec will not be returned if the log could not be found,
            or if required fields were not able to be found in the logs
            (e.g. if exitCode is missing, a useful spec will not be able
            to be constructed)
            :::

            [Parameters:]{.paramLabel}
            :   `helper` - The helper used to find all build logs
            :   `fixConfig` - The configuration for this invocation of
                fix
            :   `buildId` - The build id to look for
            :   `manuallyInvoked` - Whether or not this spec will be
                used in a command that was manually invoked

            [Returns:]{.returnLabel}
            :   A
                [`BuckFixSpec`](BuckFixSpec.html "class in com.facebook.buck.support.fix")
                constructed from the build logs or an error if one could
                not be found or constructed

            [Throws:]{.throwsLabel}
            :   `IOException` - There was a problem reading the logs on
                disk

        []{#parseFromBuildIdWithExitCode(com.facebook.buck.doctor.BuildLogHelper,com.facebook.buck.support.fix.FixBuckConfig,com.facebook.buck.core.model.BuildId,com.facebook.buck.util.ExitCode,boolean,java.util.Optional)}

        -   #### parseFromBuildIdWithExitCode

            ``` methodSignature
            public static Either<BuckFixSpec,​BuckFixSpecParser.FixSpecFailure> parseFromBuildIdWithExitCode​(BuildLogHelper helper,
                                                                                                                  FixBuckConfig fixConfig,
                                                                                                                  BuildId buildId,
                                                                                                                  ExitCode exitCode,
                                                                                                                  boolean manuallyInvoked,
                                                                                                                  Optional<Exception> runException)
                                                                                                           throws IOException
            ```

            ::: block
            Tries to construct a
            [`BuckFixSpec`](BuckFixSpec.html "class in com.facebook.buck.support.fix")
            from a specific invocation of buck
            A spec will not be returned if the log could not be found,
            or if required fields were not able to be found in the logs
            (e.g. if command args are missing, a useful spec will not be
            able to be constructed)

            Exit code is passed in, as there may not be enough
            information in the log yet (if this is called before the
            command has terminated) to otherwise construct a valid spec
            :::

            [Parameters:]{.paramLabel}
            :   `helper` - The helper used to find all build logs
            :   `fixConfig` - The configuration for this invocation of
                fix
            :   `buildId` - The build id to look for
            :   `exitCode` - The exit code for the command
            :   `manuallyInvoked` - Whether or not this spec will be
                used in a command that was manually invoked

            [Returns:]{.returnLabel}
            :   A
                [`BuckFixSpec`](BuckFixSpec.html "class in com.facebook.buck.support.fix")
                constructed from the build logs

            [Throws:]{.throwsLabel}
            :   `IOException` - There was a problem reading the logs on
                disk

        []{#parseFromFixSpecFile(java.nio.file.Path)}

        -   #### parseFromFixSpecFile

            ``` methodSignature
            public static Either<BuckFixSpec,​BuckFixSpecParser.FixSpecFailure> parseFromFixSpecFile​(Path fixSpecPath)
                                                                                                   throws IOException
            ```

            ::: block
            Tries to parse a
            [`BuckFixSpec`](BuckFixSpec.html "class in com.facebook.buck.support.fix")
            from a file already with the information of a fix spec. This
            differs from other parse\... methods in that it doesn\'t try
            to construct a fix spec from various different log files,
            only from a single spec file.
            :::

            [Parameters:]{.paramLabel}
            :   `fixSpecPath` - the absolute path to the fix spec file

            [Returns:]{.returnLabel}
            :   Either a
                [`BuckFixSpec`](BuckFixSpec.html "class in com.facebook.buck.support.fix")
                or a Failure if the spec file is missing in the given
                path

            [Throws:]{.throwsLabel}
            :   `IOException` - for any other error in the process of
                reading the file
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

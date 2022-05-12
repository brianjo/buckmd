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
[Package]{.packageLabelInType} [com.facebook.buck.doctor](package-summary.html)
:::

## Class BuildLogHelper {#class-buildloghelper .title title="Class BuildLogHelper"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.doctor.BuildLogHelper

::: description
-   

    ------------------------------------------------------------------------

        public class BuildLogHelper
        extends Object

    ::: block
    Methods for finding and inspecting buck log files.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                             Description
          ------------------------------------------------------- -------------
          `BuildLogHelper​(ProjectFilesystem projectFilesystem)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Opt                  | `getBuildLogEntryFro  | ::: block             |
        | ional<BuildLogEntry>` | mId​(BuildId buildId)` | Given a build id,     |
        |                       |                       | return the            |
        |                       |                       | corresponding         |
        |                       |                       | [`Build               |
        |                       |                       | LogEntry`](config/Bui |
        |                       |                       | ldLogEntry.html "inte |
        |                       |                       | rface in com.facebook |
        |                       |                       | .buck.doctor.config") |
        |                       |                       | of that build         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.co        | `getBuildLogs()`      |                       |
        | mmon.collect.Immutabl |                       |                       |
        | eList<BuildLogEntry>` |                       |                       |
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

        []{#<init>(com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### BuildLogHelper

                public BuildLogHelper​(ProjectFilesystem projectFilesystem)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBuildLogs()}

        -   #### getBuildLogs

            ``` methodSignature
            public com.google.common.collect.ImmutableList<BuildLogEntry> getBuildLogs()
                                                                                throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getBuildLogEntryFromId(com.facebook.buck.core.model.BuildId)}

        -   #### getBuildLogEntryFromId

            ``` methodSignature
            public Optional<BuildLogEntry> getBuildLogEntryFromId​(BuildId buildId)
                                                           throws IOException
            ```

            ::: block
            Given a build id, return the corresponding
            [`BuildLogEntry`](config/BuildLogEntry.html "interface in com.facebook.buck.doctor.config")
            of that build
            :::

            [Parameters:]{.paramLabel}
            :   `buildId` - the buildId corresponding to the
                [`BuildLogEntry`](config/BuildLogEntry.html "interface in com.facebook.buck.doctor.config")
                to retrieve

            [Returns:]{.returnLabel}
            :   An optional BuildLogEntry

            [Throws:]{.throwsLabel}
            :   `IOException` - If interacting with the filesystem fails
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

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
[Package]{.packageLabelInType} [com.facebook.buck.util.versioncontrol](package-summary.html)
:::

## Class DelegatingVersionControlCmdLineInterface {#class-delegatingversioncontrolcmdlineinterface .title title="Class DelegatingVersionControlCmdLineInterface"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.versioncontrol.DelegatingVersionControlCmdLineInterface

::: description
-   

    All Implemented Interfaces:
    :   `VersionControlCmdLineInterface`

    ------------------------------------------------------------------------

        public class DelegatingVersionControlCmdLineInterface
        extends Object
        implements VersionControlCmdLineInterface
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                            Description
          ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `DelegatingVersionControlCmdLineInterface​(Path projectRoot,                                         ProcessExecutorFactory processExecutorFactory,                                         String hgCmd,                                         com.google.common.collect.ImmutableMap<String,​String> environment)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                 Method                                                                                Description
          ----------------------------------------------------------------- ------------------------------------------------------------------------------------- -------------
          `com.google.common.collect.ImmutableSet<String>`                  `changedFiles​(String fromRevisionId)`                                                  
          `Optional<VersionControlSupplier<InputStream>>`                   `diffBetweenRevisions​(String baseRevision,                     String tipRevision)`    
          `com.facebook.buck.util.versioncontrol.FastVersionControlStats`   `fastVersionControlStats()`                                                            
          `boolean`                                                         `isSupportedVersionControlSystem()`                                                    

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

        []{#<init>(java.nio.file.Path,com.facebook.buck.util.ProcessExecutorFactory,java.lang.String,com.google.common.collect.ImmutableMap)}

        -   #### DelegatingVersionControlCmdLineInterface

                public DelegatingVersionControlCmdLineInterface​(Path projectRoot,
                                                                ProcessExecutorFactory processExecutorFactory,
                                                                String hgCmd,
                                                                com.google.common.collect.ImmutableMap<String,​String> environment)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#isSupportedVersionControlSystem()}

        -   #### isSupportedVersionControlSystem

            ``` methodSignature
            public boolean isSupportedVersionControlSystem()
                                                    throws InterruptedException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isSupportedVersionControlSystem` in
                interface `VersionControlCmdLineInterface`

            [Returns:]{.returnLabel}
            :   true if project is using version control, and we support
                it (i.e. hg)

            [Throws:]{.throwsLabel}
            :   `InterruptedException`

        []{#diffBetweenRevisions(java.lang.String,java.lang.String)}

        -   #### diffBetweenRevisions

            ``` methodSignature
            public Optional<VersionControlSupplier<InputStream>> diffBetweenRevisions​(String baseRevision,
                                                                                      String tipRevision)
                                                                               throws VersionControlCommandFailedException,
                                                                                      InterruptedException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `diffBetweenRevisions` in
                interface `VersionControlCmdLineInterface`

            [Returns:]{.returnLabel}
            :   [`VersionControlSupplier`](VersionControlSupplier.html "interface in com.facebook.buck.util.versioncontrol")
                of the input stream of the diff between two revisions or
                [`Optional.empty()`](http://docs.oracle.com/javase/7/docs/api/java/util/Optional.html?is-external=true#empty() "class or interface in java.util"){.externalLink}

            [Throws:]{.throwsLabel}
            :   `VersionControlCommandFailedException`
            :   `InterruptedException`

        []{#changedFiles(java.lang.String)}

        -   #### changedFiles

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<String> changedFiles​(String fromRevisionId)
                                                                        throws VersionControlCommandFailedException,
                                                                               InterruptedException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `changedFiles` in
                interface `VersionControlCmdLineInterface`

            [Returns:]{.returnLabel}
            :   files changed from the given revision.

            [Throws:]{.throwsLabel}
            :   `VersionControlCommandFailedException`
            :   `InterruptedException`

        []{#fastVersionControlStats()}

        -   #### fastVersionControlStats

            ``` methodSignature
            public com.facebook.buck.util.versioncontrol.FastVersionControlStats fastVersionControlStats()
                                                                                                  throws InterruptedException,
                                                                                                         VersionControlCommandFailedException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `fastVersionControlStats` in
                interface `VersionControlCmdLineInterface`

            [Throws:]{.throwsLabel}
            :   `InterruptedException`
            :   `VersionControlCommandFailedException`
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

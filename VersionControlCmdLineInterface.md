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
[Package]{.packageLabelInType} [com.facebook.buck.util.versioncontrol](package-summary.html)
:::

## Interface VersionControlCmdLineInterface {#interface-versioncontrolcmdlineinterface .title title="Interface VersionControlCmdLineInterface"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `DelegatingVersionControlCmdLineInterface`,
        `HgCmdLineInterface`, `NoOpCmdLineInterface`

    ------------------------------------------------------------------------

        public interface VersionControlCmdLineInterface

    ::: block
    Provides meta-data about the version control repository the project
    being built is using.
    :::
:::

::: summary
-   ::: {.section role="region"}
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
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#isSupportedVersionControlSystem()}

        -   #### isSupportedVersionControlSystem

            ``` methodSignature
            boolean isSupportedVersionControlSystem()
                                             throws InterruptedException
            ```

            [Returns:]{.returnLabel}
            :   true if project is using version control, and we support
                it (i.e. hg)

            [Throws:]{.throwsLabel}
            :   `InterruptedException`

        []{#diffBetweenRevisions(java.lang.String,java.lang.String)}

        -   #### diffBetweenRevisions

            ``` methodSignature
            Optional<VersionControlSupplier<InputStream>> diffBetweenRevisions​(String baseRevision,
                                                                               String tipRevision)
                                                                        throws VersionControlCommandFailedException,
                                                                               InterruptedException
            ```

            [Parameters:]{.paramLabel}
            :   `baseRevision` -
            :   `tipRevision` -

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
            com.google.common.collect.ImmutableSet<String> changedFiles​(String fromRevisionId)
                                                                 throws VersionControlCommandFailedException,
                                                                        InterruptedException
            ```

            [Parameters:]{.paramLabel}
            :   `fromRevisionId` -

            [Returns:]{.returnLabel}
            :   files changed from the given revision.

            [Throws:]{.throwsLabel}
            :   `VersionControlCommandFailedException`
            :   `InterruptedException`

        []{#fastVersionControlStats()}

        -   #### fastVersionControlStats

            ``` methodSignature
            com.facebook.buck.util.versioncontrol.FastVersionControlStats fastVersionControlStats()
                                                                                           throws InterruptedException,
                                                                                                  VersionControlCommandFailedException
            ```

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

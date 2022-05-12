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
[Package]{.packageLabelInType} [com.facebook.buck.doctor.config](package-summary.html)
:::

## Interface SourceControlInfo {#interface-sourcecontrolinfo .title title="Interface SourceControlInfo"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        public interface SourceControlInfo
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                  Method                                                                                                                                                                                                                                                                                                            Description
          -------------------------------------------------- ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `com.google.common.collect.ImmutableSet<String>`   `getBasedOffWhichTracked()`                                                                                                                                                                                                                                                                                        
          `String`                                           `getCurrentRevisionId()`                                                                                                                                                                                                                                                                                           
          `Optional<VersionControlSupplier<InputStream>>`    `getDiff()`                                                                                                                                                                                                                                                                                                        
          `com.google.common.collect.ImmutableSet<String>`   `getDirtyFiles()`                                                                                                                                                                                                                                                                                                  
          `Optional<String>`                                 `getRevisionIdOffTracked()`                                                                                                                                                                                                                                                                                        
          `Optional<Long>`                                   `getRevisionTimestampOffTracked()`                                                                                                                                                                                                                                                                                 
          `static SourceControlInfo`                         `of​(String currentRevisionId,   com.google.common.collect.ImmutableSet<String> basedOffWhichTracked,   Optional<String> revisionIdOffTracked,   Optional<Long> revisionTimestampOffTracked,   Optional<VersionControlSupplier<InputStream>> diff,   com.google.common.collect.ImmutableSet<String> dirtyFiles)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getCurrentRevisionId()}

        -   #### getCurrentRevisionId

            ``` methodSignature
            String getCurrentRevisionId()
            ```

        []{#getBasedOffWhichTracked()}

        -   #### getBasedOffWhichTracked

            ``` methodSignature
            com.google.common.collect.ImmutableSet<String> getBasedOffWhichTracked()
            ```

        []{#getRevisionIdOffTracked()}

        -   #### getRevisionIdOffTracked

            ``` methodSignature
            Optional<String> getRevisionIdOffTracked()
            ```

        []{#getRevisionTimestampOffTracked()}

        -   #### getRevisionTimestampOffTracked

            ``` methodSignature
            Optional<Long> getRevisionTimestampOffTracked()
            ```

        []{#getDiff()}

        -   #### getDiff

            ``` methodSignature
            Optional<VersionControlSupplier<InputStream>> getDiff()
            ```

        []{#getDirtyFiles()}

        -   #### getDirtyFiles

            ``` methodSignature
            com.google.common.collect.ImmutableSet<String> getDirtyFiles()
            ```

        []{#of(java.lang.String,com.google.common.collect.ImmutableSet,java.util.Optional,java.util.Optional,java.util.Optional,com.google.common.collect.ImmutableSet)}

        -   #### of

            ``` methodSignature
            static SourceControlInfo of​(String currentRevisionId,
                                        com.google.common.collect.ImmutableSet<String> basedOffWhichTracked,
                                        Optional<String> revisionIdOffTracked,
                                        Optional<Long> revisionTimestampOffTracked,
                                        Optional<VersionControlSupplier<InputStream>> diff,
                                        com.google.common.collect.ImmutableSet<String> dirtyFiles)
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

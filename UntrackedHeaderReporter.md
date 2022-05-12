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
[Package]{.packageLabelInType} [com.facebook.buck.cxx](package-summary.html)
:::

## Interface UntrackedHeaderReporter {#interface-untrackedheaderreporter .title title="Interface UntrackedHeaderReporter"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        public interface UntrackedHeaderReporter

    ::: block
    Produces the error message when an untracked header is detected.
    When preprocessing/compiling, we may encounter some headers that are
    missing from BUCK file. If the file is not whitelisted classes
    implementing this interface generate the message for this error.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                Description
          ------------------- ------------------------------------------------------------------------------------- -------------
          `String`            `getErrorReport​(SourcePathResolverAdapter pathResolver,               Path header)`    
          `boolean`           `isDetailed()`                                                                         

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

        []{#isDetailed()}

        -   #### isDetailed

            ``` methodSignature
            boolean isDetailed()
            ```

        []{#getErrorReport(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,java.nio.file.Path)}

        -   #### getErrorReport

            ``` methodSignature
            String getErrorReport​(SourcePathResolverAdapter pathResolver,
                                  Path header)
                           throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `Exception` - in case there is some error while
                generating the report. Some reporters access the disk,
                which can fail.
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

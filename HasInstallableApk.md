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
-   [Nested](#nested.class.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.android](package-summary.html)
:::

## Interface HasInstallableApk {#interface-hasinstallableapk .title title="Interface HasInstallableApk"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `AndroidBinary`, `AndroidBundle`, `AndroidInstrumentationApk`,
        `ApkGenrule`

    ------------------------------------------------------------------------

        public interface HasInstallableApk

    ::: block
    Build rule that generates an APK that can be installed with the
    install command.
    :::

    [See Also:]{.seeLabel}
    :   [`InstallCommand`](../cli/InstallCommand.html "class in com.facebook.buck.cli")
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Interface                     Description
          ------------------- ----------------------------- -------------
          `static class `     `HasInstallableApk.ApkInfo`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type             Method                     Description
          ----------------------------- -------------------------- -------------
          `HasInstallableApk.ApkInfo`   `getApkInfo()`              
          `BuildTarget`                 `getBuildTarget()`          
          `ProjectFilesystem`           `getProjectFilesystem()`    

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

        []{#getApkInfo()}

        -   #### getApkInfo

            ``` methodSignature
            HasInstallableApk.ApkInfo getApkInfo()
            ```

        []{#getBuildTarget()}

        -   #### getBuildTarget

            ``` methodSignature
            BuildTarget getBuildTarget()
            ```

        []{#getProjectFilesystem()}

        -   #### getProjectFilesystem

            ``` methodSignature
            ProjectFilesystem getProjectFilesystem()
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
-   [Nested](#nested.class.summary) \| 
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

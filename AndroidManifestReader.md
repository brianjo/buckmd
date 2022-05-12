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
[Package]{.packageLabelInType} [com.facebook.buck.android](package-summary.html)
:::

## Interface AndroidManifestReader {#interface-androidmanifestreader .title title="Interface AndroidManifestReader"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `DefaultAndroidManifestReader`

    ------------------------------------------------------------------------

        public interface AndroidManifestReader

    ::: block
    Allows querying an Android manifest file for various types of
    information.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                             Description
          ------------------- ---------------------------------- -------------
          `String`            `getInstrumentationTestRunner()`    
          `List<String>`      `getLauncherActivities()`           
          `String`            `getPackage()`                      
          `String`            `getTargetPackage()`                
          `String`            `getVersionCode()`                  

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

        []{#getLauncherActivities()}

        -   #### getLauncherActivities

            ``` methodSignature
            List<String> getLauncherActivities()
            ```

            [Returns:]{.returnLabel}
            :   list of names (as they appear in the manifest) of
                activities that should appear in the Android app drawer.

        []{#getPackage()}

        -   #### getPackage

            ``` methodSignature
            String getPackage()
            ```

            [Returns:]{.returnLabel}
            :   the value of the package attribute to the manifest
                element.

        []{#getVersionCode()}

        -   #### getVersionCode

            ``` methodSignature
            String getVersionCode()
            ```

            [Returns:]{.returnLabel}
            :   the value of the versionCode attribute to the manifest
                element.

        []{#getInstrumentationTestRunner()}

        -   #### getInstrumentationTestRunner

            ``` methodSignature
            String getInstrumentationTestRunner()
            ```

            [Returns:]{.returnLabel}
            :   the name of the instrumentation test runner.

        []{#getTargetPackage()}

        -   #### getTargetPackage

            ``` methodSignature
            String getTargetPackage()
            ```

            [Returns:]{.returnLabel}
            :   the value of the target package attribute to the
                manifest element.
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

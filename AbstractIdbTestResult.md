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
[Package]{.packageLabelInType} [com.facebook.buck.apple](package-summary.html)
:::

## Interface AbstractIdbTestResult {#interface-abstractidbtestresult .title title="Interface AbstractIdbTestResult"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        public interface AbstractIdbTestResult

    ::: block
    Object that represents the xctest result when using idb
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `String[]`            | `getActivityLogs()`   | ::: block             |
        |                       |                       | Array of strings that |
        |                       |                       | show the activity     |
        |                       |                       | logs                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getBundleName()`     | ::: block             |
        |                       |                       | String that           |
        |                       |                       | represents the name   |
        |                       |                       | of the test bundle    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getClassName()`      | ::: block             |
        |                       |                       | String that           |
        |                       |                       | represents the name   |
        |                       |                       | of the class of the   |
        |                       |                       | test                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Boolean`             | `getCrashed()`        | ::: block             |
        |                       |                       | Boolean that shows if |
        |                       |                       | the test crashed or   |
        |                       |                       | not                   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Float`               | `getDuration()`       | ::: block             |
        |                       |                       | Time spent executing  |
        |                       |                       | the test              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.fa               | `getFailureInfo()`    | ::: block             |
        | cebook.buck.apple.Imm |                       | Object that           |
        | utableIdbFailureInfo` |                       | represents the        |
        |                       |                       | failure information   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String[]`            | `getLogs()`           | ::: block             |
        |                       |                       | Array of strings that |
        |                       |                       | show the logs of the  |
        |                       |                       | test                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getMethodName()`     | ::: block             |
        |                       |                       | String that           |
        |                       |                       | represents the name   |
        |                       |                       | of the method of the  |
        |                       |                       | test                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Boolean`             | `getPassed()`         | ::: block             |
        |                       |                       | Boolean that shows if |
        |                       |                       | the test passed or    |
        |                       |                       | not                   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

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

        []{#getBundleName()}

        -   #### getBundleName

            ``` methodSignature
            String getBundleName()
            ```

            ::: block
            String that represents the name of the test bundle
            :::

        []{#getClassName()}

        -   #### getClassName

            ``` methodSignature
            String getClassName()
            ```

            ::: block
            String that represents the name of the class of the test
            :::

        []{#getMethodName()}

        -   #### getMethodName

            ``` methodSignature
            String getMethodName()
            ```

            ::: block
            String that represents the name of the method of the test
            :::

        []{#getLogs()}

        -   #### getLogs

            ``` methodSignature
            String[] getLogs()
            ```

            ::: block
            Array of strings that show the logs of the test
            :::

        []{#getDuration()}

        -   #### getDuration

            ``` methodSignature
            Float getDuration()
            ```

            ::: block
            Time spent executing the test
            :::

        []{#getPassed()}

        -   #### getPassed

            ``` methodSignature
            Boolean getPassed()
            ```

            ::: block
            Boolean that shows if the test passed or not
            :::

        []{#getCrashed()}

        -   #### getCrashed

            ``` methodSignature
            Boolean getCrashed()
            ```

            ::: block
            Boolean that shows if the test crashed or not
            :::

        []{#getFailureInfo()}

        -   #### getFailureInfo

            ``` methodSignature
            com.facebook.buck.apple.ImmutableIdbFailureInfo getFailureInfo()
            ```

            ::: block
            Object that represents the failure information
            :::

        []{#getActivityLogs()}

        -   #### getActivityLogs

            ``` methodSignature
            String[] getActivityLogs()
            ```

            ::: block
            Array of strings that show the activity logs
            :::
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

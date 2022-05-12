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
[Package]{.packageLabelInType} [com.facebook.buck.util.environment](package-summary.html)
:::

## Interface ExecutionEnvironment {#interface-executionenvironment .title title="Interface ExecutionEnvironment"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `DefaultExecutionEnvironment`

    ------------------------------------------------------------------------

        public interface ExecutionEnvironment
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `int`                 | `getAvailableCores()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getenv​(String key)`  | ::: block             |
        |                       |                       | Gets the environment  |
        |                       |                       | variable indicated by |
        |                       |                       | the specified key.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getHostname()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Network`             | `getL                 |                       |
        |                       | ikelyActiveNetwork()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Platform`            | `getPlatform()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `long`                | `getTotalMemory()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getUsername()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getWifiSsid()`       |                       |
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

        []{#getHostname()}

        -   #### getHostname

            ``` methodSignature
            String getHostname()
            ```

            [Returns:]{.returnLabel}
            :   The current hostname or \'unknown\'

        []{#getUsername()}

        -   #### getUsername

            ``` methodSignature
            String getUsername()
            ```

            [Returns:]{.returnLabel}
            :   The current username or \'unknown\'

        []{#getAvailableCores()}

        -   #### getAvailableCores

            ``` methodSignature
            int getAvailableCores()
            ```

            [Returns:]{.returnLabel}
            :   The number of cores on this machine.

        []{#getTotalMemory()}

        -   #### getTotalMemory

            ``` methodSignature
            long getTotalMemory()
            ```

            [Returns:]{.returnLabel}
            :   The amount of system memory on this machine in bytes.

        []{#getPlatform()}

        -   #### getPlatform

            ``` methodSignature
            Platform getPlatform()
            ```

            [Returns:]{.returnLabel}
            :   The current operating system.

        []{#getLikelyActiveNetwork()}

        -   #### getLikelyActiveNetwork

            ``` methodSignature
            Network getLikelyActiveNetwork()
            ```

            [Returns:]{.returnLabel}
            :   Whether an ethernet interface is available and enabled.

        []{#getWifiSsid()}

        -   #### getWifiSsid

            ``` methodSignature
            Optional<String> getWifiSsid()
            ```

            [Returns:]{.returnLabel}
            :   The SSID of the current wifi network if it can be
                determined.

        []{#getenv(java.lang.String)}

        -   #### getenv

            ``` methodSignature
            Optional<String> getenv​(String key)
            ```

            ::: block
            Gets the environment variable indicated by the specified
            key.
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

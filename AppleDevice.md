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
[Package]{.packageLabelInType} [com.facebook.buck.apple.simulator](package-summary.html)
:::

## Interface AppleDevice {#interface-appledevice .title title="Interface AppleDevice"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        public interface AppleDevice

    ::: block
    Object that represents an Apple simulator or a physical device. Used
    with idb.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `String`              | `getArchitecture()`   | ::: block             |
        |                       |                       | String that           |
        |                       |                       | represents the        |
        |                       |                       | architecture of the   |
        |                       |                       | device (i.e.,         |
        |                       |                       | \"x86_64\", etc)      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default String`      | `getHost()`           | ::: block             |
        |                       |                       | String that           |
        |                       |                       | represents the host   |
        |                       |                       | of the device         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `getIs_local()`       | ::: block             |
        |                       |                       | String that indicates |
        |                       |                       | if the device is      |
        |                       |                       | local or remote       |
        |                       |                       | (\"true\" or          |
        |                       |                       | \"false\")            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getName()`           | ::: block             |
        |                       |                       | String that           |
        |                       |                       | represents the name   |
        |                       |                       | of the device (i.e.,  |
        |                       |                       | \"iPhone X\", \"iPad  |
        |                       |                       | Air\", etc)           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getOs_version()`     | ::: block             |
        |                       |                       | String that           |
        |                       |                       | represents the iOS    |
        |                       |                       | version running on    |
        |                       |                       | the device (i.e.,     |
        |                       |                       | \"iOS 12.4\", etc)    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default int`         | `getPort()`           | ::: block             |
        |                       |                       | String that           |
        |                       |                       | represents the port   |
        |                       |                       | of the device         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getState()`          | ::: block             |
        |                       |                       | String that           |
        |                       |                       | represents the state  |
        |                       |                       | of the device (i.e.,  |
        |                       |                       | \"Booted\",           |
        |                       |                       | \"Shutdown\", etc)    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getType()`           | ::: block             |
        |                       |                       | String that           |
        |                       |                       | represents the type   |
        |                       |                       | of the device         |
        |                       |                       | (\"simulator\" or     |
        |                       |                       | \"device\")           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getUdid()`           | ::: block             |
        |                       |                       | String that           |
        |                       |                       | represents the udid   |
        |                       |                       | of the device (its    |
        |                       |                       | identifier)           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static AppleDevice`  | `o                    |                       |
        |                       | f​(String name,   Stri |                       |
        |                       | ng udid,   String sta |                       |
        |                       | te,   String type,    |                       |
        |                       | String os_version,    |                       |
        |                       | String architecture)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Default
        Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getName()}

        -   #### getName

            ``` methodSignature
            String getName()
            ```

            ::: block
            String that represents the name of the device (i.e.,
            \"iPhone X\", \"iPad Air\", etc)
            :::

        []{#getUdid()}

        -   #### getUdid

            ``` methodSignature
            String getUdid()
            ```

            ::: block
            String that represents the udid of the device (its
            identifier)
            :::

        []{#getState()}

        -   #### getState

            ``` methodSignature
            String getState()
            ```

            ::: block
            String that represents the state of the device (i.e.,
            \"Booted\", \"Shutdown\", etc)
            :::

        []{#getType()}

        -   #### getType

            ``` methodSignature
            String getType()
            ```

            ::: block
            String that represents the type of the device (\"simulator\"
            or \"device\")
            :::

        []{#getOs_version()}

        -   #### getOs_version

            ``` methodSignature
            String getOs_version()
            ```

            ::: block
            String that represents the iOS version running on the device
            (i.e., \"iOS 12.4\", etc)
            :::

        []{#getArchitecture()}

        -   #### getArchitecture

            ``` methodSignature
            String getArchitecture()
            ```

            ::: block
            String that represents the architecture of the device (i.e.,
            \"x86_64\", etc)
            :::

        []{#getHost()}

        -   #### getHost

            ``` methodSignature
            @Derived
            default String getHost()
            ```

            ::: block
            String that represents the host of the device
            :::

        []{#getPort()}

        -   #### getPort

            ``` methodSignature
            @Derived
            default int getPort()
            ```

            ::: block
            String that represents the port of the device
            :::

        []{#getIs_local()}

        -   #### getIs_local

            ``` methodSignature
            @Derived
            default boolean getIs_local()
            ```

            ::: block
            String that indicates if the device is local or remote
            (\"true\" or \"false\")
            :::

        []{#of(java.lang.String,java.lang.String,java.lang.String,java.lang.String,java.lang.String,java.lang.String)}

        -   #### of

            ``` methodSignature
            static AppleDevice of​(String name,
                                  String udid,
                                  String state,
                                  String type,
                                  String os_version,
                                  String architecture)
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

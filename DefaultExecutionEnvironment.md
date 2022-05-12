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
[Package]{.packageLabelInType} [com.facebook.buck.util.environment](package-summary.html)
:::

## Class DefaultExecutionEnvironment {#class-defaultexecutionenvironment .title title="Class DefaultExecutionEnvironment"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.environment.DefaultExecutionEnvironment

::: description
-   

    All Implemented Interfaces:
    :   `ExecutionEnvironment`

    ------------------------------------------------------------------------

        public class DefaultExecutionEnvironment
        extends Object
        implements ExecutionEnvironment
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                          Description
          ---------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `DefaultExecutionEnvironment​(com.google.common.collect.ImmutableMap<String,​String> environment,                            Properties properties)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
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

        []{#<init>(com.google.common.collect.ImmutableMap,java.util.Properties)}

        -   #### DefaultExecutionEnvironment

                public DefaultExecutionEnvironment​(com.google.common.collect.ImmutableMap<String,​String> environment,
                                                   Properties properties)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getHostname()}

        -   #### getHostname

            ``` methodSignature
            public String getHostname()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getHostname` in interface `ExecutionEnvironment`

            [Returns:]{.returnLabel}
            :   The current hostname or \'unknown\'

        []{#getUsername()}

        -   #### getUsername

            ``` methodSignature
            public String getUsername()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getUsername` in interface `ExecutionEnvironment`

            [Returns:]{.returnLabel}
            :   The current username or \'unknown\'

        []{#getAvailableCores()}

        -   #### getAvailableCores

            ``` methodSignature
            public int getAvailableCores()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getAvailableCores` in interface `ExecutionEnvironment`

            [Returns:]{.returnLabel}
            :   The number of cores on this machine.

        []{#getTotalMemory()}

        -   #### getTotalMemory

            ``` methodSignature
            public long getTotalMemory()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTotalMemory` in interface `ExecutionEnvironment`

            [Returns:]{.returnLabel}
            :   The amount of system memory on this machine in bytes.

        []{#getPlatform()}

        -   #### getPlatform

            ``` methodSignature
            public Platform getPlatform()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPlatform` in interface `ExecutionEnvironment`

            [Returns:]{.returnLabel}
            :   The current operating system.

        []{#getLikelyActiveNetwork()}

        -   #### getLikelyActiveNetwork

            ``` methodSignature
            public Network getLikelyActiveNetwork()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLikelyActiveNetwork` in
                interface `ExecutionEnvironment`

            [Returns:]{.returnLabel}
            :   Whether an ethernet interface is available and enabled.

        []{#getWifiSsid()}

        -   #### getWifiSsid

            ``` methodSignature
            public Optional<String> getWifiSsid()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getWifiSsid` in interface `ExecutionEnvironment`

            [Returns:]{.returnLabel}
            :   The SSID of the current wifi network if it can be
                determined.

        []{#getenv(java.lang.String)}

        -   #### getenv

            ``` methodSignature
            public Optional<String> getenv​(String key)
            ```

            ::: block
            [Description copied from
            interface: `ExecutionEnvironment`]{.descfrmTypeLabel}
            :::

            ::: block
            Gets the environment variable indicated by the specified
            key.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getenv` in interface `ExecutionEnvironment`
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

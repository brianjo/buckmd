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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.util.network.hostname](package-summary.html)
:::

## Interface HostnameFetchingWin32Library {#interface-hostnamefetchingwin32library .title title="Interface HostnameFetchingWin32Library"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `com.sun.jna.AltCallingConvention`, `com.sun.jna.Library`,
        `com.sun.jna.win32.StdCall`, `com.sun.jna.win32.StdCallLibrary`

    ------------------------------------------------------------------------

        public interface HostnameFetchingWin32Library
        extends com.sun.jna.win32.StdCallLibrary
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.sun.jna.Library}

            ### Nested classes/interfaces inherited from interface com.sun.jna.Library

            `com.sun.jna.Library.Handler`

        ```{=html}
        <!-- -->
        ```
        -   []{#nested.classes.inherited.from.class.com.sun.jna.win32.StdCallLibrary}

            ### Nested classes/interfaces inherited from interface com.sun.jna.win32.StdCallLibrary

            `com.sun.jna.win32.StdCallLibrary.StdCallCallback`
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                       Field                                                           Description
          --------------------------------------- --------------------------------------------------------------- -------------
          `static int`                            `COMPUTER_NAME_FORMAT__ComputerNameDnsDomain`                    
          `static int`                            `COMPUTER_NAME_FORMAT__ComputerNameDnsFullyQualified`            
          `static int`                            `COMPUTER_NAME_FORMAT__ComputerNameDnsHostname`                  
          `static int`                            `COMPUTER_NAME_FORMAT__ComputerNameNetBIOS`                      
          `static int`                            `COMPUTER_NAME_FORMAT__ComputerNamePhysicalDnsDomain`            
          `static int`                            `COMPUTER_NAME_FORMAT__ComputerNamePhysicalDnsFullyQualified`    
          `static int`                            `COMPUTER_NAME_FORMAT__ComputerNamePhysicalDnsHostname`          
          `static int`                            `COMPUTER_NAME_FORMAT__ComputerNamePhysicalNetBIOS`              
          `static HostnameFetchingWin32Library`   `INSTANCE`                                                       

          : Fields[ ]{.tabEnd}

        -   []{#fields.inherited.from.class.com.sun.jna.Library}

            ### Fields inherited from interface com.sun.jna.Library

            `OPTION_ALLOW_OBJECTS, OPTION_CALLING_CONVENTION, OPTION_CLASSLOADER, OPTION_FUNCTION_MAPPER, OPTION_INVOCATION_MAPPER, OPTION_OPEN_FLAGS, OPTION_STRING_ENCODING, OPTION_STRUCTURE_ALIGNMENT, OPTION_TYPE_MAPPER`

        ```{=html}
        <!-- -->
        ```
        -   []{#fields.inherited.from.class.com.sun.jna.win32.StdCallLibrary}

            ### Fields inherited from interface com.sun.jna.win32.StdCallLibrary

            `FUNCTION_MAPPER, STDCALL_CONVENTION`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                                                          Description
          ------------------- ------------------------------------------------------------------------------------------------------------------------------- -------------
          `boolean`           `GetComputerNameEx​(int nameType,                  char[] buffer,                  com.sun.jna.ptr.IntByReference bufferSize)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#INSTANCE}

        -   #### INSTANCE

                static final HostnameFetchingWin32Library INSTANCE

        []{#COMPUTER_NAME_FORMAT__ComputerNameNetBIOS}

        -   #### COMPUTER_NAME_FORMAT\_\_ComputerNameNetBIOS

                static final int COMPUTER_NAME_FORMAT__ComputerNameNetBIOS

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.util.network.hostname.HostnameFetchingWin32Library.COMPUTER_NAME_FORMAT__ComputerNameNetBIOS)

        []{#COMPUTER_NAME_FORMAT__ComputerNameDnsHostname}

        -   #### COMPUTER_NAME_FORMAT\_\_ComputerNameDnsHostname

                static final int COMPUTER_NAME_FORMAT__ComputerNameDnsHostname

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.util.network.hostname.HostnameFetchingWin32Library.COMPUTER_NAME_FORMAT__ComputerNameDnsHostname)

        []{#COMPUTER_NAME_FORMAT__ComputerNameDnsDomain}

        -   #### COMPUTER_NAME_FORMAT\_\_ComputerNameDnsDomain

                static final int COMPUTER_NAME_FORMAT__ComputerNameDnsDomain

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.util.network.hostname.HostnameFetchingWin32Library.COMPUTER_NAME_FORMAT__ComputerNameDnsDomain)

        []{#COMPUTER_NAME_FORMAT__ComputerNameDnsFullyQualified}

        -   #### COMPUTER_NAME_FORMAT\_\_ComputerNameDnsFullyQualified

                static final int COMPUTER_NAME_FORMAT__ComputerNameDnsFullyQualified

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.util.network.hostname.HostnameFetchingWin32Library.COMPUTER_NAME_FORMAT__ComputerNameDnsFullyQualified)

        []{#COMPUTER_NAME_FORMAT__ComputerNamePhysicalNetBIOS}

        -   #### COMPUTER_NAME_FORMAT\_\_ComputerNamePhysicalNetBIOS

                static final int COMPUTER_NAME_FORMAT__ComputerNamePhysicalNetBIOS

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.util.network.hostname.HostnameFetchingWin32Library.COMPUTER_NAME_FORMAT__ComputerNamePhysicalNetBIOS)

        []{#COMPUTER_NAME_FORMAT__ComputerNamePhysicalDnsHostname}

        -   #### COMPUTER_NAME_FORMAT\_\_ComputerNamePhysicalDnsHostname

                static final int COMPUTER_NAME_FORMAT__ComputerNamePhysicalDnsHostname

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.util.network.hostname.HostnameFetchingWin32Library.COMPUTER_NAME_FORMAT__ComputerNamePhysicalDnsHostname)

        []{#COMPUTER_NAME_FORMAT__ComputerNamePhysicalDnsDomain}

        -   #### COMPUTER_NAME_FORMAT\_\_ComputerNamePhysicalDnsDomain

                static final int COMPUTER_NAME_FORMAT__ComputerNamePhysicalDnsDomain

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.util.network.hostname.HostnameFetchingWin32Library.COMPUTER_NAME_FORMAT__ComputerNamePhysicalDnsDomain)

        []{#COMPUTER_NAME_FORMAT__ComputerNamePhysicalDnsFullyQualified}

        -   #### COMPUTER_NAME_FORMAT\_\_ComputerNamePhysicalDnsFullyQualified

                static final int COMPUTER_NAME_FORMAT__ComputerNamePhysicalDnsFullyQualified

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.util.network.hostname.HostnameFetchingWin32Library.COMPUTER_NAME_FORMAT__ComputerNamePhysicalDnsFullyQualified)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#GetComputerNameEx(int,char[],com.sun.jna.ptr.IntByReference)}

        -   #### GetComputerNameEx

            ``` methodSignature
            boolean GetComputerNameEx​(int nameType,
                                      char[] buffer,
                                      com.sun.jna.ptr.IntByReference bufferSize)
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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

<div>

-   Summary: 
-   [Nested](#nested.class.summary) \| 
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

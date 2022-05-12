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
[Package]{.packageLabelInType} [com.facebook.buck.io.windowsfs](package-summary.html)
:::

## Interface WindowsFSLibrary {#interface-windowsfslibrary .title title="Interface WindowsFSLibrary"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `com.sun.jna.Library`

    ------------------------------------------------------------------------

        public interface WindowsFSLibrary
        extends com.sun.jna.Library

    ::: block
    Utility class to bridge native windows FS calls to Java using JNA.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.sun.jna.Library}

            ### Nested classes/interfaces inherited from interface com.sun.jna.Library

            `com.sun.jna.Library.Handler`
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type           Field                                            Description
          --------------------------- ------------------------------------------------ -------------
          `static int`                `ERROR_ALREADY_EXISTS`                            
          `static int`                `ERROR_PRIVILEGE_NOT_HELD`                        
          `static WindowsFSLibrary`   `INSTANCE`                                        
          `static int`                `INVALID_PARAMETER_ERROR`                         
          `static int`                `SYMBOLIC_LINK_FLAG_ALLOW_UNPRIVILEGED_CREATE`    
          `static int`                `SYMBOLIC_LINK_FLAG_DIRECTORY`                    

          : Fields[ ]{.tabEnd}

        -   []{#fields.inherited.from.class.com.sun.jna.Library}

            ### Fields inherited from interface com.sun.jna.Library

            `OPTION_ALLOW_OBJECTS, OPTION_CALLING_CONVENTION, OPTION_CLASSLOADER, OPTION_FUNCTION_MAPPER, OPTION_INVOCATION_MAPPER, OPTION_OPEN_FLAGS, OPTION_STRING_ENCODING, OPTION_STRUCTURE_ALIGNMENT, OPTION_TYPE_MAPPER`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                                                        Description
          ------------------- ----------------------------------------------------------------------------------------------------------------------------- -------------
          `byte`              `CreateSymbolicLinkW​(String lpSymlinkFileName,                    String lpTargetFileName,                    int dwFlags)`    
          `int`               `GetLastError()`                                                                                                               

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

                static final WindowsFSLibrary INSTANCE

        []{#SYMBOLIC_LINK_FLAG_DIRECTORY}

        -   #### SYMBOLIC_LINK_FLAG_DIRECTORY

                static final int SYMBOLIC_LINK_FLAG_DIRECTORY

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.io.windowsfs.WindowsFSLibrary.SYMBOLIC_LINK_FLAG_DIRECTORY)

        []{#SYMBOLIC_LINK_FLAG_ALLOW_UNPRIVILEGED_CREATE}

        -   #### SYMBOLIC_LINK_FLAG_ALLOW_UNPRIVILEGED_CREATE

                static final int SYMBOLIC_LINK_FLAG_ALLOW_UNPRIVILEGED_CREATE

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.io.windowsfs.WindowsFSLibrary.SYMBOLIC_LINK_FLAG_ALLOW_UNPRIVILEGED_CREATE)

        []{#INVALID_PARAMETER_ERROR}

        -   #### INVALID_PARAMETER_ERROR

                static final int INVALID_PARAMETER_ERROR

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.io.windowsfs.WindowsFSLibrary.INVALID_PARAMETER_ERROR)

        []{#ERROR_ALREADY_EXISTS}

        -   #### ERROR_ALREADY_EXISTS

                static final int ERROR_ALREADY_EXISTS

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.io.windowsfs.WindowsFSLibrary.ERROR_ALREADY_EXISTS)

        []{#ERROR_PRIVILEGE_NOT_HELD}

        -   #### ERROR_PRIVILEGE_NOT_HELD

                static final int ERROR_PRIVILEGE_NOT_HELD

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.io.windowsfs.WindowsFSLibrary.ERROR_PRIVILEGE_NOT_HELD)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#CreateSymbolicLinkW(java.lang.String,java.lang.String,int)}

        -   #### CreateSymbolicLinkW

            ``` methodSignature
            byte CreateSymbolicLinkW​(String lpSymlinkFileName,
                                     String lpTargetFileName,
                                     int dwFlags)
            ```

        []{#GetLastError()}

        -   #### GetLastError

            ``` methodSignature
            int GetLastError()
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

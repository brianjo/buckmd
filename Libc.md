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
[Package]{.packageLabelInType} [com.facebook.buck.util](package-summary.html)
:::

## Interface Libc {#interface-libc .title title="Interface Libc"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `com.sun.jna.Library`

    ------------------------------------------------------------------------

        public interface Libc
        extends com.sun.jna.Library
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type     Interface               Description
          --------------------- ----------------------- -------------
          `static class `       `Libc.Constants`         
          `static interface `   `Libc.OpenPtyLibrary`    

          : Nested Classes[ ]{.tabEnd}

        -   []{#nested.classes.inherited.from.class.com.sun.jna.Library}

            ### Nested classes/interfaces inherited from interface com.sun.jna.Library

            `com.sun.jna.Library.Handler`
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field        Description
          ------------------- ------------ -------------
          `static Libc`       `INSTANCE`    

          : Fields[ ]{.tabEnd}

        -   []{#fields.inherited.from.class.com.sun.jna.Library}

            ### Fields inherited from interface com.sun.jna.Library

            `OPTION_ALLOW_OBJECTS, OPTION_CALLING_CONVENTION, OPTION_CLASSLOADER, OPTION_FUNCTION_MAPPER, OPTION_INVOCATION_MAPPER, OPTION_OPEN_FLAGS, OPTION_STRING_ENCODING, OPTION_STRUCTURE_ALIGNMENT, OPTION_TYPE_MAPPER`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type       Method                                                                   Description
          ----------------------- ------------------------------------------------------------------------ -------------
          `int`                   `fcntl​(int fd,      int cmd,      Object... args)`                        
          `int`                   `getpid()`                                                                
          `int`                   `getuid()`                                                                
          `int`                   `ioctl​(int fd,      com.sun.jna.Pointer request,      Object... args)`    
          `int`                   `kill​(int pid,     int sig)`                                              
          `int`                   `setsid()`                                                                
          `com.sun.jna.Pointer`   `signal​(int signal,       com.sun.jna.Pointer function)`                  

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

                static final Libc INSTANCE
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#signal(int,com.sun.jna.Pointer)}

        -   #### signal

            ``` methodSignature
            com.sun.jna.Pointer signal​(int signal,
                                       com.sun.jna.Pointer function)
            ```

        []{#kill(int,int)}

        -   #### kill

            ``` methodSignature
            int kill​(int pid,
                     int sig)
              throws com.sun.jna.LastErrorException
            ```

            [Throws:]{.throwsLabel}
            :   `com.sun.jna.LastErrorException`

        []{#setsid()}

        -   #### setsid

            ``` methodSignature
            int setsid()
            ```

        []{#ioctl(int,com.sun.jna.Pointer,java.lang.Object...)}

        -   #### ioctl

            ``` methodSignature
            int ioctl​(int fd,
                      com.sun.jna.Pointer request,
                      Object... args)
            ```

        []{#fcntl(int,int,java.lang.Object...)}

        -   #### fcntl

            ``` methodSignature
            int fcntl​(int fd,
                      int cmd,
                      Object... args)
            ```

        []{#getpid()}

        -   #### getpid

            ``` methodSignature
            int getpid()
            ```

        []{#getuid()}

        -   #### getuid

            ``` methodSignature
            int getuid()
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

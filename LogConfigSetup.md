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
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.log](package-summary.html)
:::

## Class LogConfigSetup {#class-logconfigsetup .title title="Class LogConfigSetup"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.log.LogConfigSetup

::: description
-   

    ------------------------------------------------------------------------

        public abstract class LogConfigSetup
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                      Description
          ------------------- -------------------------- -------------
          `static class `     `LogConfigSetup.Builder`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type         Field                          Description
          ------------------------- ------------------------------ -------------
          `static int`              `DEFAULT_MAX_COUNT`             
          `static long`             `DEFAULT_MAX_LOG_SIZE_BYTES`    
          `static int`              `DEFAULT_MIN_COUNT`             
          `static LogConfigSetup`   `DEFAULT_SETUP`                 

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor          Description
          -------------------- -------------
          `LogConfigSetup()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                 Method                   Description
          --------------------------------- ------------------------ -------------
          `static LogConfigSetup.Builder`   `builder()`               
          `int`                             `getCount()`              
          `abstract Path`                   `getLogDir()`             
          `Path`                            `getLogFilePath()`        
          `String`                          `getLogFilePrefix()`      
          `long`                            `getMaxLogSizeBytes()`    
          `boolean`                         `getRotateLog()`          

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#DEFAULT_MAX_COUNT}

        -   #### DEFAULT_MAX_COUNT

                public static final int DEFAULT_MAX_COUNT

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.log.LogConfigSetup.DEFAULT_MAX_COUNT)

        []{#DEFAULT_MIN_COUNT}

        -   #### DEFAULT_MIN_COUNT

                public static final int DEFAULT_MIN_COUNT

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.log.LogConfigSetup.DEFAULT_MIN_COUNT)

        []{#DEFAULT_MAX_LOG_SIZE_BYTES}

        -   #### DEFAULT_MAX_LOG_SIZE_BYTES

                public static final long DEFAULT_MAX_LOG_SIZE_BYTES

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.log.LogConfigSetup.DEFAULT_MAX_LOG_SIZE_BYTES)

        []{#DEFAULT_SETUP}

        -   #### DEFAULT_SETUP

                public static final LogConfigSetup DEFAULT_SETUP
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### LogConfigSetup

                public LogConfigSetup()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getLogDir()}

        -   #### getLogDir

            ``` methodSignature
            public abstract Path getLogDir()
            ```

        []{#getRotateLog()}

        -   #### getRotateLog

            ``` methodSignature
            @Default
            public boolean getRotateLog()
            ```

        []{#getCount()}

        -   #### getCount

            ``` methodSignature
            @Default
            public int getCount()
            ```

        []{#getMaxLogSizeBytes()}

        -   #### getMaxLogSizeBytes

            ``` methodSignature
            @Default
            public long getMaxLogSizeBytes()
            ```

        []{#getLogFilePrefix()}

        -   #### getLogFilePrefix

            ``` methodSignature
            @Default
            public String getLogFilePrefix()
            ```

        []{#getLogFilePath()}

        -   #### getLogFilePath

            ``` methodSignature
            public Path getLogFilePath()
            ```

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static LogConfigSetup.Builder builder()
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
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

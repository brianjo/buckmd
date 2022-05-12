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
[Package]{.packageLabelInType} [com.facebook.buck.android](package-summary.html)
:::

## Class BuckEventAndroidLogger {#class-buckeventandroidlogger .title title="Class BuckEventAndroidLogger"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.BuckEventAndroidLogger

::: description
-   

    All Implemented Interfaces:
    :   `com.android.common.utils.ILogger`

    ------------------------------------------------------------------------

        public class BuckEventAndroidLogger
        extends Object
        implements com.android.common.utils.ILogger

    ::: block
    Implementation of `ILogger` which posts to an
    [`BuckEventBus`](../event/BuckEventBus.html "interface in com.facebook.buck.event")
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                       Description
          ------------------------------------------------- -------------
          `BuckEventAndroidLogger​(BuckEventBus eventBus)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                       Description
          ------------------- ---------------------------------------------------------------------------- -------------
          `void`              `error​(Throwable throwable,      String errorFormat,      Object... args)`    
          `void`              `info​(String msgFormat,     Object... args)`                                  
          `void`              `verbose​(String msgFormat,        Object... args)`                            
          `void`              `warning​(String msgFormat,        Object... args)`                            

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

        []{#<init>(com.facebook.buck.event.BuckEventBus)}

        -   #### BuckEventAndroidLogger

                public BuckEventAndroidLogger​(BuckEventBus eventBus)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#error(java.lang.Throwable,java.lang.String,java.lang.Object...)}

        -   #### error

            ``` methodSignature
            public void error​(@Nullable
                              Throwable throwable,
                              @Nullable
                              String errorFormat,
                              Object... args)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `error` in interface `com.android.common.utils.ILogger`

        []{#warning(java.lang.String,java.lang.Object...)}

        -   #### warning

            ``` methodSignature
            public void warning​(String msgFormat,
                                Object... args)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `warning` in
                interface `com.android.common.utils.ILogger`

        []{#info(java.lang.String,java.lang.Object...)}

        -   #### info

            ``` methodSignature
            public void info​(String msgFormat,
                             Object... args)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `info` in interface `com.android.common.utils.ILogger`

        []{#verbose(java.lang.String,java.lang.Object...)}

        -   #### verbose

            ``` methodSignature
            public void verbose​(String msgFormat,
                                Object... args)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `verbose` in
                interface `com.android.common.utils.ILogger`
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

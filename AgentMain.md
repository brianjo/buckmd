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
[Package]{.packageLabelInType} [com.facebook.buck.android.agent](package-summary.html)
:::

## Class AgentMain {#class-agentmain .title title="Class AgentMain"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.agent.AgentMain

::: description
-   

    ------------------------------------------------------------------------

        public class AgentMain
        extends Object

    ::: block
    Main class for an agent that runs on an Android device to aid app
    installation.
    This does not run as a normal Android app. It is packaged into an
    APK and installed as a convenient way to get it on the device, but
    it is run from the \"adb shell\" command line using the \"dalvikvm\"
    command. Therefore, we do not have an Android Context and therefore
    cannot interact with any system services.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                               Description
          ------------------- ----------------------------------- -------------
          `static int`        `CONNECT_TIMEOUT_MS`                 
          `static int`        `LINE_LENGTH_LIMIT`                  
          `static int`        `RECEIVE_TIMEOUT_MS`                 
          `static int`        `TOTAL_RECEIVE_TIMEOUT_MS_PER_MB`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                  Description
          ------------------- ----------------------- -------------
          `static void`       `main​(String[] args)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
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

        []{#LINE_LENGTH_LIMIT}

        -   #### LINE_LENGTH_LIMIT

                public static final int LINE_LENGTH_LIMIT

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.android.agent.AgentMain.LINE_LENGTH_LIMIT)

        []{#CONNECT_TIMEOUT_MS}

        -   #### CONNECT_TIMEOUT_MS

                public static final int CONNECT_TIMEOUT_MS

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.android.agent.AgentMain.CONNECT_TIMEOUT_MS)

        []{#RECEIVE_TIMEOUT_MS}

        -   #### RECEIVE_TIMEOUT_MS

                public static final int RECEIVE_TIMEOUT_MS

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.android.agent.AgentMain.RECEIVE_TIMEOUT_MS)

        []{#TOTAL_RECEIVE_TIMEOUT_MS_PER_MB}

        -   #### TOTAL_RECEIVE_TIMEOUT_MS_PER_MB

                public static final int TOTAL_RECEIVE_TIMEOUT_MS_PER_MB

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.android.agent.AgentMain.TOTAL_RECEIVE_TIMEOUT_MS_PER_MB)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#main(java.lang.String[])}

        -   #### main

            ``` methodSignature
            public static void main​(String[] args)
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

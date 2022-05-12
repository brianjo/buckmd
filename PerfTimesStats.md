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
[Package]{.packageLabelInType} [com.facebook.buck.log](package-summary.html)
:::

## Class PerfTimesStats {#class-perftimesstats .title title="Class PerfTimesStats"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.log.PerfTimesStats

::: description
-   

    ------------------------------------------------------------------------

        public abstract class PerfTimesStats
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                      Description
          ------------------- -------------------------- -------------
          `static class `     `PerfTimesStats.Builder`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor          Description
          -------------------- -------------
          `PerfTimesStats()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                 Method                      Description
          --------------------------------- --------------------------- -------------
          `static PerfTimesStats.Builder`   `builder()`                  
          `Long`                            `getActionGraphTimeMs()`     
          `Long`                            `getBuildTimeMs()`           
          `Long`                            `getFetchTimeMs()`           
          `Long`                            `getInitTimeMs()`            
          `Long`                            `getInstallTimeMs()`         
          `Long`                            `getParseTimeMs()`           
          `Long`                            `getProcessingTimeMs()`      
          `Long`                            `getProjectTimeMs()`         
          `Long`                            `getPythonTimeMs()`          
          `Long`                            `getRulekeyTimeMs()`         
          `Long`                            `getTotalRulekeyTimeMs()`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
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

        []{#<init>()}

        -   #### PerfTimesStats

                public PerfTimesStats()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getPythonTimeMs()}

        -   #### getPythonTimeMs

            ``` methodSignature
            @Default
            public Long getPythonTimeMs()
            ```

            [Returns:]{.returnLabel}
            :   duration of the time spent in python, in milliseconds.

        []{#getInitTimeMs()}

        -   #### getInitTimeMs

            ``` methodSignature
            @Default
            public Long getInitTimeMs()
            ```

            [Returns:]{.returnLabel}
            :   duration Buck spends initializing, in milliseconds.

        []{#getProcessingTimeMs()}

        -   #### getProcessingTimeMs

            ``` methodSignature
            @Default
            public Long getProcessingTimeMs()
            ```

            [Returns:]{.returnLabel}
            :   time spent between initialization and start of parsing,
                in milliseconds.

        []{#getParseTimeMs()}

        -   #### getParseTimeMs

            ``` methodSignature
            @Default
            public Long getParseTimeMs()
            ```

            [Returns:]{.returnLabel}
            :   time spent parsing and processing BUCK files, in
                milliseconds.

        []{#getActionGraphTimeMs()}

        -   #### getActionGraphTimeMs

            ``` methodSignature
            @Default
            public Long getActionGraphTimeMs()
            ```

            [Returns:]{.returnLabel}
            :   time it takes to generate the action graph, in
                milliseconds.

        []{#getRulekeyTimeMs()}

        -   #### getRulekeyTimeMs

            ``` methodSignature
            @Default
            public Long getRulekeyTimeMs()
            ```

            [Returns:]{.returnLabel}
            :   duration of the rule keys computation, from the start of
                rule key calculation to the fetching of the first
                artifact from the remote cache, in milliseconds.

        []{#getTotalRulekeyTimeMs()}

        -   #### getTotalRulekeyTimeMs

            ``` methodSignature
            @Default
            public Long getTotalRulekeyTimeMs()
            ```

            [Returns:]{.returnLabel}
            :   rule key computation is happening throughout the build
                with different types of rule keys. This measures the
                total time we spend calculating all different types of
                rule keys.

        []{#getFetchTimeMs()}

        -   #### getFetchTimeMs

            ``` methodSignature
            @Default
            public Long getFetchTimeMs()
            ```

            [Returns:]{.returnLabel}
            :   duration of the fetch operation, from the first fetch
                event to the start of the local build, in milliseconds.

        []{#getBuildTimeMs()}

        -   #### getBuildTimeMs

            ``` methodSignature
            @Default
            public Long getBuildTimeMs()
            ```

            [Returns:]{.returnLabel}
            :   duration of the local build phase, from start of the
                local build to when the build completes, in
                milliseconds.

        []{#getInstallTimeMs()}

        -   #### getInstallTimeMs

            ``` methodSignature
            @Default
            public Long getInstallTimeMs()
            ```

            [Returns:]{.returnLabel}
            :   time it takes to install to a device, in milliseconds.

        []{#getProjectTimeMs()}

        -   #### getProjectTimeMs

            ``` methodSignature
            @Default
            public Long getProjectTimeMs()
            ```

            [Returns:]{.returnLabel}
            :   time it takes to generate an IDE project, in
                milliseconds.

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static PerfTimesStats.Builder builder()
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

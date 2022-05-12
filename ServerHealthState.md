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
[Package]{.packageLabelInType} [com.facebook.buck.slb](package-summary.html)
:::

## Class ServerHealthState {#class-serverhealthstate .title title="Class ServerHealthState"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.slb.ServerHealthState

::: description
-   

    ------------------------------------------------------------------------

        public class ServerHealthState
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                            Description
          ---------------------------------------------------------------------------------------------------------------------- -------------
          `ServerHealthState​(URI server)`                                                                                         
          `ServerHealthState​(URI server,                  int minSamplesToReportError)`                                           
          `ServerHealthState​(URI server,                  int maxSamplesStored,                  int minSamplesToReportError)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `float`               | `getErrorPer          |                       |
        |                       | centage​(long nowMilli |                       |
        |                       | s,                    |                       |
        |                       | int timeRangeMillis)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `IOException`         | `getLastException()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `float`               | `getLastRepor         |                       |
        |                       | tedErrorPercentage()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `long`                | `getL                 |                       |
        |                       | astReportedLatency()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getL                 |                       |
        |                       | astReportedSamples()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `long`                | `getPingLatencyM      |                       |
        |                       | illis​(long nowMillis, |                       |
        |                       |                       |                       |
        |                       | int timeRangeMillis)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getPing              |                       |
        |                       | LatencySampleCount()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `get                  |                       |
        |                       | RequestSampleCount()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `URI`                 | `getServer()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `reportExcept         |                       |
        |                       | ion​(IOException exp)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `reportPi             | ::: block             |
        |                       | ngLatency​(long nowMil | NOTE: Assumes         |
        |                       | lis,                  | nowMillis is roughly  |
        |                       |  long latencyMillis)` | non-decreasing in     |
        |                       |                       | consecutive calls.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `reportRequestE       | ::: block             |
        |                       | rror​(long nowMillis)` | NOTE: Assumes         |
        |                       |                       | nowMillis is roughly  |
        |                       |                       | non-decreasing in     |
        |                       |                       | consecutive calls.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `reportRequestSuc     | ::: block             |
        |                       | cess​(long nowMillis)` | NOTE: Assumes         |
        |                       |                       | nowMillis is roughly  |
        |                       |                       | non-decreasing in     |
        |                       |                       | consecutive calls.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString​(lon         |                       |
        |                       | g nowMillis,          |                       |
        |                       | int timeRangeMillis)` |                       |
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

        []{#<init>(java.net.URI)}

        -   #### ServerHealthState

                public ServerHealthState​(URI server)

        []{#<init>(java.net.URI,int)}

        -   #### ServerHealthState

                public ServerHealthState​(URI server,
                                         int minSamplesToReportError)

        []{#<init>(java.net.URI,int,int)}

        -   #### ServerHealthState

                public ServerHealthState​(URI server,
                                         int maxSamplesStored,
                                         int minSamplesToReportError)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#reportPingLatency(long,long)}

        -   #### reportPingLatency

            ``` methodSignature
            public void reportPingLatency​(long nowMillis,
                                          long latencyMillis)
            ```

            ::: block
            NOTE: Assumes nowMillis is roughly non-decreasing in
            consecutive calls.
            :::

            [Parameters:]{.paramLabel}
            :   `nowMillis` -
            :   `latencyMillis` -

        []{#reportException(java.io.IOException)}

        -   #### reportException

            ``` methodSignature
            public void reportException​(IOException exp)
            ```

        []{#reportRequestSuccess(long)}

        -   #### reportRequestSuccess

            ``` methodSignature
            public void reportRequestSuccess​(long nowMillis)
            ```

            ::: block
            NOTE: Assumes nowMillis is roughly non-decreasing in
            consecutive calls.
            :::

            [Parameters:]{.paramLabel}
            :   `nowMillis` -

        []{#reportRequestError(long)}

        -   #### reportRequestError

            ``` methodSignature
            public void reportRequestError​(long nowMillis)
            ```

            ::: block
            NOTE: Assumes nowMillis is roughly non-decreasing in
            consecutive calls.
            :::

            [Parameters:]{.paramLabel}
            :   `nowMillis` -

        []{#getPingLatencySampleCount()}

        -   #### getPingLatencySampleCount

            ``` methodSignature
            public int getPingLatencySampleCount()
            ```

        []{#getRequestSampleCount()}

        -   #### getRequestSampleCount

            ``` methodSignature
            public int getRequestSampleCount()
            ```

        []{#getErrorPercentage(long,int)}

        -   #### getErrorPercentage

            ``` methodSignature
            public float getErrorPercentage​(long nowMillis,
                                            int timeRangeMillis)
            ```

            [Parameters:]{.paramLabel}
            :   `nowMillis` - Current timestamp.
            :   `timeRangeMillis` - Time range for \'nowMillis\' to
                compute the errorPercentage for.

            [Returns:]{.returnLabel}
            :   Value in the interval \[0.0, 1.0\].

        []{#getServer()}

        -   #### getServer

            ``` methodSignature
            public URI getServer()
            ```

        []{#getPingLatencyMillis(long,int)}

        -   #### getPingLatencyMillis

            ``` methodSignature
            public long getPingLatencyMillis​(long nowMillis,
                                             int timeRangeMillis)
            ```

        []{#getLastException()}

        -   #### getLastException

            ``` methodSignature
            @Nullable
            public IOException getLastException()
            ```

        []{#toString(long,int)}

        -   #### toString

            ``` methodSignature
            public String toString​(long nowMillis,
                                   int timeRangeMillis)
            ```

        []{#getLastReportedErrorPercentage()}

        -   #### getLastReportedErrorPercentage

            ``` methodSignature
            public float getLastReportedErrorPercentage()
            ```

        []{#getLastReportedSamples()}

        -   #### getLastReportedSamples

            ``` methodSignature
            public int getLastReportedSamples()
            ```

        []{#getLastReportedLatency()}

        -   #### getLastReportedLatency

            ``` methodSignature
            public long getLastReportedLatency()
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

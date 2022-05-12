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
[Package]{.packageLabelInType} [com.facebook.buck.counters](package-summary.html)
:::

## Class CounterRegistryImpl {#class-counterregistryimpl .title title="Class CounterRegistryImpl"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.counters.CounterRegistryImpl

::: description
-   

    All Implemented Interfaces:
    :   `CounterRegistry`, `Closeable`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class CounterRegistryImpl
        extends Object
        implements CounterRegistry
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.counters.CounterRegistry}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.counters.[CounterRegistry](CounterRegistry.html "interface in com.facebook.buck.counters")

            `CounterRegistry.AsyncCounterRegistrationEvent`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                        Description
          -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `CounterRegistryImpl​(ScheduledExecutorService service,                    BuckEventBus eventBus)`                                                                                                   
          `CounterRegistryImpl​(ScheduledExecutorService service,                    BuckEventBus eventBus,                    long firstFlushIntervalMillis,                    long flushIntervalMillis)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                                                                               Description
          ------------------- ---------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `void`              `close()`                                                                                                                                             
          `IntegerCounter`    `newIntegerCounter​(String category,                  String name,                  com.google.common.collect.ImmutableMap<String,​String> tags)`       
          `SamplingCounter`   `newSamplingCounter​(String category,                   String name,                   com.google.common.collect.ImmutableMap<String,​String> tags)`    
          `TagSetCounter`     `newTagSetCounter​(String category,                 String name,                 com.google.common.collect.ImmutableMap<String,​String> tags)`          
          `void`              `registerCounters​(CounterRegistry.AsyncCounterRegistrationEvent event)`                                                                               
          `void`              `registerCounters​(Collection<Counter> countersToRegister)`                                                                                            

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

        []{#<init>(java.util.concurrent.ScheduledExecutorService,com.facebook.buck.event.BuckEventBus)}

        -   #### CounterRegistryImpl

                public CounterRegistryImpl​(ScheduledExecutorService service,
                                           BuckEventBus eventBus)

        []{#<init>(java.util.concurrent.ScheduledExecutorService,com.facebook.buck.event.BuckEventBus,long,long)}

        -   #### CounterRegistryImpl

                public CounterRegistryImpl​(ScheduledExecutorService service,
                                           BuckEventBus eventBus,
                                           long firstFlushIntervalMillis,
                                           long flushIntervalMillis)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#newIntegerCounter(java.lang.String,java.lang.String,com.google.common.collect.ImmutableMap)}

        -   #### newIntegerCounter

            ``` methodSignature
            public IntegerCounter newIntegerCounter​(String category,
                                                    String name,
                                                    com.google.common.collect.ImmutableMap<String,​String> tags)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `newIntegerCounter` in interface `CounterRegistry`

        []{#newSamplingCounter(java.lang.String,java.lang.String,com.google.common.collect.ImmutableMap)}

        -   #### newSamplingCounter

            ``` methodSignature
            public SamplingCounter newSamplingCounter​(String category,
                                                      String name,
                                                      com.google.common.collect.ImmutableMap<String,​String> tags)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `newSamplingCounter` in interface `CounterRegistry`

        []{#newTagSetCounter(java.lang.String,java.lang.String,com.google.common.collect.ImmutableMap)}

        -   #### newTagSetCounter

            ``` methodSignature
            public TagSetCounter newTagSetCounter​(String category,
                                                  String name,
                                                  com.google.common.collect.ImmutableMap<String,​String> tags)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `newTagSetCounter` in interface `CounterRegistry`

        []{#registerCounters(java.util.Collection)}

        -   #### registerCounters

            ``` methodSignature
            public void registerCounters​(Collection<Counter> countersToRegister)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `registerCounters` in interface `CounterRegistry`

        []{#registerCounters(com.facebook.buck.counters.CounterRegistry.AsyncCounterRegistrationEvent)}

        -   #### registerCounters

            ``` methodSignature
            public void registerCounters​(CounterRegistry.AsyncCounterRegistrationEvent event)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `registerCounters` in interface `CounterRegistry`

        []{#close()}

        -   #### close

            ``` methodSignature
            public void close()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `Closeable`
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

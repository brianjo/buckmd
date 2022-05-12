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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.counters](package-summary.html)
:::

## Interface CounterRegistry {#interface-counterregistry .title title="Interface CounterRegistry"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `AutoCloseable`, `Closeable`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `CounterRegistryImpl`

    ------------------------------------------------------------------------

        public interface CounterRegistry
        extends Closeable
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Interface                                         Description
          ------------------- ------------------------------------------------- -------------
          `static class `     `CounterRegistry.AsyncCounterRegistrationEvent`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                                                                               Description
          ------------------- ---------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `IntegerCounter`    `newIntegerCounter​(String category,                  String name,                  com.google.common.collect.ImmutableMap<String,​String> tags)`       
          `SamplingCounter`   `newSamplingCounter​(String category,                   String name,                   com.google.common.collect.ImmutableMap<String,​String> tags)`    
          `TagSetCounter`     `newTagSetCounter​(String category,                 String name,                 com.google.common.collect.ImmutableMap<String,​String> tags)`          
          `void`              `registerCounters​(CounterRegistry.AsyncCounterRegistrationEvent event)`                                                                               
          `void`              `registerCounters​(Collection<Counter> counters)`                                                                                                      

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

        -   []{#methods.inherited.from.class.java.io.Closeable}

            ### Methods inherited from interface java.io.[Closeable](http://docs.oracle.com/javase/7/docs/api/java/io/Closeable.html?is-external=true "class or interface in java.io"){.externalLink}

            `close`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#newIntegerCounter(java.lang.String,java.lang.String,com.google.common.collect.ImmutableMap)}

        -   #### newIntegerCounter

            ``` methodSignature
            IntegerCounter newIntegerCounter​(String category,
                                             String name,
                                             com.google.common.collect.ImmutableMap<String,​String> tags)
            ```

        []{#newSamplingCounter(java.lang.String,java.lang.String,com.google.common.collect.ImmutableMap)}

        -   #### newSamplingCounter

            ``` methodSignature
            SamplingCounter newSamplingCounter​(String category,
                                               String name,
                                               com.google.common.collect.ImmutableMap<String,​String> tags)
            ```

        []{#newTagSetCounter(java.lang.String,java.lang.String,com.google.common.collect.ImmutableMap)}

        -   #### newTagSetCounter

            ``` methodSignature
            TagSetCounter newTagSetCounter​(String category,
                                           String name,
                                           com.google.common.collect.ImmutableMap<String,​String> tags)
            ```

        []{#registerCounters(java.util.Collection)}

        -   #### registerCounters

            ``` methodSignature
            void registerCounters​(Collection<Counter> counters)
            ```

        []{#registerCounters(com.facebook.buck.counters.CounterRegistry.AsyncCounterRegistrationEvent)}

        -   #### registerCounters

            ``` methodSignature
            void registerCounters​(CounterRegistry.AsyncCounterRegistrationEvent event)
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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

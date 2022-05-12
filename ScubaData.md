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
[Package]{.packageLabelInType} [com.facebook.buck.event](package-summary.html)
:::

## Class ScubaData {#class-scubadata .title title="Class ScubaData"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.event.ScubaData

::: description
-   

    ------------------------------------------------------------------------

        public abstract class ScubaData
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                 Description
          ------------------- --------------------- -------------
          `static class `     `ScubaData.Builder`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor     Description
          --------------- -------------
          `ScubaData()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                          Method                                                                  Description
          -------------------------------------------------------------------------- ----------------------------------------------------------------------- -------------
          `static void`                                                              `addScubaData​(ScubaData.Builder builder,             ScubaData data)`    
          `static ScubaData.Builder`                                                 `builder()`                                                              
          `static ScubaData.Builder`                                                 `builder​(ScubaData data)`                                                
          `abstract com.google.common.collect.ImmutableMap<String,​Long>`             `getInts()`                                                              
          `abstract com.google.common.collect.ImmutableMap<String,​String>`           `getNormals()`                                                           
          `abstract com.google.common.collect.ImmutableSetMultimap<String,​String>`   `getTags()`                                                              
          `static ScubaData`                                                         `of()`                                                                   

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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### ScubaData

                public ScubaData()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getInts()}

        -   #### getInts

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableMap<String,​Long> getInts()
            ```

        []{#getNormals()}

        -   #### getNormals

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableMap<String,​String> getNormals()
            ```

        []{#getTags()}

        -   #### getTags

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSetMultimap<String,​String> getTags()
            ```

        []{#addScubaData(com.facebook.buck.event.ScubaData.Builder,com.facebook.buck.event.ScubaData)}

        -   #### addScubaData

            ``` methodSignature
            public static void addScubaData​(ScubaData.Builder builder,
                                            ScubaData data)
            ```

        []{#builder(com.facebook.buck.event.ScubaData)}

        -   #### builder

            ``` methodSignature
            public static ScubaData.Builder builder​(ScubaData data)
            ```

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static ScubaData.Builder builder()
            ```

        []{#of()}

        -   #### of

            ``` methodSignature
            public static ScubaData of()
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

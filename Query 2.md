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
[Package]{.packageLabelInType} [com.facebook.buck.rules.query](package-summary.html)
:::

## Class Query {#class-query .title title="Class Query"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.query.Query

::: description
-   

    ------------------------------------------------------------------------

        public abstract class Query
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor   Description
          ------------- -------------
          `Query()`      

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                      Method                                                                                           Description
          ---------------------------------------------------------------------- ------------------------------------------------------------------------------------------------ -------------
          `abstract BaseName`                                                    `getBaseName()`                                                                                   
          `abstract String`                                                      `getQuery()`                                                                                      
          `abstract com.google.common.collect.ImmutableSortedSet<BuildTarget>`   `getResolvedQuery()`                                                                              
          `abstract TargetConfiguration`                                         `getTargetConfiguration()`                                                                        
          `static Query`                                                         `of​(String query,   TargetConfiguration targetConfiguration,   BaseName baseName)`                
          `Query`                                                                `withQuery​(String query)`                                                                         
          `Query`                                                                `withResolvedQuery​(com.google.common.collect.ImmutableSortedSet<BuildTarget> resolveDepQuery)`    

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

        -   #### Query

                public Query()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getQuery()}

        -   #### getQuery

            ``` methodSignature
            public abstract String getQuery()
            ```

        []{#getTargetConfiguration()}

        -   #### getTargetConfiguration

            ``` methodSignature
            public abstract TargetConfiguration getTargetConfiguration()
            ```

        []{#getBaseName()}

        -   #### getBaseName

            ``` methodSignature
            public abstract BaseName getBaseName()
            ```

        []{#getResolvedQuery()}

        -   #### getResolvedQuery

            ``` methodSignature
            @Nullable
            @NaturalOrder
            public abstract com.google.common.collect.ImmutableSortedSet<BuildTarget> getResolvedQuery()
            ```

        []{#of(java.lang.String,com.facebook.buck.core.model.TargetConfiguration,com.facebook.buck.core.model.BaseName)}

        -   #### of

            ``` methodSignature
            public static Query of​(String query,
                                   TargetConfiguration targetConfiguration,
                                   BaseName baseName)
            ```

        []{#withQuery(java.lang.String)}

        -   #### withQuery

            ``` methodSignature
            public Query withQuery​(String query)
            ```

        []{#withResolvedQuery(com.google.common.collect.ImmutableSortedSet)}

        -   #### withResolvedQuery

            ``` methodSignature
            public Query withResolvedQuery​(com.google.common.collect.ImmutableSortedSet<BuildTarget> resolveDepQuery)
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

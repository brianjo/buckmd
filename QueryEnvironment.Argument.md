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
[Package]{.packageLabelInType} [com.facebook.buck.query](package-summary.html)
:::

## Class QueryEnvironment.Argument\<ENV_NODE_TYPE\> {#class-queryenvironment.argumentenv_node_type .title title="Class QueryEnvironment.Argument"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.query.QueryEnvironment.Argument\<ENV_NODE_TYPE\>

::: description
-   

    [Type Parameters:]{.paramLabel}
    :   `ENV_NODE_TYPE` - If this argument represents an
        [`QueryEnvironment.ArgumentType.EXPRESSION`](QueryEnvironment.ArgumentType.html#EXPRESSION),
        determines the type of the
        [`QueryEnvironment`](QueryEnvironment.html "interface in com.facebook.buck.query")
        in which the expression is expected to be evaluated.

    ```{=html}
    <!-- -->
    ```

    Enclosing interface:
    :   [QueryEnvironment](QueryEnvironment.html "interface in com.facebook.buck.query")\<[NODE_TYPE](QueryEnvironment.html "type parameter in QueryEnvironment")\>

    ------------------------------------------------------------------------

        public static class QueryEnvironment.Argument<ENV_NODE_TYPE>
        extends Object

    ::: block
    Value of an argument of a user-defined query function.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                           Method                                          Description
          ------------------------------------------- ----------------------------------------------- -------------
          `boolean`                                   `equals​(Object other)`                           
          `boolean`                                   `equalTo​(QueryEnvironment.Argument<?> other)`    
          `QueryExpression<ENV_NODE_TYPE>`            `getExpression()`                                
          `int`                                       `getInteger()`                                   
          `QueryEnvironment.ArgumentType`             `getType()`                                      
          `String`                                    `getWord()`                                      
          `int`                                       `hashCode()`                                     
          `static QueryEnvironment.Argument<?>`       `of​(int integer)`                                
          `static <T> QueryEnvironment.Argument<T>`   `of​(QueryExpression<T> expression)`              
          `static QueryEnvironment.Argument<?>`       `of​(String word)`                                
          `String`                                    `toString()`                                     

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#of(com.facebook.buck.query.QueryExpression)}

        -   #### of

            ``` methodSignature
            public static <T> QueryEnvironment.Argument<T> of​(QueryExpression<T> expression)
            ```

        []{#of(java.lang.String)}

        -   #### of

            ``` methodSignature
            public static QueryEnvironment.Argument<?> of​(String word)
            ```

        []{#of(int)}

        -   #### of

            ``` methodSignature
            public static QueryEnvironment.Argument<?> of​(int integer)
            ```

        []{#getType()}

        -   #### getType

            ``` methodSignature
            public QueryEnvironment.ArgumentType getType()
            ```

        []{#getExpression()}

        -   #### getExpression

            ``` methodSignature
            public QueryExpression<ENV_NODE_TYPE> getExpression()
            ```

        []{#getWord()}

        -   #### getWord

            ``` methodSignature
            public String getWord()
            ```

        []{#getInteger()}

        -   #### getInteger

            ``` methodSignature
            public int getInteger()
            ```

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(Object other)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `Object`

        []{#equalTo(com.facebook.buck.query.QueryEnvironment.Argument)}

        -   #### equalTo

            ``` methodSignature
            public boolean equalTo​(QueryEnvironment.Argument<?> other)
            ```

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `Object`
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

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

## Class TargetLiteral\<NODE_TYPE\> {#class-targetliteralnode_type .title title="Class TargetLiteral"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.query.QueryExpression](QueryExpression.html "class in com.facebook.buck.query")\<NODE_TYPE\>

    -   -   com.facebook.buck.query.TargetLiteral\<NODE_TYPE\>

::: description
-   

    ------------------------------------------------------------------------

        public final class TargetLiteral<NODE_TYPE>
        extends QueryExpression<NODE_TYPE>

    ::: block
    A literal set of targets. (The syntax of the string \"pattern\"
    determines which.)
        expr ::= WORD
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `boolean`             | `eq                   | ::: block             |
        |                       | uals​(Object another)` | This instance is      |
        |                       |                       | equal to all          |
        |                       |                       | instances of          |
        |                       |                       | `TargetLiteral` that  |
        |                       |                       | have equal attribute  |
        |                       |                       | values.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `<OUTPUT_             | `eval​(QueryEvalua     |                       |
        | TYPE extends QueryTar | tor<NODE_TYPE> evalua |                       |
        | get>Set<OUTPUT_TYPE>` | tor,     QueryEnviron |                       |
        |                       | ment<NODE_TYPE> env)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getPattern()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `of​(String pattern)`  | ::: block             |
        | <T> TargetLiteral<T>` |                       | Construct a new       |
        |                       |                       | immutable             |
        |                       |                       | `TargetLiteral`       |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          | ::: block             |
        |                       |                       | Returns this query    |
        |                       |                       | expression            |
        |                       |                       | pretty-printed.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `traverse​(com.f       | ::: block             |
        |                       | acebook.buck.query.Qu | Accepts and applies   |
        |                       | eryExpression.Visitor | the given visitor.    |
        |                       | <NODE_TYPE> visitor)` | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.query.QueryExpression}

            ### Methods inherited from class com.facebook.buck.query.[QueryExpression](QueryExpression.html "class in com.facebook.buck.query")

            `collectTargetPatterns, getTargets, parse`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getPattern()}

        -   #### getPattern

            ``` methodSignature
            public String getPattern()
            ```

            [Returns:]{.returnLabel}
            :   The value of the `pattern` attribute

        []{#eval(com.facebook.buck.query.QueryEvaluator,com.facebook.buck.query.QueryEnvironment)}

        -   #### eval

            ``` methodSignature
            public <OUTPUT_TYPE extends QueryTarget> Set<OUTPUT_TYPE> eval​(QueryEvaluator<NODE_TYPE> evaluator,
                                                                           QueryEnvironment<NODE_TYPE> env)
                                                                    throws QueryException
            ```

            [Throws:]{.throwsLabel}
            :   `QueryException`

        []{#traverse(com.facebook.buck.query.QueryExpression.Visitor)}

        -   #### traverse

            ``` methodSignature
            public void traverse​(com.facebook.buck.query.QueryExpression.Visitor<NODE_TYPE> visitor)
            ```

            ::: block
            [Description copied from
            class: `QueryExpression`]{.descfrmTypeLabel}
            :::

            ::: block
            Accepts and applies the given visitor.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `traverse` in class `QueryExpression<NODE_TYPE>`

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            ::: block
            [Description copied from
            class: `QueryExpression`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns this query expression pretty-printed.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `toString` in class `QueryExpression<NODE_TYPE>`

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(@Nullable
                                  Object another)
            ```

            ::: block
            This instance is equal to all instances of `TargetLiteral`
            that have equal attribute values.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `Object`

            [Returns:]{.returnLabel}
            :   `true` if `this` is equal to `another` instance

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `Object`

        []{#of(java.lang.String)}

        -   #### of

            ``` methodSignature
            public static <T> TargetLiteral<T> of​(String pattern)
            ```

            ::: block
            Construct a new immutable `TargetLiteral` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `pattern` - The value for the `pattern` attribute

            [Returns:]{.returnLabel}
            :   An immutable TargetLiteral instance
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

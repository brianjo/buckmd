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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.query](package-summary.html)
:::

## Class QueryNormalizer {#class-querynormalizer .title title="Class QueryNormalizer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.query.QueryNormalizer

::: description
-   

    ------------------------------------------------------------------------

        public final class QueryNormalizer
        extends Object

    ::: block
    Translates raw query to its canonical view, replacing substitutions
    if needed
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Field                 | Description           |
        +=======================+=======================+=======================+
        | `static String`       | `SET_SEPARATOR`       | ::: block             |
        |                       |                       | String used to        |
        |                       |                       | separate distinct     |
        |                       |                       | sets when using       |
        |                       |                       | \`%Ss\` in a query    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `SET_SUBSTITUTOR`     | ::: block             |
        |                       |                       | String used to        |
        |                       |                       | specify a             |
        |                       |                       | substitution location |
        |                       |                       | of a set which is     |
        |                       |                       | specified as a list   |
        |                       |                       | of newline-separated  |
        |                       |                       | strings which follow  |
        |                       |                       | the query itself      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor           Description
          --------------------- -------------
          `QueryNormalizer()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static String`       | `nor                  | ::: block             |
        |                       | malize​(String query)` | Format query using    |
        |                       |                       | list substitution If  |
        |                       |                       | the first line of the |
        |                       |                       | query contains %Ss    |
        |                       |                       | then subsequent lines |
        |                       |                       | are treated as        |
        |                       |                       | replacement strings   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `normalizePa          | ::: block             |
        |                       | ttern​(String pattern, | Format query using    |
        |                       |                  List | list substitution     |
        |                       | <String> formatArgs)` | :::                   |
        +-----------------------+-----------------------+-----------------------+

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

        []{#SET_SEPARATOR}

        -   #### SET_SEPARATOR

                public static final String SET_SEPARATOR

            ::: block
            String used to separate distinct sets when using \`%Ss\` in
            a query
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.query.QueryNormalizer.SET_SEPARATOR)

        []{#SET_SUBSTITUTOR}

        -   #### SET_SUBSTITUTOR

                public static final String SET_SUBSTITUTOR

            ::: block
            String used to specify a substitution location of a set
            which is specified as a list of newline-separated strings
            which follow the query itself
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.query.QueryNormalizer.SET_SUBSTITUTOR)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### QueryNormalizer

                public QueryNormalizer()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#normalizePattern(java.lang.String,java.util.List)}

        -   #### normalizePattern

            ``` methodSignature
            public static String normalizePattern​(String pattern,
                                                  List<String> formatArgs)
                                           throws QueryException
            ```

            ::: block
            Format query using list substitution
            :::

            [Parameters:]{.paramLabel}
            :   `pattern` - Query that contains one or more %Ss
            :   `formatArgs` - Replacement strings for each %Ss
                occurrence, if there is just on replacement then all %sS
                instance would be replaced with it. If there is another
                mismatch between number of %Ss and replacement strings
                then the error is raised

            [Throws:]{.throwsLabel}
            :   `QueryException`

        []{#normalize(java.lang.String)}

        -   #### normalize

            ``` methodSignature
            public static String normalize​(String query)
                                    throws QueryException
            ```

            ::: block
            Format query using list substitution If the first line of
            the query contains %Ss then subsequent lines are treated as
            replacement strings
            :::

            [Throws:]{.throwsLabel}
            :   `QueryException`
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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

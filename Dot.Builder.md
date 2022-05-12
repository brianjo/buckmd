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
[Package]{.packageLabelInType} [com.facebook.buck.cli](package-summary.html)
:::

## Class Dot.Builder\<T\> {#class-dot.buildert .title title="Class Dot.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cli.Dot.Builder\<T\>

::: description
-   

    [Type Parameters:]{.paramLabel}
    :   `T` -

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [Dot](Dot.html "class in com.facebook.buck.cli")\<[T](Dot.html "type parameter in Dot")\>

    ------------------------------------------------------------------------

        public static class Dot.Builder<T>
        extends Object

    ::: block
    Builder class for Dot output
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Dot<T>`              | `build()`             |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Dot.Builder<T>`      | `setCompac            |                       |
        |                       | tMode​(boolean value)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Dot.Builder<T>`      | `setNodesToFil        |                       |
        |                       | ter​(java.util.functio |                       |
        |                       | n.Predicate<T> pred)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Dot.Builder<T>`      | `setNodeToAtt         | ::: block             |
        |                       | ributes​(java.util.fun | Configures a function |
        |                       | ction.Function<T,​com. | to be used to extract |
        |                       | google.common.collect | additional attributes |
        |                       | .ImmutableSortedMap<S | to include when       |
        |                       | tring,​String>> func)` | rendering graph       |
        |                       |                       | nodes.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Dot.Builder<T>`      | `setNodeToName​(ja     |                       |
        |                       | va.util.function.Func |                       |
        |                       | tion<T,​String> func)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Dot.Builder<T>`      | `setNodeToTypeName​(ja |                       |
        |                       | va.util.function.Func |                       |
        |                       | tion<T,​String> func)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Dot.Builder<T>`      | `se                   |                       |
        |                       | tOutputOrder​(Dot.Outp |                       |
        |                       | utOrder outputOrder)` |                       |
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
    -   []{#method.detail}

        ### Method Detail

        []{#setNodeToName(java.util.function.Function)}

        -   #### setNodeToName

            ``` methodSignature
            public Dot.Builder<T> setNodeToName​(java.util.function.Function<T,​String> func)
            ```

        []{#setNodeToTypeName(java.util.function.Function)}

        -   #### setNodeToTypeName

            ``` methodSignature
            public Dot.Builder<T> setNodeToTypeName​(java.util.function.Function<T,​String> func)
            ```

        []{#setOutputOrder(com.facebook.buck.cli.Dot.OutputOrder)}

        -   #### setOutputOrder

            ``` methodSignature
            public Dot.Builder<T> setOutputOrder​(Dot.OutputOrder outputOrder)
            ```

        []{#setNodesToFilter(java.util.function.Predicate)}

        -   #### setNodesToFilter

            ``` methodSignature
            public Dot.Builder<T> setNodesToFilter​(java.util.function.Predicate<T> pred)
            ```

        []{#setCompactMode(boolean)}

        -   #### setCompactMode

            ``` methodSignature
            public Dot.Builder<T> setCompactMode​(boolean value)
            ```

        []{#setNodeToAttributes(java.util.function.Function)}

        -   #### setNodeToAttributes

            ``` methodSignature
            public Dot.Builder<T> setNodeToAttributes​(java.util.function.Function<T,​com.google.common.collect.ImmutableSortedMap<String,​String>> func)
            ```

            ::: block
            Configures a function to be used to extract additional
            attributes to include when rendering graph nodes.
            In order ot prevent collisions, all attribute names are
            prefixed with `buck_`. They are also escaped in order to be
            compatible with the [Dot
            format](https://graphviz.gitlab.io/_pages/doc/info/lang.html).
            :::

        []{#build()}

        -   #### build

            ``` methodSignature
            public Dot<T> build()
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

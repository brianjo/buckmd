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
[Package]{.packageLabelInType} [com.facebook.buck.util.json](package-summary.html)
:::

## Class JsonBuilder {#class-jsonbuilder .title title="Class JsonBuilder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.json.JsonBuilder

::: description
-   

    ------------------------------------------------------------------------

        public class JsonBuilder
        extends Object

    ::: block
    Fluent API for constructing a JSON string.
    For example, `{"a": {"b": true, "c": [1.0,2.0,3.0]}}` can be written
    as:

         JsonBuilder.object()
           .addObject(
             "a",
             JsonBuilder.object()
               .addBoolean("b", true)
               .addArray("c", JsonBuilder.array().addNumber(1.0).addNumber(2.0).addNumber(3.0)))
           .toString();
         
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `Json                 | ::: block             |
        |                       | Builder.ArrayBuilder` | Builder for a JSON    |
        |                       |                       | array string.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `JsonB                | ::: block             |
        |                       | uilder.ObjectBuilder` | Builder for a JSON    |
        |                       |                       | object string.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static Json          | `array()`             | ::: block             |
        | Builder.ArrayBuilder` |                       | Creates a builder for |
        |                       |                       | a JSON array string.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Json          | `arrayOfDoubl         |                       |
        | Builder.ArrayBuilder` | es​(java.util.stream.D |                       |
        |                       | oubleStream numbers)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static JsonB         | `object()`            | ::: block             |
        | uilder.ObjectBuilder` |                       | Creates a builder for |
        |                       |                       | a JSON object string. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `toArray​(java.ut      |                       |
        | <T> java.util.stream. | il.function.BiConsume |                       |
        | Collector<T,​JsonBuild | r<JsonBuilder.ArrayBu |                       |
        | er.ArrayBuilder,​JsonB | ilder,​T> accumulate)` |                       |
        | uilder.ArrayBuilder>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `toArrayOfArrays()`   |                       |
        | tic java.util.stream. |                       |                       |
        | Collector<JsonBuilder |                       |                       |
        | .ArrayBuilder,​?,​JsonB |                       |                       |
        | uilder.ArrayBuilder>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `stat                 | `toArrayOfObjects()`  |                       |
        | ic java.util.stream.C |                       |                       |
        | ollector<JsonBuilder. |                       |                       |
        | ObjectBuilder,​?,​JsonB |                       |                       |
        | uilder.ArrayBuilder>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `toArrayOfStrings()`  |                       |
        |  java.util.stream.Col |                       |                       |
        | lector<String,​?,​JsonB |                       |                       |
        | uilder.ArrayBuilder>` |                       |                       |
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
    -   []{#method.detail}

        ### Method Detail

        []{#array()}

        -   #### array

            ``` methodSignature
            public static JsonBuilder.ArrayBuilder array()
            ```

            ::: block
            Creates a builder for a JSON array string.
            :::

        []{#object()}

        -   #### object

            ``` methodSignature
            public static JsonBuilder.ObjectBuilder object()
            ```

            ::: block
            Creates a builder for a JSON object string.
            :::

        []{#arrayOfDoubles(java.util.stream.DoubleStream)}

        -   #### arrayOfDoubles

            ``` methodSignature
            public static JsonBuilder.ArrayBuilder arrayOfDoubles​(java.util.stream.DoubleStream numbers)
            ```

        []{#toArrayOfStrings()}

        -   #### toArrayOfStrings

            ``` methodSignature
            public static java.util.stream.Collector<String,​?,​JsonBuilder.ArrayBuilder> toArrayOfStrings()
            ```

        []{#toArrayOfArrays()}

        -   #### toArrayOfArrays

            ``` methodSignature
            public static java.util.stream.Collector<JsonBuilder.ArrayBuilder,​?,​JsonBuilder.ArrayBuilder> toArrayOfArrays()
            ```

        []{#toArrayOfObjects()}

        -   #### toArrayOfObjects

            ``` methodSignature
            public static java.util.stream.Collector<JsonBuilder.ObjectBuilder,​?,​JsonBuilder.ArrayBuilder> toArrayOfObjects()
            ```

        []{#toArray(java.util.function.BiConsumer)}

        -   #### toArray

            ``` methodSignature
            public static <T> java.util.stream.Collector<T,​JsonBuilder.ArrayBuilder,​JsonBuilder.ArrayBuilder> toArray​(java.util.function.BiConsumer<JsonBuilder.ArrayBuilder,​T> accumulate)
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

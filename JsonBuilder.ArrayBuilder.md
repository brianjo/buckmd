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

## Class JsonBuilder.ArrayBuilder {#class-jsonbuilder.arraybuilder .title title="Class JsonBuilder.ArrayBuilder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.json.JsonBuilder.ArrayBuilder

::: description
-   

    Enclosing class:
    :   [JsonBuilder](JsonBuilder.html "class in com.facebook.buck.util.json")

    ------------------------------------------------------------------------

        public static class JsonBuilder.ArrayBuilder
        extends Object

    ::: block
    Builder for a JSON array string.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Json                 | `a                    | ::: block             |
        | Builder.ArrayBuilder` | ddArray​(JsonBuilder.A | Adds a nested JSON    |
        |                       | rrayBuilder builder)` | array to the array.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Json                 | `addBo                | ::: block             |
        | Builder.ArrayBuilder` | olean​(boolean value)` | Adds a boolean value  |
        |                       |                       | to the array.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Json                 | `addBoolean​(Optional< | ::: block             |
        | Builder.ArrayBuilder` | Boolean> maybeValue)` | Adds a boolean value  |
        |                       |                       | to the array, or      |
        |                       |                       | \'null\' if not       |
        |                       |                       | present.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Json                 | `addNull()`           | ::: block             |
        | Builder.ArrayBuilder` |                       | Adds a \'null\' value |
        |                       |                       | to the array.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Json                 | `add                  | ::: block             |
        | Builder.ArrayBuilder` | Number​(double value)` | Adds a numeric value  |
        |                       |                       | to the array.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Json                 | `addNumber​(Optional   | ::: block             |
        | Builder.ArrayBuilder` | <Double> maybeValue)` | Adds a numeric value  |
        |                       |                       | to the array, or      |
        |                       |                       | \'null\' if not       |
        |                       |                       | present.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Json                 | `add                  | ::: block             |
        | Builder.ArrayBuilder` | Object​(JsonBuilder.Ob | Adds a nested JSON    |
        |                       | jectBuilder builder)` | object to the array.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Json                 | `add                  | ::: block             |
        | Builder.ArrayBuilder` | Raw​(String rawValue)` | Adds a raw JSON value |
        |                       |                       | to the array.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Json                 | `addRaw​(Optional<St   | ::: block             |
        | Builder.ArrayBuilder` | ring> maybeRawValue)` | Adds a raw JSON value |
        |                       |                       | to the array, or      |
        |                       |                       | \'null\' if not       |
        |                       |                       | present.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Json                 | `add                  | ::: block             |
        | Builder.ArrayBuilder` | String​(String value)` | Adds a string to the  |
        |                       |                       | array.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Json                 | `addString​(Optional   | ::: block             |
        | Builder.ArrayBuilder` | <String> maybeValue)` | Adds a string to the  |
        |                       |                       | array, or \'null\' if |
        |                       |                       | not present.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Json                 | `merge​(JsonBuilder    | ::: block             |
        | Builder.ArrayBuilder` | .ArrayBuilder other)` | Merges two            |
        |                       |                       | ArrayBuilders.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#addNull()}

        -   #### addNull

            ``` methodSignature
            public JsonBuilder.ArrayBuilder addNull()
            ```

            ::: block
            Adds a \'null\' value to the array.
            :::

        []{#addBoolean(boolean)}

        -   #### addBoolean

            ``` methodSignature
            public JsonBuilder.ArrayBuilder addBoolean​(boolean value)
            ```

            ::: block
            Adds a boolean value to the array.
            :::

        []{#addBoolean(java.util.Optional)}

        -   #### addBoolean

            ``` methodSignature
            public JsonBuilder.ArrayBuilder addBoolean​(Optional<Boolean> maybeValue)
            ```

            ::: block
            Adds a boolean value to the array, or \'null\' if not
            present.
            :::

        []{#addNumber(double)}

        -   #### addNumber

            ``` methodSignature
            public JsonBuilder.ArrayBuilder addNumber​(double value)
            ```

            ::: block
            Adds a numeric value to the array.
            :::

        []{#addNumber(java.util.Optional)}

        -   #### addNumber

            ``` methodSignature
            public JsonBuilder.ArrayBuilder addNumber​(Optional<Double> maybeValue)
            ```

            ::: block
            Adds a numeric value to the array, or \'null\' if not
            present.
            :::

        []{#addString(java.lang.String)}

        -   #### addString

            ``` methodSignature
            public JsonBuilder.ArrayBuilder addString​(String value)
            ```

            ::: block
            Adds a string to the array.
            :::

        []{#addString(java.util.Optional)}

        -   #### addString

            ``` methodSignature
            public JsonBuilder.ArrayBuilder addString​(Optional<String> maybeValue)
            ```

            ::: block
            Adds a string to the array, or \'null\' if not present.
            :::

        []{#addObject(com.facebook.buck.util.json.JsonBuilder.ObjectBuilder)}

        -   #### addObject

            ``` methodSignature
            public JsonBuilder.ArrayBuilder addObject​(JsonBuilder.ObjectBuilder builder)
            ```

            ::: block
            Adds a nested JSON object to the array.
            :::

        []{#addArray(com.facebook.buck.util.json.JsonBuilder.ArrayBuilder)}

        -   #### addArray

            ``` methodSignature
            public JsonBuilder.ArrayBuilder addArray​(JsonBuilder.ArrayBuilder builder)
            ```

            ::: block
            Adds a nested JSON array to the array.
            :::

        []{#addRaw(java.lang.String)}

        -   #### addRaw

            ``` methodSignature
            public JsonBuilder.ArrayBuilder addRaw​(String rawValue)
            ```

            ::: block
            Adds a raw JSON value to the array.
            :::

        []{#addRaw(java.util.Optional)}

        -   #### addRaw

            ``` methodSignature
            public JsonBuilder.ArrayBuilder addRaw​(Optional<String> maybeRawValue)
            ```

            ::: block
            Adds a raw JSON value to the array, or \'null\' if not
            present.
            :::

        []{#merge(com.facebook.buck.util.json.JsonBuilder.ArrayBuilder)}

        -   #### merge

            ``` methodSignature
            public JsonBuilder.ArrayBuilder merge​(JsonBuilder.ArrayBuilder other)
            ```

            ::: block
            Merges two ArrayBuilders. Necessary for Collectors. This
            *should* never be called when collecting streams, as the
            provided `Collector` instances are not concurrent.
            :::
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

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

## Class JsonBuilder.ObjectBuilder {#class-jsonbuilder.objectbuilder .title title="Class JsonBuilder.ObjectBuilder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.json.JsonBuilder.ObjectBuilder

::: description
-   

    Enclosing class:
    :   [JsonBuilder](JsonBuilder.html "class in com.facebook.buck.util.json")

    ------------------------------------------------------------------------

        public static class JsonBuilder.ObjectBuilder
        extends Object

    ::: block
    Builder for a JSON object string.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `JsonB                | `addArr               | ::: block             |
        | uilder.ObjectBuilder` | ay​(String fieldName,  | Adds a nested JSON    |
        |                       |         JsonBuilder.A | array to the object.  |
        |                       | rrayBuilder builder)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsonB                | `addBoolean​(S         | ::: block             |
        | uilder.ObjectBuilder` | tring fieldName,      | Adds a boolean value  |
        |                       |       boolean value)` | to the object.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsonB                | `addBoo               | ::: block             |
        | uilder.ObjectBuilder` | lean​(String fieldName | Adds a boolean value  |
        |                       | ,           Optional< | to the object, if     |
        |                       | Boolean> maybeValue)` | present.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsonB                | `addNu                | ::: block             |
        | uilder.ObjectBuilder` | ll​(String fieldName)` | Adds a \'null\' value |
        |                       |                       | to the object.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsonB                | `addNumber            | ::: block             |
        | uilder.ObjectBuilder` | ​(String fieldName,    | Adds a numeric value  |
        |                       |        double value)` | to the object.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsonB                | `add                  | ::: block             |
        | uilder.ObjectBuilder` | Number​(String fieldNa | Adds a numeric value  |
        |                       | me,          Optional | to the object, if     |
        |                       | <Double> maybeValue)` | present.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsonB                | `addObject            | ::: block             |
        | uilder.ObjectBuilder` | ​(String fieldName,    | Adds a nested JSON    |
        |                       |        JsonBuilder.Ob | object to the object. |
        |                       | jectBuilder builder)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsonB                | `addRaw               | ::: block             |
        | uilder.ObjectBuilder` | ​(String fieldName,    | Adds a raw JSON value |
        |                       |     String rawValue)` | to the object.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsonB                | `                     | ::: block             |
        | uilder.ObjectBuilder` | addRaw​(String fieldNa | Adds a raw JSON value |
        |                       | me,       Optional<St | to the object, if     |
        |                       | ring> maybeRawValue)` | present.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsonB                | `addString            | ::: block             |
        | uilder.ObjectBuilder` | ​(String fieldName,    | Adds a string to the  |
        |                       |        String value)` | object.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsonB                | `add                  | ::: block             |
        | uilder.ObjectBuilder` | String​(String fieldNa | Adds a string to the  |
        |                       | me,          Optional | object, if present.   |
        |                       | <String> maybeValue)` | :::                   |
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

        []{#addNull(java.lang.String)}

        -   #### addNull

            ``` methodSignature
            public JsonBuilder.ObjectBuilder addNull​(String fieldName)
            ```

            ::: block
            Adds a \'null\' value to the object.
            :::

        []{#addBoolean(java.lang.String,boolean)}

        -   #### addBoolean

            ``` methodSignature
            public JsonBuilder.ObjectBuilder addBoolean​(String fieldName,
                                                        boolean value)
            ```

            ::: block
            Adds a boolean value to the object.
            :::

        []{#addBoolean(java.lang.String,java.util.Optional)}

        -   #### addBoolean

            ``` methodSignature
            public JsonBuilder.ObjectBuilder addBoolean​(String fieldName,
                                                        Optional<Boolean> maybeValue)
            ```

            ::: block
            Adds a boolean value to the object, if present.
            :::

        []{#addNumber(java.lang.String,double)}

        -   #### addNumber

            ``` methodSignature
            public JsonBuilder.ObjectBuilder addNumber​(String fieldName,
                                                       double value)
            ```

            ::: block
            Adds a numeric value to the object.
            :::

        []{#addNumber(java.lang.String,java.util.Optional)}

        -   #### addNumber

            ``` methodSignature
            public JsonBuilder.ObjectBuilder addNumber​(String fieldName,
                                                       Optional<Double> maybeValue)
            ```

            ::: block
            Adds a numeric value to the object, if present.
            :::

        []{#addString(java.lang.String,java.lang.String)}

        -   #### addString

            ``` methodSignature
            public JsonBuilder.ObjectBuilder addString​(String fieldName,
                                                       String value)
            ```

            ::: block
            Adds a string to the object.
            :::

        []{#addString(java.lang.String,java.util.Optional)}

        -   #### addString

            ``` methodSignature
            public JsonBuilder.ObjectBuilder addString​(String fieldName,
                                                       Optional<String> maybeValue)
            ```

            ::: block
            Adds a string to the object, if present.
            :::

        []{#addObject(java.lang.String,com.facebook.buck.util.json.JsonBuilder.ObjectBuilder)}

        -   #### addObject

            ``` methodSignature
            public JsonBuilder.ObjectBuilder addObject​(String fieldName,
                                                       JsonBuilder.ObjectBuilder builder)
            ```

            ::: block
            Adds a nested JSON object to the object.
            :::

        []{#addArray(java.lang.String,com.facebook.buck.util.json.JsonBuilder.ArrayBuilder)}

        -   #### addArray

            ``` methodSignature
            public JsonBuilder.ObjectBuilder addArray​(String fieldName,
                                                      JsonBuilder.ArrayBuilder builder)
            ```

            ::: block
            Adds a nested JSON array to the object.
            :::

        []{#addRaw(java.lang.String,java.lang.String)}

        -   #### addRaw

            ``` methodSignature
            public JsonBuilder.ObjectBuilder addRaw​(String fieldName,
                                                    String rawValue)
            ```

            ::: block
            Adds a raw JSON value to the object.
            :::

        []{#addRaw(java.lang.String,java.util.Optional)}

        -   #### addRaw

            ``` methodSignature
            public JsonBuilder.ObjectBuilder addRaw​(String fieldName,
                                                    Optional<String> maybeRawValue)
            ```

            ::: block
            Adds a raw JSON value to the object, if present.
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

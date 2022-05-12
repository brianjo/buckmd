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
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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

## Class ObjectMappers {#class-objectmappers .title title="Class ObjectMappers"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.json.ObjectMappers

::: description
-   

    ------------------------------------------------------------------------

        public class ObjectMappers
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Field                 | Description           |
        +=======================+=======================+=======================+
        | `static co            | `READER`              |                       |
        | m.fasterxml.jackson.d |                       |                       |
        | atabind.ObjectReader` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static co            | `READER_INTERNED`     | ::: block             |
        | m.fasterxml.jackson.d |                       | ObjectReader that     |
        | atabind.ObjectReader` |                       | interns custom        |
        |                       |                       | objects on            |
        |                       |                       | serialization, like   |
        |                       |                       | Un                    |
        |                       |                       | configuredBuildTarget |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static co            | `READER_WITH_TYPE`    | ::: block             |
        | m.fasterxml.jackson.d |                       | ObjectReader that     |
        | atabind.ObjectReader` |                       | deserializes objects  |
        |                       |                       | that had type         |
        |                       |                       | information preserved |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static co            | `WRITER`              |                       |
        | m.fasterxml.jackson.d |                       |                       |
        | atabind.ObjectWriter` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static co            | `WRITER_WITH_TYPE`    | ::: block             |
        | m.fasterxml.jackson.d |                       | ObjectWrite that      |
        | atabind.ObjectWriter` |                       | serializes objects    |
        |                       |                       | along with their type |
        |                       |                       | information           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static <T> T`        | `co                   |                       |
        |                       | nvertValue​(Map<String |                       |
        |                       | ,​Object> map,         |                       |
        |                       |      Class<T> clazz)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `createGenerator​(     |                       |
        |  com.fasterxml.jackso | OutputStream stream)` |                       |
        | n.core.JsonGenerator` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `creat                |                       |
        | tic com.fasterxml.jac | eParser​(byte[] json)` |                       |
        | kson.core.JsonParser` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `createParser         |                       |
        | tic com.fasterxml.jac | ​(InputStream stream)` |                       |
        | kson.core.JsonParser` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `createP              |                       |
        | tic com.fasterxml.jac | arser​(Reader reader)` |                       |
        | kson.core.JsonParser` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `creat                |                       |
        | tic com.fasterxml.jac | eParser​(String json)` |                       |
        | kson.core.JsonParser` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `cre                  |                       |
        | tic com.fasterxml.jac | ateParser​(Path path)` |                       |
        | kson.core.JsonParser` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static co            | `createWithE          | ::: block             |
        | m.fasterxml.jackson.d | mptyBeansPermitted()` | Creates an            |
        | atabind.ObjectMapper` |                       | `ObjectMapper` that   |
        |                       |                       | allows to use objects |
        |                       |                       | without fields.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `fromJsonFun          |                       |
        | <T> java.util.functio | ction​(Class<T> type)` |                       |
        | n.Function<String,​T>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static co            | `legacyCreate()`      |                       |
        | m.fasterxml.jackson.d |                       |                       |
        | atabind.ObjectMapper` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static <T> T`        | `read                 |                       |
        |                       | Value​(String json,    |                       |
        |                       |        com.fasterxml. |                       |
        |                       | jackson.core.type.Typ |                       |
        |                       | eReference<T> clazz)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static <T> T`        | `readVa               |                       |
        |                       | lue​(String json,      |                       |
        |                       |      Class<T> clazz)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static <T> T`        | `re                   |                       |
        |                       | adValue​(Path file,    |                       |
        |                       |        com.fasterxml. |                       |
        |                       | jackson.core.type.Typ |                       |
        |                       | eReference<T> clazz)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static <T> T`        | `read                 |                       |
        |                       | Value​(Path file,      |                       |
        |                       |      Class<T> clazz)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `toJsonFunction()`    |                       |
        | <T> java.util.functio |                       |                       |
        | n.Function<T,​String>` |                       |                       |
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

        []{#READER}

        -   #### READER

                public static final com.fasterxml.jackson.databind.ObjectReader READER

        []{#WRITER}

        -   #### WRITER

                public static final com.fasterxml.jackson.databind.ObjectWriter WRITER

        []{#READER_WITH_TYPE}

        -   #### READER_WITH_TYPE

                public static final com.fasterxml.jackson.databind.ObjectReader READER_WITH_TYPE

            ::: block
            ObjectReader that deserializes objects that had type
            information preserved
            :::

        []{#WRITER_WITH_TYPE}

        -   #### WRITER_WITH_TYPE

                public static final com.fasterxml.jackson.databind.ObjectWriter WRITER_WITH_TYPE

            ::: block
            ObjectWrite that serializes objects along with their type
            information
            :::

        []{#READER_INTERNED}

        -   #### READER_INTERNED

                public static final com.fasterxml.jackson.databind.ObjectReader READER_INTERNED

            ::: block
            ObjectReader that interns custom objects on serialization,
            like UnconfiguredBuildTarget
            :::
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#readValue(java.nio.file.Path,java.lang.Class)}

        -   #### readValue

            ``` methodSignature
            public static <T> T readValue​(Path file,
                                          Class<T> clazz)
                                   throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#readValue(java.nio.file.Path,com.fasterxml.jackson.core.type.TypeReference)}

        -   #### readValue

            ``` methodSignature
            public static <T> T readValue​(Path file,
                                          com.fasterxml.jackson.core.type.TypeReference<T> clazz)
                                   throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#readValue(java.lang.String,java.lang.Class)}

        -   #### readValue

            ``` methodSignature
            public static <T> T readValue​(String json,
                                          Class<T> clazz)
                                   throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#readValue(java.lang.String,com.fasterxml.jackson.core.type.TypeReference)}

        -   #### readValue

            ``` methodSignature
            public static <T> T readValue​(String json,
                                          com.fasterxml.jackson.core.type.TypeReference<T> clazz)
                                   throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#createParser(java.nio.file.Path)}

        -   #### createParser

            ``` methodSignature
            public static com.fasterxml.jackson.core.JsonParser createParser​(Path path)
                                                                      throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#createParser(java.lang.String)}

        -   #### createParser

            ``` methodSignature
            public static com.fasterxml.jackson.core.JsonParser createParser​(String json)
                                                                      throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#createParser(byte[])}

        -   #### createParser

            ``` methodSignature
            public static com.fasterxml.jackson.core.JsonParser createParser​(byte[] json)
                                                                      throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#createParser(java.io.InputStream)}

        -   #### createParser

            ``` methodSignature
            public static com.fasterxml.jackson.core.JsonParser createParser​(InputStream stream)
                                                                      throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#createParser(java.io.Reader)}

        -   #### createParser

            ``` methodSignature
            public static com.fasterxml.jackson.core.JsonParser createParser​(Reader reader)
                                                                      throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#createGenerator(java.io.OutputStream)}

        -   #### createGenerator

            ``` methodSignature
            public static com.fasterxml.jackson.core.JsonGenerator createGenerator​(OutputStream stream)
                                                                            throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#convertValue(java.util.Map,java.lang.Class)}

        -   #### convertValue

            ``` methodSignature
            public static <T> T convertValue​(Map<String,​Object> map,
                                             Class<T> clazz)
            ```

        []{#toJsonFunction()}

        -   #### toJsonFunction

            ``` methodSignature
            public static <T> java.util.function.Function<T,​String> toJsonFunction()
            ```

        []{#fromJsonFunction(java.lang.Class)}

        -   #### fromJsonFunction

            ``` methodSignature
            public static <T> java.util.function.Function<String,​T> fromJsonFunction​(Class<T> type)
            ```

        []{#legacyCreate()}

        -   #### legacyCreate

            ``` methodSignature
            public static com.fasterxml.jackson.databind.ObjectMapper legacyCreate()
            ```

        []{#createWithEmptyBeansPermitted()}

        -   #### createWithEmptyBeansPermitted

            ``` methodSignature
            public static com.fasterxml.jackson.databind.ObjectMapper createWithEmptyBeansPermitted()
            ```

            ::: block
            Creates an `ObjectMapper` that allows to use objects without
            fields.
            :::

            [See Also:]{.seeLabel}
            :   `SerializationFeature.FAIL_ON_EMPTY_BEANS`
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
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

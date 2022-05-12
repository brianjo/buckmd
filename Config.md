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
[Package]{.packageLabelInType} [com.facebook.buck.util.config](package-summary.html)
:::

## Class Config {#class-config .title title="Class Config"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.config.Config

::: description
-   

    ------------------------------------------------------------------------

        public class Config
        extends Object

    ::: block
    Structured representation of data read from a stack of `.ini` files,
    where each file can override values defined by the previous ones.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Field                 | Description           |
        +=======================+=======================+=======================+
        | `static String`       | `DEFAULT              | ::: block             |
        |                       | _KEY_VALUE_SEPARATOR` | Used in a string      |
        |                       |                       | representation of a   |
        |                       |                       | map; separates keys   |
        |                       |                       | from values           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static char`         | `DE                   | ::: block             |
        |                       | FAULT_PAIR_SEPARATOR` | Used in a string      |
        |                       |                       | representation of a   |
        |                       |                       | map; separates pairs  |
        |                       |                       | of value              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `Config()`                        | ::: block                         |
        |                                   | Convenience constructor to create |
        |                                   | an empty config.                  |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `Config​(RawConfig rawConfig)`     |                                   |
        +-----------------------------------+-----------------------------------+
        | `Co                               |                                   |
        | nfig​(RawConfig rawConfig,       c |                                   |
        | om.google.common.collect.Immutabl |                                   |
        | eMap<Path,​RawConfig> configsMap)` |                                   |
        +-----------------------------------+-----------------------------------+

        : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `boolean`             | `equals​(Object obj)`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.c         | `get                  |                       |
        | ommon.collect.Immutab | ​(String sectionName)` |                       |
        | leMap<String,​String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `get​(String secti     |                       |
        |                       | on,    String field)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Boolean>`   | `getBoolean​(String se |                       |
        |                       | ctionName,            |                       |
        |                       | String propertyName)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getB                 |                       |
        |                       | ooleanValue​(String se |                       |
        |                       | ctionName,            |                       |
        |                       |      String propertyN |                       |
        |                       | ame,                b |                       |
        |                       | oolean defaultValue)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.co        | `getConfigsMap()`     | ::: block             |
        | mmon.collect.Immutabl |                       | A map of Paths to the |
        | eMap<Path,​RawConfig>` |                       | RawConfig that came   |
        |                       |                       | from that config      |
        |                       |                       | file.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `<T extends           | `getEn                |                       |
        |  Enum<T>>Optional<T>` | um​(String section,    |                       |
        |                       |      String field,    |                       |
        |                       |      Class<T> clazz)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Float>`     | `getFloat​(String      |                       |
        |                       | sectionName,          |                       |
        |                       | String propertyName)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `OptionalInt`         | `getInteger​(String se |                       |
        |                       | ctionName,            |                       |
        |                       | String propertyName)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `ge                   |                       |
        | ogle.common.collect.I | tListWithoutComments​( |                       |
        | mmutableList<String>` | String sectionName,   |                       |
        |                       |                       |                       |
        |                       | String propertyName)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getListWithoutComme  |                       |
        | ogle.common.collect.I | nts​(String sectionNam |                       |
        | mmutableList<String>` | e,                    |                       |
        |                       |     String propertyNa |                       |
        |                       | me,                   |                       |
        |                       |      char splitChar)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Long>`      | `getLong​(String       |                       |
        |                       |  sectionName,         |                       |
        |                       | String propertyName)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.c         | `g                    | ::: block             |
        | ommon.collect.Immutab | etMap​(String section, | Convert a string      |
        | leMap<String,​String>` |        String field)` | representation of a   |
        |                       |                       | map to a binary       |
        |                       |                       | `Immutable            |
        |                       |                       | Map<String, String>`, |
        |                       |                       | using default         |
        |                       |                       | separators            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.c         | `                     | ::: block             |
        | ommon.collect.Immutab | getMap​(String section | Convert a string      |
        | leMap<String,​String>` | ,       String field, | representation of a   |
        |                       |        char pairSepar | map to a binary       |
        |                       | atorChar,       Strin | `Immutabl             |
        |                       | g keyValueSeparator)` | eMap<String, String>` |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<com.goo     | `getOptionalListWit   | ::: block             |
        | gle.common.collect.Im | houtComments​(String s | ini4j leaves things   |
        | mutableList<String>>` | ectionName,           | that look like        |
        |                       |                       | comments in the       |
        |                       | String propertyName)` | values of entries in  |
        |                       |                       | the file.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<com.goo     | `g                    |                       |
        | gle.common.collect.Im | etOptionalListWithout |                       |
        | mutableList<String>>` | Comments​(String secti |                       |
        |                       | onName,               |                       |
        |                       |                  Stri |                       |
        |                       | ng propertyName,      |                       |
        |                       |                       |                       |
        |                       |      char splitChar)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `getOrderI            | ::: block             |
        | common.hash.HashCode` | ndependentHashCode()` | gets an               |
        |                       |                       | order-independent     |
        |                       |                       | `HashCode` of this    |
        |                       |                       | [`Co                  |
        |                       |                       | nfig`](Config.html "c |
        |                       |                       | lass in com.facebook. |
        |                       |                       | buck.util.config")\'s |
        |                       |                       | raw data.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RawConfig`           | `getRawConfig()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common    | `g                    |                       |
        | .collect.ImmutableMap | etSectionToEntries()` |                       |
        | <String,​com.google.co |                       |                       |
        | mmon.collect.Immutabl |                       |                       |
        | eMap<String,​String>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<URI>`       | `g                    |                       |
        |                       | etUrl​(String section, |                       |
        |                       |        String field)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getValue​(String      |                       |
        |                       | sectionName,          |                       |
        |                       | String propertyName)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Config`              | `overri               |                       |
        |                       | deWith​(Config other)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
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
    -   []{#field.detail}

        ### Field Detail

        []{#DEFAULT_PAIR_SEPARATOR}

        -   #### DEFAULT_PAIR_SEPARATOR

                public static final char DEFAULT_PAIR_SEPARATOR

            ::: block
            Used in a string representation of a map; separates pairs of
            value
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.config.Config.DEFAULT_PAIR_SEPARATOR)

        []{#DEFAULT_KEY_VALUE_SEPARATOR}

        -   #### DEFAULT_KEY_VALUE_SEPARATOR

                public static final String DEFAULT_KEY_VALUE_SEPARATOR

            ::: block
            Used in a string representation of a map; separates keys
            from values
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.config.Config.DEFAULT_KEY_VALUE_SEPARATOR)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### Config

                public Config()

            ::: block
            Convenience constructor to create an empty config.
            :::

        []{#<init>(com.facebook.buck.util.config.RawConfig)}

        -   #### Config

                public Config​(RawConfig rawConfig)

        []{#<init>(com.facebook.buck.util.config.RawConfig,com.google.common.collect.ImmutableMap)}

        -   #### Config

                public Config​(RawConfig rawConfig,
                              com.google.common.collect.ImmutableMap<Path,​RawConfig> configsMap)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#get(java.lang.String,java.lang.String)}

        -   #### get

            ``` methodSignature
            public Optional<String> get​(String section,
                                        String field)
            ```

        []{#get(java.lang.String)}

        -   #### get

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​String> get​(String sectionName)
            ```

        []{#getOrderIndependentHashCode()}

        -   #### getOrderIndependentHashCode

            ``` methodSignature
            public com.google.common.hash.HashCode getOrderIndependentHashCode()
            ```

            ::: block
            gets an order-independent `HashCode` of this
            [`Config`](Config.html "class in com.facebook.buck.util.config")\'s
            raw data.
            :::

        []{#getSectionToEntries()}

        -   #### getSectionToEntries

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​com.google.common.collect.ImmutableMap<String,​String>> getSectionToEntries()
            ```

        []{#getListWithoutComments(java.lang.String,java.lang.String)}

        -   #### getListWithoutComments

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getListWithoutComments​(String sectionName,
                                                                                          String propertyName)
            ```

            [Returns:]{.returnLabel}
            :   An `ImmutableList` containing all entries that don\'t
                look like comments, or the empty list if the property is
                not defined or there are no values.

        []{#getListWithoutComments(java.lang.String,java.lang.String,char)}

        -   #### getListWithoutComments

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getListWithoutComments​(String sectionName,
                                                                                          String propertyName,
                                                                                          char splitChar)
            ```

        []{#getOptionalListWithoutComments(java.lang.String,java.lang.String)}

        -   #### getOptionalListWithoutComments

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableList<String>> getOptionalListWithoutComments​(String sectionName,
                                                                                                            String propertyName)
            ```

            ::: block
            ini4j leaves things that look like comments in the values of
            entries in the file. Generally, we don\'t want to include
            these in our parameters, so filter them out where necessary.
            In an INI file, the comment separator is \";\", but some
            parsers (ini4j included) use \"#\" too. This method handles
            both cases.
            :::

            [Returns:]{.returnLabel}
            :   an `ImmutableList` containing all entries that don\'t
                look like comments, the empty list if the property is
                defined but there are no values, or Optional.empty() if
                the property is not defined.

        []{#getOptionalListWithoutComments(java.lang.String,java.lang.String,char)}

        -   #### getOptionalListWithoutComments

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableList<String>> getOptionalListWithoutComments​(String sectionName,
                                                                                                            String propertyName,
                                                                                                            char splitChar)
            ```

        []{#getValue(java.lang.String,java.lang.String)}

        -   #### getValue

            ``` methodSignature
            public Optional<String> getValue​(String sectionName,
                                             String propertyName)
            ```

        []{#getLong(java.lang.String,java.lang.String)}

        -   #### getLong

            ``` methodSignature
            public Optional<Long> getLong​(String sectionName,
                                          String propertyName)
            ```

        []{#getInteger(java.lang.String,java.lang.String)}

        -   #### getInteger

            ``` methodSignature
            public OptionalInt getInteger​(String sectionName,
                                          String propertyName)
            ```

        []{#getFloat(java.lang.String,java.lang.String)}

        -   #### getFloat

            ``` methodSignature
            public Optional<Float> getFloat​(String sectionName,
                                            String propertyName)
            ```

        []{#getBooleanValue(java.lang.String,java.lang.String,boolean)}

        -   #### getBooleanValue

            ``` methodSignature
            public boolean getBooleanValue​(String sectionName,
                                           String propertyName,
                                           boolean defaultValue)
            ```

        []{#getBoolean(java.lang.String,java.lang.String)}

        -   #### getBoolean

            ``` methodSignature
            public Optional<Boolean> getBoolean​(String sectionName,
                                                String propertyName)
            ```

        []{#getEnum(java.lang.String,java.lang.String,java.lang.Class)}

        -   #### getEnum

            ``` methodSignature
            public <T extends Enum<T>> Optional<T> getEnum​(String section,
                                                           String field,
                                                           Class<T> clazz)
            ```

        []{#getUrl(java.lang.String,java.lang.String)}

        -   #### getUrl

            ``` methodSignature
            public Optional<URI> getUrl​(String section,
                                        String field)
            ```

        []{#getMap(java.lang.String,java.lang.String,char,java.lang.String)}

        -   #### getMap

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​String> getMap​(String section,
                                                                                      String field,
                                                                                      char pairSeparatorChar,
                                                                                      String keyValueSeparator)
            ```

            ::: block
            Convert a string representation of a map to a binary
            `ImmutableMap<String, String>`
            :::

            [Parameters:]{.paramLabel}
            :   `section` - Config file section name
            :   `field` - Config file value name
            :   `pairSeparatorChar` - Character that separates pairs of
                keys and values
            :   `keyValueSeparator` - String that separates keys and
                values

            [Returns:]{.returnLabel}
            :   An `ImmutableMap`

        []{#getMap(java.lang.String,java.lang.String)}

        -   #### getMap

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​String> getMap​(String section,
                                                                                      String field)
            ```

            ::: block
            Convert a string representation of a map to a binary
            `ImmutableMap<String, String>`, using default separators
            :::

            [Parameters:]{.paramLabel}
            :   `section` - Config file section name
            :   `field` - Config file value name

            [Returns:]{.returnLabel}
            :   An `ImmutableMap`

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(Object obj)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `Object`

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `Object`

        []{#overrideWith(com.facebook.buck.util.config.Config)}

        -   #### overrideWith

            ``` methodSignature
            public Config overrideWith​(Config other)
            ```

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

        []{#getRawConfig()}

        -   #### getRawConfig

            ``` methodSignature
            public RawConfig getRawConfig()
            ```

        []{#getConfigsMap()}

        -   #### getConfigsMap

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<Path,​RawConfig> getConfigsMap()
            ```

            ::: block
            A map of Paths to the RawConfig that came from that config
            file. When accessing this structure, bear in mind that it
            might have values that have been overriden in the merged
            rawConfig.
            :::

            [Returns:]{.returnLabel}
            :   A map of Paths to the RawConfig whose origin is that
                config file.
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

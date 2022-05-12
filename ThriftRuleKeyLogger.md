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
[Package]{.packageLabelInType} [com.facebook.buck.log.thrift](package-summary.html)
:::

## Class ThriftRuleKeyLogger {#class-thriftrulekeylogger .title title="Class ThriftRuleKeyLogger"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.log.thrift.ThriftRuleKeyLogger

::: description
-   

    All Implemented Interfaces:
    :   `AutoCloseable`

    ------------------------------------------------------------------------

        public class ThriftRuleKeyLogger
        extends Object
        implements AutoCloseable

    ::: block
    Writes out length prefixed ThriftCompact serialized representations
    of Rule Keys to an output stream.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `ThriftRu                         | ::: block                         |
        | leKeyLogger​(OutputStream writer)` | Creates a ThriftRuleKeyLogger     |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+

        : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `close()`             | ::: block             |
        |                       |                       | Close the output      |
        |                       |                       | stream                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `c                    | ::: block             |
        |  ThriftRuleKeyLogger` | reate​(Path filename)` | Create an instance of |
        |                       |                       | a logger that writes  |
        |                       |                       | to the given file     |
        |                       |                       | name                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `wr                   | ::: block             |
        |                       | ite​(com.facebook.buck | Writes a serialized   |
        |                       | .log.thrift.rulekeys. | form of the rule key  |
        |                       | FullRuleKey ruleKey)` | to the output stream. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.io.OutputStream)}

        -   #### ThriftRuleKeyLogger

                public ThriftRuleKeyLogger​(OutputStream writer)

            ::: block
            Creates a ThriftRuleKeyLogger
            :::

            [Parameters:]{.paramLabel}
            :   `writer` - The stream to write serialized data to
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#close()}

        -   #### close

            ``` methodSignature
            public void close()
            ```

            ::: block
            Close the output stream
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`

        []{#write(com.facebook.buck.log.thrift.rulekeys.FullRuleKey)}

        -   #### write

            ``` methodSignature
            public void write​(com.facebook.buck.log.thrift.rulekeys.FullRuleKey ruleKey)
            ```

            ::: block
            Writes a serialized form of the rule key to the output
            stream. Serialization is Thrift Compact, with a 4 byte
            length prefix. Serialization or write errors are swallowed,
            and logged so that failures to write do not terminate buck
            :::

            [Parameters:]{.paramLabel}
            :   `ruleKey` - The non-null ruleKey to write out to the
                ifle

        []{#create(java.nio.file.Path)}

        -   #### create

            ``` methodSignature
            public static ThriftRuleKeyLogger create​(Path filename)
                                              throws IOException
            ```

            ::: block
            Create an instance of a logger that writes to the given file
            name
            An attempt is made to create all subdirectories before
            opening the file
            :::

            [Parameters:]{.paramLabel}
            :   `filename` - The file to write thrift data to

            [Returns:]{.returnLabel}
            :   A binary logger

            [Throws:]{.throwsLabel}
            :   `FileNotFoundException` - Thrown if the subdirectory
                containing the filename could not be created
            :   `IOException`
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

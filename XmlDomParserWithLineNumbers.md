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
[Package]{.packageLabelInType} [com.facebook.buck.util.xml](package-summary.html)
:::

## Class XmlDomParserWithLineNumbers {#class-xmldomparserwithlinenumbers .title title="Class XmlDomParserWithLineNumbers"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.xml.XmlDomParserWithLineNumbers

::: description
-   

    ------------------------------------------------------------------------

        public class XmlDomParserWithLineNumbers
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static Document`     | `pa                   |                       |
        |                       | rse​(InputStream xml)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Document`     | `pa                   | ::: block             |
        |                       | rse​(InputSource xml)` | Constructs a document |
        |                       |                       | builder, parses xml,  |
        |                       |                       | then returns a        |
        |                       |                       | document with a new   |
        |                       |                       | DocumentLocation      |
        |                       |                       | object stored as      |
        |                       |                       | userData in each node |
        |                       |                       | :::                   |
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

        []{#parse(java.io.InputStream)}

        -   #### parse

            ``` methodSignature
            public static Document parse​(InputStream xml)
                                  throws IOException,
                                         SAXException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`
            :   `SAXException`

        []{#parse(org.xml.sax.InputSource)}

        -   #### parse

            ``` methodSignature
            public static Document parse​(InputSource xml)
                                  throws IOException,
                                         SAXException
            ```

            ::: block
            Constructs a document builder, parses xml, then returns a
            document with a new DocumentLocation object stored as
            userData in each node
            :::

            [Parameters:]{.paramLabel}
            :   `xml` - the input source of xml

            [Returns:]{.returnLabel}
            :   a document of parsed xml with line and column data in
                each node

            [Throws:]{.throwsLabel}
            :   `IOException`
            :   `SAXException`
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

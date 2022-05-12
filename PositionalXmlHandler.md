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
[Package]{.packageLabelInType} [com.facebook.buck.util.xml](package-summary.html)
:::

## Class PositionalXmlHandler {#class-positionalxmlhandler .title title="Class PositionalXmlHandler"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [org.xml.sax.helpers.DefaultHandler](http://docs.oracle.com/javase/7/docs/api/org/xml/sax/helpers/DefaultHandler.html?is-external=true "class or interface in org.xml.sax.helpers"){.externalLink}

    -   -   com.facebook.buck.util.xml.PositionalXmlHandler

::: description
-   

    All Implemented Interfaces:
    :   `ContentHandler`, `DTDHandler`, `EntityResolver`, `ErrorHandler`

    ------------------------------------------------------------------------

        public class PositionalXmlHandler
        extends DefaultHandler

    ::: block
    Builds a DOM tree that maintains element line and column numbers in
    userData
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                      Description
          ------------------- -------------------------- -------------
          `static String`     `LOCATION_USER_DATA_KEY`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                Description
          -------------------------- -------------
          `PositionalXmlHandler()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                                                  Description
          ------------------- ----------------------------------------------------------------------------------------------------------------------- -------------
          `void`              `characters​(char[] ch,           int start,           int length)`                                                       
          `void`              `endElement​(String uri,           String localName,           String qName)`                                             
          `void`              `error​(SAXParseException ex)`                                                                                            
          `void`              `fatalError​(SAXParseException ex)`                                                                                       
          `void`              `setDocumentLocator​(Locator locator)`                                                                                    
          `void`              `startDocument()`                                                                                                        
          `void`              `startElement​(String uri,             String localName,             String qName,             Attributes attributes)`    
          `void`              `warning​(SAXParseException exception)`                                                                                   

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.org.xml.sax.helpers.DefaultHandler}

            ### Methods inherited from class org.xml.sax.helpers.[DefaultHandler](http://docs.oracle.com/javase/7/docs/api/org/xml/sax/helpers/DefaultHandler.html?is-external=true "class or interface in org.xml.sax.helpers"){.externalLink}

            `endDocument, endPrefixMapping, ignorableWhitespace, notationDecl, processingInstruction, resolveEntity, skippedEntity, startPrefixMapping, unparsedEntityDecl`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#LOCATION_USER_DATA_KEY}

        -   #### LOCATION_USER_DATA_KEY

                public static final String LOCATION_USER_DATA_KEY

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.xml.PositionalXmlHandler.LOCATION_USER_DATA_KEY)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### PositionalXmlHandler

                public PositionalXmlHandler()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#startDocument()}

        -   #### startDocument

            ``` methodSignature
            public void startDocument()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `startDocument` in interface `ContentHandler`

            [Overrides:]{.overrideSpecifyLabel}
            :   `startDocument` in class `DefaultHandler`

        []{#setDocumentLocator(org.xml.sax.Locator)}

        -   #### setDocumentLocator

            ``` methodSignature
            public void setDocumentLocator​(Locator locator)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `setDocumentLocator` in interface `ContentHandler`

            [Overrides:]{.overrideSpecifyLabel}
            :   `setDocumentLocator` in class `DefaultHandler`

        []{#startElement(java.lang.String,java.lang.String,java.lang.String,org.xml.sax.Attributes)}

        -   #### startElement

            ``` methodSignature
            public void startElement​(String uri,
                                     String localName,
                                     String qName,
                                     Attributes attributes)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `startElement` in interface `ContentHandler`

            [Overrides:]{.overrideSpecifyLabel}
            :   `startElement` in class `DefaultHandler`

        []{#endElement(java.lang.String,java.lang.String,java.lang.String)}

        -   #### endElement

            ``` methodSignature
            public void endElement​(String uri,
                                   String localName,
                                   String qName)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `endElement` in interface `ContentHandler`

            [Overrides:]{.overrideSpecifyLabel}
            :   `endElement` in class `DefaultHandler`

        []{#characters(char[],int,int)}

        -   #### characters

            ``` methodSignature
            public void characters​(char[] ch,
                                   int start,
                                   int length)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `characters` in interface `ContentHandler`

            [Overrides:]{.overrideSpecifyLabel}
            :   `characters` in class `DefaultHandler`

        []{#error(org.xml.sax.SAXParseException)}

        -   #### error

            ``` methodSignature
            public void error​(SAXParseException ex)
                       throws SAXException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `error` in interface `ErrorHandler`

            [Overrides:]{.overrideSpecifyLabel}
            :   `error` in class `DefaultHandler`

            [Throws:]{.throwsLabel}
            :   `SAXException`

        []{#fatalError(org.xml.sax.SAXParseException)}

        -   #### fatalError

            ``` methodSignature
            public void fatalError​(SAXParseException ex)
                            throws SAXException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `fatalError` in interface `ErrorHandler`

            [Overrides:]{.overrideSpecifyLabel}
            :   `fatalError` in class `DefaultHandler`

            [Throws:]{.throwsLabel}
            :   `SAXException`

        []{#warning(org.xml.sax.SAXParseException)}

        -   #### warning

            ``` methodSignature
            public void warning​(SAXParseException exception)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `warning` in interface `ErrorHandler`

            [Overrides:]{.overrideSpecifyLabel}
            :   `warning` in class `DefaultHandler`
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

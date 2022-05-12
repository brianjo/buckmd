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
[Package]{.packageLabelInType} [com.facebook.buck.test](package-summary.html)
:::

## Class TestXmlUnescaper {#class-testxmlunescaper .title title="Class TestXmlUnescaper"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.test.TestXmlUnescaper

::: description
-   

    ------------------------------------------------------------------------

        public abstract class TestXmlUnescaper
        extends Object

    ::: block
    An XML escaper that replaces invalid xml characters with valid ones.
    The behaviour is intended to match that of guava\'s XmlEscapers
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type           Field                   Description
          --------------------------- ----------------------- -------------
          `static TestXmlUnescaper`   `ATTRIBUTE_UNESCAPER`    
          `static TestXmlUnescaper`   `CONTENT_UNESCAPER`      

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor            Description
          ---------------------- -------------
          `TestXmlUnescaper()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type          Method                                                                        Description
          -------------------------- ----------------------------------------------------------------------------- -------------
          `String`                   `unescape​(String str)`                                                         
          `protected abstract int`   `unescapeStr​(String s,            int offset,            StringBuilder sb)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
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

        []{#CONTENT_UNESCAPER}

        -   #### CONTENT_UNESCAPER

                public static final TestXmlUnescaper CONTENT_UNESCAPER

        []{#ATTRIBUTE_UNESCAPER}

        -   #### ATTRIBUTE_UNESCAPER

                public static final TestXmlUnescaper ATTRIBUTE_UNESCAPER
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### TestXmlUnescaper

                public TestXmlUnescaper()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#unescape(java.lang.String)}

        -   #### unescape

            ``` methodSignature
            public final String unescape​(String str)
            ```

            [Parameters:]{.paramLabel}
            :   `str` - the String with xml escaped characters

            [Returns:]{.returnLabel}
            :   the unescaped string

        []{#unescapeStr(java.lang.String,int,java.lang.StringBuilder)}

        -   #### unescapeStr

            ``` methodSignature
            protected abstract int unescapeStr​(String s,
                                               int offset,
                                               StringBuilder sb)
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

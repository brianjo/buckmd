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
[Package]{.packageLabelInType} [com.facebook.buck.util.i18n](package-summary.html)
:::

## Class NumberFormatter {#class-numberformatter .title title="Class NumberFormatter"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.i18n.NumberFormatter

::: description
-   

    ------------------------------------------------------------------------

        @ThreadSafe
        public class NumberFormatter
        extends Object

    ::: block
    Thread-safe and i18n-safe wrapper for
    [`NumberFormat`](http://docs.oracle.com/javase/7/docs/api/java/text/NumberFormat.html?is-external=true "class or interface in java.text"){.externalLink}
    (which is not thread-safe).
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `NumberFormatter​(java             | ::: block                         |
        | .util.function.Function<Locale,​Nu | Given a function which creates    |
        | mberFormat> numberFormatCreator)` | [`NumberFormat`](htt              |
        |                                   | p://docs.oracle.com/javase/7/docs |
        |                                   | /api/java/text/NumberFormat.html? |
        |                                   | is-external=true "class or interf |
        |                                   | ace in java.text"){.externalLink} |
        |                                   | objects for a                     |
        |                                   | [`Locale`                         |
        |                                   | ](http://docs.oracle.com/javase/7 |
        |                                   | /docs/api/java/util/Locale.html?i |
        |                                   | s-external=true "class or interfa |
        |                                   | ce in java.util"){.externalLink}, |
        |                                   | returns a wrapper providing       |
        |                                   | thread-safe access to the         |
        |                                   | formatter for that locale.        |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+

        : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                                 Description
          ------------------- ------------------------------------------------------------------------------------------------------ -------------
          `String`            `format​(Locale locale,       double number)`                                                            
          `StringBuffer`      `format​(Locale locale,       double number,       StringBuffer toAppendTo,       FieldPosition pos)`    
          `String`            `format​(Locale locale,       long number)`                                                              
          `String`            `format​(Locale locale,       Object object)`                                                            
          `StringBuffer`      `format​(Locale locale,       Object object,       StringBuffer toAppendTo,       FieldPosition pos)`    
          `Number`            `parse​(Locale locale,      String source)`                                                              
          `Number`            `parse​(Locale locale,      String source,      ParsePosition pos)`                                      
          `Object`            `parseObject​(Locale locale,            String source,            ParsePosition pos)`                    

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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.util.function.Function)}

        -   #### NumberFormatter

                public NumberFormatter​(java.util.function.Function<Locale,​NumberFormat> numberFormatCreator)

            ::: block
            Given a function which creates
            [`NumberFormat`](http://docs.oracle.com/javase/7/docs/api/java/text/NumberFormat.html?is-external=true "class or interface in java.text"){.externalLink}
            objects for a
            [`Locale`](http://docs.oracle.com/javase/7/docs/api/java/util/Locale.html?is-external=true "class or interface in java.util"){.externalLink},
            returns a wrapper providing thread-safe access to the
            formatter for that locale.
            :::
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#format(java.util.Locale,double)}

        -   #### format

            ``` methodSignature
            public String format​(Locale locale,
                                 double number)
            ```

            [See Also:]{.seeLabel}
            :   [`NumberFormat.format(double)`](http://docs.oracle.com/javase/7/docs/api/java/text/NumberFormat.html?is-external=true#format(double) "class or interface in java.text"){.externalLink}

        []{#format(java.util.Locale,double,java.lang.StringBuffer,java.text.FieldPosition)}

        -   #### format

            ``` methodSignature
            public StringBuffer format​(Locale locale,
                                       double number,
                                       StringBuffer toAppendTo,
                                       FieldPosition pos)
            ```

            [See Also:]{.seeLabel}
            :   [`NumberFormat.format(double, StringBuffer, FieldPosition)`](http://docs.oracle.com/javase/7/docs/api/java/text/NumberFormat.html?is-external=true#format(double,java.lang.StringBuffer,java.text.FieldPosition) "class or interface in java.text"){.externalLink}

        []{#format(java.util.Locale,long)}

        -   #### format

            ``` methodSignature
            public String format​(Locale locale,
                                 long number)
            ```

            [See Also:]{.seeLabel}
            :   [`NumberFormat.format(long)`](http://docs.oracle.com/javase/7/docs/api/java/text/NumberFormat.html?is-external=true#format(long) "class or interface in java.text"){.externalLink}

        []{#format(java.util.Locale,java.lang.Object)}

        -   #### format

            ``` methodSignature
            public String format​(Locale locale,
                                 Object object)
            ```

            [See Also:]{.seeLabel}
            :   [`Format.format(Object)`](http://docs.oracle.com/javase/7/docs/api/java/text/Format.html?is-external=true#format(java.lang.Object) "class or interface in java.text"){.externalLink}

        []{#format(java.util.Locale,java.lang.Object,java.lang.StringBuffer,java.text.FieldPosition)}

        -   #### format

            ``` methodSignature
            public StringBuffer format​(Locale locale,
                                       Object object,
                                       StringBuffer toAppendTo,
                                       FieldPosition pos)
            ```

            [See Also:]{.seeLabel}
            :   [`NumberFormat.format(Object, StringBuffer, FieldPosition)`](http://docs.oracle.com/javase/7/docs/api/java/text/NumberFormat.html?is-external=true#format(java.lang.Object,java.lang.StringBuffer,java.text.FieldPosition) "class or interface in java.text"){.externalLink}

        []{#parse(java.util.Locale,java.lang.String)}

        -   #### parse

            ``` methodSignature
            public Number parse​(Locale locale,
                                String source)
                         throws ParseException
            ```

            [Throws:]{.throwsLabel}
            :   `ParseException`

            [See Also:]{.seeLabel}
            :   [`NumberFormat.parse(String)`](http://docs.oracle.com/javase/7/docs/api/java/text/NumberFormat.html?is-external=true#parse(java.lang.String) "class or interface in java.text"){.externalLink}

        []{#parse(java.util.Locale,java.lang.String,java.text.ParsePosition)}

        -   #### parse

            ``` methodSignature
            public Number parse​(Locale locale,
                                String source,
                                ParsePosition pos)
            ```

            [See Also:]{.seeLabel}
            :   [`NumberFormat.parse(String, ParsePosition)`](http://docs.oracle.com/javase/7/docs/api/java/text/NumberFormat.html?is-external=true#parse(java.lang.String,java.text.ParsePosition) "class or interface in java.text"){.externalLink}

        []{#parseObject(java.util.Locale,java.lang.String,java.text.ParsePosition)}

        -   #### parseObject

            ``` methodSignature
            public Object parseObject​(Locale locale,
                                      String source,
                                      ParsePosition pos)
            ```

            [See Also:]{.seeLabel}
            :   [`NumberFormat.parseObject(String, ParsePosition)`](http://docs.oracle.com/javase/7/docs/api/java/text/NumberFormat.html?is-external=true#parseObject(java.lang.String,java.text.ParsePosition) "class or interface in java.text"){.externalLink}
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

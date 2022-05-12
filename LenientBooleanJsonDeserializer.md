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
-   [Nested](#nested.class.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.util](package-summary.html)
:::

## Class LenientBooleanJsonDeserializer {#class-lenientbooleanjsondeserializer .title title="Class LenientBooleanJsonDeserializer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.fasterxml.jackson.databind.JsonDeserializer\<[Boolean](http://docs.oracle.com/javase/7/docs/api/java/lang/Boolean.html?is-external=true "class or interface in java.lang"){.externalLink}\>

    -   -   com.facebook.buck.util.LenientBooleanJsonDeserializer

::: description
-   

    All Implemented Interfaces:
    :   `com.fasterxml.jackson.databind.deser.NullValueProvider`

    ------------------------------------------------------------------------

        public class LenientBooleanJsonDeserializer
        extends com.fasterxml.jackson.databind.JsonDeserializer<Boolean>

    ::: block
    JSON deserializer which converts boolean, numeric, and string values
    into booleans.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.fasterxml.jackson.databind.JsonDeserializer}

            ### Nested classes/interfaces inherited from class com.fasterxml.jackson.databind.JsonDeserializer

            `com.fasterxml.jackson.databind.JsonDeserializer.None`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                          Description
          ------------------------------------ -------------
          `LenientBooleanJsonDeserializer()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                                                                                     Description
          ------------------- ---------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `Boolean`           `deserialize​(com.fasterxml.jackson.core.JsonParser jsonParser,            com.fasterxml.jackson.databind.DeserializationContext deserializationContext)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.fasterxml.jackson.databind.JsonDeserializer}

            ### Methods inherited from class com.fasterxml.jackson.databind.JsonDeserializer

            `deserialize, deserializeWithType, findBackReference, getDelegatee, getEmptyAccessPattern, getEmptyValue, getEmptyValue, getKnownPropertyNames, getNullAccessPattern, getNullValue, getNullValue, getObjectIdReader, handledType, isCachable, replaceDelegatee, supportsUpdate, unwrappingDeserializer`

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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### LenientBooleanJsonDeserializer

                public LenientBooleanJsonDeserializer()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#deserialize(com.fasterxml.jackson.core.JsonParser,com.fasterxml.jackson.databind.DeserializationContext)}

        -   #### deserialize

            ``` methodSignature
            public Boolean deserialize​(com.fasterxml.jackson.core.JsonParser jsonParser,
                                       com.fasterxml.jackson.databind.DeserializationContext deserializationContext)
                                throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `deserialize` in
                class `com.fasterxml.jackson.databind.JsonDeserializer<Boolean>`

            [Throws:]{.throwsLabel}
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
-   [Nested](#nested.class.summary) \| 
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

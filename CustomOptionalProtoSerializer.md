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
[Package]{.packageLabelInType} [com.facebook.buck.util.json](package-summary.html)
:::

## Class CustomOptionalProtoSerializer {#class-customoptionalprotoserializer .title title="Class CustomOptionalProtoSerializer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.fasterxml.jackson.databind.JsonSerializer\<[Optional](http://docs.oracle.com/javase/7/docs/api/java/util/Optional.html?is-external=true "class or interface in java.util"){.externalLink}\<com.google.protobuf.Message\>\>

    -   -   com.facebook.buck.util.json.CustomOptionalProtoSerializer

::: description
-   

    All Implemented Interfaces:
    :   `com.fasterxml.jackson.databind.jsonFormatVisitors.JsonFormatVisitable`

    ------------------------------------------------------------------------

        public class CustomOptionalProtoSerializer
        extends com.fasterxml.jackson.databind.JsonSerializer<Optional<com.google.protobuf.Message>>

    ::: block
    Custom serializer for ProtoBuf classes as jackson is not able to
    serialize them.
    https://stackoverflow.com/questions/51588778/convert-a-protobuf-to-json-using-jackson
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.fasterxml.jackson.databind.JsonSerializer}

            ### Nested classes/interfaces inherited from class com.fasterxml.jackson.databind.JsonSerializer

            `com.fasterxml.jackson.databind.JsonSerializer.None`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                         Description
          ----------------------------------- -------------
          `CustomOptionalProtoSerializer()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                                                                                                                      Description
          ------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `void`              `serialize​(Optional<com.google.protobuf.Message> message,          com.fasterxml.jackson.core.JsonGenerator gen,          com.fasterxml.jackson.databind.SerializerProvider serializers)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.fasterxml.jackson.databind.JsonSerializer}

            ### Methods inherited from class com.fasterxml.jackson.databind.JsonSerializer

            `acceptJsonFormatVisitor, getDelegatee, handledType, isEmpty, isEmpty, isUnwrappingSerializer, properties, replaceDelegatee, serializeWithType, unwrappingSerializer, usesObjectId, withFilterId`

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

        -   #### CustomOptionalProtoSerializer

                public CustomOptionalProtoSerializer()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#serialize(java.util.Optional,com.fasterxml.jackson.core.JsonGenerator,com.fasterxml.jackson.databind.SerializerProvider)}

        -   #### serialize

            ``` methodSignature
            public void serialize​(Optional<com.google.protobuf.Message> message,
                                  com.fasterxml.jackson.core.JsonGenerator gen,
                                  com.fasterxml.jackson.databind.SerializerProvider serializers)
                           throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `serialize` in
                class `com.fasterxml.jackson.databind.JsonSerializer<Optional<com.google.protobuf.Message>>`

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

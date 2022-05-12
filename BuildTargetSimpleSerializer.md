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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
-   [Field](#field.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.core.model.impl](package-summary.html)
:::

## Class BuildTargetSimpleSerializer {#class-buildtargetsimpleserializer .title title="Class BuildTargetSimpleSerializer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.fasterxml.jackson.databind.JsonSerializer\<T\>

    -   -   com.fasterxml.jackson.databind.ser.std.StdSerializer\<[BuildTarget](../BuildTarget.html "class in com.facebook.buck.core.model")\>

        -   -   com.facebook.buck.core.model.impl.BuildTargetSimpleSerializer

::: description
-   

    All Implemented Interfaces:
    :   `com.fasterxml.jackson.databind.jsonFormatVisitors.JsonFormatVisitable`,
        `com.fasterxml.jackson.databind.jsonschema.SchemaAware`,
        `Serializable`

    ------------------------------------------------------------------------

        public class BuildTargetSimpleSerializer
        extends com.fasterxml.jackson.databind.ser.std.StdSerializer<BuildTarget>

    ::: block
    JSON serializer of
    [`BuildTarget`](../BuildTarget.html "class in com.facebook.buck.core.model")
    that uses fully qualified name to represent a target.
    :::

    [See Also:]{.seeLabel}
    :   [Serialized
        Form](../../../../../../serialized-form.html#com.facebook.buck.core.model.impl.BuildTargetSimpleSerializer)
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
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.fasterxml.jackson.databind.ser.std.StdSerializer}

            ### Fields inherited from class com.fasterxml.jackson.databind.ser.std.StdSerializer

            `_handledType`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                                                       Description
          -------------- ----------------------------------------------------------------- -------------
          `protected `   `BuildTargetSimpleSerializer​(Class<BuildTarget> instanceClass)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                                                                                             Description
          ------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `void`              `serialize​(BuildTarget buildTarget,          com.fasterxml.jackson.core.JsonGenerator gen,          com.fasterxml.jackson.databind.SerializerProvider provider)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.fasterxml.jackson.databind.ser.std.StdSerializer}

            ### Methods inherited from class com.fasterxml.jackson.databind.ser.std.StdSerializer

            `_neitherNull, _nonEmpty, acceptJsonFormatVisitor, createSchemaNode, createSchemaNode, findAnnotatedContentSerializer, findContextualConvertingSerializer, findConvertingContentSerializer, findFormatFeature, findFormatOverrides, findIncludeOverrides, findPropertyFilter, getSchema, getSchema, handledType, isDefaultSerializer, visitArrayFormat, visitArrayFormat, visitFloatFormat, visitIntFormat, visitIntFormat, visitStringFormat, visitStringFormat, wrapAndThrow, wrapAndThrow`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.fasterxml.jackson.databind.JsonSerializer}

            ### Methods inherited from class com.fasterxml.jackson.databind.JsonSerializer

            `getDelegatee, isEmpty, isEmpty, isUnwrappingSerializer, properties, replaceDelegatee, serializeWithType, unwrappingSerializer, usesObjectId, withFilterId`

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

        []{#<init>(java.lang.Class)}

        -   #### BuildTargetSimpleSerializer

                protected BuildTargetSimpleSerializer​(Class<BuildTarget> instanceClass)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#serialize(com.facebook.buck.core.model.BuildTarget,com.fasterxml.jackson.core.JsonGenerator,com.fasterxml.jackson.databind.SerializerProvider)}

        -   #### serialize

            ``` methodSignature
            public void serialize​(BuildTarget buildTarget,
                                  com.fasterxml.jackson.core.JsonGenerator gen,
                                  com.fasterxml.jackson.databind.SerializerProvider provider)
                           throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `serialize` in
                class `com.fasterxml.jackson.databind.ser.std.StdSerializer<BuildTarget>`

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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

<div>

-   Summary: 
-   [Nested](#nested.class.summary) \| 
-   [Field](#field.summary) \| 
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

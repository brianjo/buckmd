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
[Package]{.packageLabelInType} [com.facebook.buck.core.test.rule](package-summary.html)
:::

## Interface ExternalTestSpec {#interface-externaltestspec .title title="Interface ExternalTestSpec"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `com.fasterxml.jackson.databind.JsonSerializable`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `ExternalRunnerTestProtocol`, `ExternalTestRunnerTestSpec`

    ------------------------------------------------------------------------

        public interface ExternalTestSpec
        extends com.fasterxml.jackson.databind.JsonSerializable

    ::: block
    A JSON-serializable structure that gets passed to external test
    runners.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.fasterxml.jackson.databind.JsonSerializable}

            ### Nested classes/interfaces inherited from interface com.fasterxml.jackson.databind.JsonSerializable

            `com.fasterxml.jackson.databind.JsonSerializable.Base`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                                                                                                                                                                                       Description
          ------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `void`              `serialize​(com.fasterxml.jackson.core.JsonGenerator jsonGenerator,          com.fasterxml.jackson.databind.SerializerProvider serializerProvider)`                                                                                                            
          `void`              `serializeWithType​(com.fasterxml.jackson.core.JsonGenerator jsonGenerator,                  com.fasterxml.jackson.databind.SerializerProvider serializerProvider,                  com.fasterxml.jackson.databind.jsontype.TypeSerializer typeSerializer)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#serialize(com.fasterxml.jackson.core.JsonGenerator,com.fasterxml.jackson.databind.SerializerProvider)}

        -   #### serialize

            ``` methodSignature
            void serialize​(com.fasterxml.jackson.core.JsonGenerator jsonGenerator,
                           com.fasterxml.jackson.databind.SerializerProvider serializerProvider)
                    throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `serialize` in
                interface `com.fasterxml.jackson.databind.JsonSerializable`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#serializeWithType(com.fasterxml.jackson.core.JsonGenerator,com.fasterxml.jackson.databind.SerializerProvider,com.fasterxml.jackson.databind.jsontype.TypeSerializer)}

        -   #### serializeWithType

            ``` methodSignature
            void serializeWithType​(com.fasterxml.jackson.core.JsonGenerator jsonGenerator,
                                   com.fasterxml.jackson.databind.SerializerProvider serializerProvider,
                                   com.fasterxml.jackson.databind.jsontype.TypeSerializer typeSerializer)
                            throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `serializeWithType` in
                interface `com.fasterxml.jackson.databind.JsonSerializable`

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

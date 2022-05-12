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
[Package]{.packageLabelInType} [com.facebook.buck.core.test.rule](package-summary.html)
:::

## Class ExternalRunnerTestProtocol {#class-externalrunnertestprotocol .title title="Class ExternalRunnerTestProtocol"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.test.rule.ExternalRunnerTestProtocol

::: description
-   

    All Implemented Interfaces:
    :   `ExternalTestSpec`,
        `com.fasterxml.jackson.databind.JsonSerializable`

    ------------------------------------------------------------------------

        public abstract class ExternalRunnerTestProtocol
        extends Object
        implements ExternalTestSpec

    ::: block
    The JSON serializable object for test protocol
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
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                      Description
          -------------------------------- -------------
          `ExternalRunnerTestProtocol()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                Method                                                                                                                                                                                                                                                       Description
          ------------------------------------------------ ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `protected abstract SourcePathResolverAdapter`   `getSourcePathResolver()`                                                                                                                                                                                                                                     
          `protected abstract CoercedTestRunnerSpec`       `getSpecs()`                                                                                                                                                                                                                                                  
          `protected abstract BuildTarget`                 `getTarget()`                                                                                                                                                                                                                                                 
          `void`                                           `serialize​(com.fasterxml.jackson.core.JsonGenerator jsonGenerator,          com.fasterxml.jackson.databind.SerializerProvider serializerProvider)`                                                                                                            
          `void`                                           `serializeWithType​(com.fasterxml.jackson.core.JsonGenerator jsonGenerator,                  com.fasterxml.jackson.databind.SerializerProvider serializerProvider,                  com.fasterxml.jackson.databind.jsontype.TypeSerializer typeSerializer)`    

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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### ExternalRunnerTestProtocol

                public ExternalRunnerTestProtocol()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getTarget()}

        -   #### getTarget

            ``` methodSignature
            protected abstract BuildTarget getTarget()
            ```

            [Returns:]{.returnLabel}
            :   the build target of this rule.

        []{#getSpecs()}

        -   #### getSpecs

            ``` methodSignature
            protected abstract CoercedTestRunnerSpec getSpecs()
            ```

            [Returns:]{.returnLabel}
            :   the test protocol specs defined in the BUCK file. This
                is a free form dictionary that will be serialized and
                passed to the test runners.

        []{#getSourcePathResolver()}

        -   #### getSourcePathResolver

            ``` methodSignature
            protected abstract SourcePathResolverAdapter getSourcePathResolver()
            ```

        []{#serialize(com.fasterxml.jackson.core.JsonGenerator,com.fasterxml.jackson.databind.SerializerProvider)}

        -   #### serialize

            ``` methodSignature
            public void serialize​(com.fasterxml.jackson.core.JsonGenerator jsonGenerator,
                                  com.fasterxml.jackson.databind.SerializerProvider serializerProvider)
                           throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `serialize` in interface `ExternalTestSpec`

            [Specified by:]{.overrideSpecifyLabel}
            :   `serialize` in
                interface `com.fasterxml.jackson.databind.JsonSerializable`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#serializeWithType(com.fasterxml.jackson.core.JsonGenerator,com.fasterxml.jackson.databind.SerializerProvider,com.fasterxml.jackson.databind.jsontype.TypeSerializer)}

        -   #### serializeWithType

            ``` methodSignature
            public void serializeWithType​(com.fasterxml.jackson.core.JsonGenerator jsonGenerator,
                                          com.fasterxml.jackson.databind.SerializerProvider serializerProvider,
                                          com.fasterxml.jackson.databind.jsontype.TypeSerializer typeSerializer)
                                   throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `serializeWithType` in interface `ExternalTestSpec`

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

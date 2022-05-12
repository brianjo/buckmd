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
-   Nested \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.core.module.annotationprocessor](package-summary.html)
:::

## Class BuckModuleAnnotationProcessor {#class-buckmoduleannotationprocessor .title title="Class BuckModuleAnnotationProcessor"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [javax.annotation.processing.AbstractProcessor](http://docs.oracle.com/javase/7/docs/api/javax/annotation/processing/AbstractProcessor.html?is-external=true "class or interface in javax.annotation.processing"){.externalLink}

    -   -   com.facebook.buck.core.module.annotationprocessor.BuckModuleAnnotationProcessor

::: description
-   

    All Implemented Interfaces:
    :   `Processor`

    ------------------------------------------------------------------------

        @SupportedAnnotationTypes("com.facebook.buck.core.module.BuckModule")
        public class BuckModuleAnnotationProcessor
        extends AbstractProcessor

    ::: block
    Generates an adapter plugin for the plugin framework to allow
    loading modules from jars outside of the main Buck jar.
    For example, given the following configuration:

           package com.facebook.buck.some.module;

          @BuckModule
           public class SomeModule {}
         

    The annotation processor will generate the following adapter in the
    same package:
           public class SomeModuleAdapterPlugin extends Plugin {
             public SomeModuleAdapterPlugin(PluginWrapper wrapper) {
               super(wrapper);
             }
           }
         
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.javax.annotation.processing.AbstractProcessor}

            ### Fields inherited from class javax.annotation.processing.[AbstractProcessor](http://docs.oracle.com/javase/7/docs/api/javax/annotation/processing/AbstractProcessor.html?is-external=true "class or interface in javax.annotation.processing"){.externalLink}

            `processingEnv`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                         Description
          ----------------------------------- -------------
          `BuckModuleAnnotationProcessor()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                Description
          ------------------- ------------------------------------------------------------------------------------- -------------
          `SourceVersion`     `getSupportedSourceVersion()`                                                          
          `boolean`           `process​(Set<? extends TypeElement> annotations,        RoundEnvironment roundEnv)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.javax.annotation.processing.AbstractProcessor}

            ### Methods inherited from class javax.annotation.processing.[AbstractProcessor](http://docs.oracle.com/javase/7/docs/api/javax/annotation/processing/AbstractProcessor.html?is-external=true "class or interface in javax.annotation.processing"){.externalLink}

            `getCompletions, getSupportedAnnotationTypes, getSupportedOptions, init, isInitialized`

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

        -   #### BuckModuleAnnotationProcessor

                public BuckModuleAnnotationProcessor()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getSupportedSourceVersion()}

        -   #### getSupportedSourceVersion

            ``` methodSignature
            public SourceVersion getSupportedSourceVersion()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSupportedSourceVersion` in interface `Processor`

            [Overrides:]{.overrideSpecifyLabel}
            :   `getSupportedSourceVersion` in class `AbstractProcessor`

        []{#process(java.util.Set,javax.annotation.processing.RoundEnvironment)}

        -   #### process

            ``` methodSignature
            public boolean process​(Set<? extends TypeElement> annotations,
                                   RoundEnvironment roundEnv)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `process` in interface `Processor`

            [Specified by:]{.overrideSpecifyLabel}
            :   `process` in class `AbstractProcessor`
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
-   Nested \| 
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

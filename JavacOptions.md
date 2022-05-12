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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java](package-summary.html)
:::

## Class JavacOptions {#class-javacoptions .title title="Class JavacOptions"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.JavacOptions

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`

    ------------------------------------------------------------------------

        public abstract class JavacOptions
        extends Object
        implements AddsToRuleKey

    ::: block
    Represents the command line options that should be passed to javac.
    Note that the options do not include either the classpath or the
    directory for storing class files.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `                     |                       |
        |                       | JavacOptions.Builder` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `Ja                   | ::: block             |
        |                       | vacOptions.SpoolMode` | The method in which   |
        |                       |                       | the compiler output   |
        |                       |                       | is spooled.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor        Description
          ------------------ -------------
          `JavacOptions()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                                          Method                                                                                                                                                   Description
          ------------------------------------------------------------------------------------------ -------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `void`                                                                                     `appendOptionsTo​(OptionsConsumer optionsConsumer,                SourcePathResolverAdapter pathResolver,                ProjectFilesystem filesystem)`    
          `static JavacOptions.Builder`                                                              `builder()`                                                                                                                                               
          `static JavacOptions.Builder`                                                              `builder​(JavacOptions options)`                                                                                                                           
          `abstract Optional<String>`                                                                `getBootclasspath()`                                                                                                                                      
          `abstract List<String>`                                                                    `getExtraArguments()`                                                                                                                                     
          `JavacPluginParams`                                                                        `getJavaAnnotationProcessorParams()`                                                                                                                      
          `JavacLanguageLevelOptions`                                                                `getLanguageLevelOptions()`                                                                                                                               
          `com.google.common.collect.ImmutableList<SourcePath>`                                      `getSourceLevelBootclasspath()`                                                                                                                           
          `protected abstract Map<String,​com.google.common.collect.ImmutableList<PathSourcePath>>`   `getSourceToBootclasspath()`                                                                                                                              
          `JavacOptions.SpoolMode`                                                                   `getSpoolMode()`                                                                                                                                          
          `JavacPluginParams`                                                                        `getStandardJavacPluginParams()`                                                                                                                          
          `protected boolean`                                                                        `isDebug()`                                                                                                                                               
          `protected boolean`                                                                        `isProductionBuild()`                                                                                                                                     
          `protected boolean`                                                                        `isVerbose()`                                                                                                                                             
          `boolean`                                                                                  `trackClassUsage()`                                                                                                                                       
          `boolean`                                                                                  `trackJavacPhaseEvents()`                                                                                                                                 
          `void`                                                                                     `validateOptions​(java.util.function.Function<String,​Boolean> classpathChecker)`                                                                           
          `JavacOptions`                                                                             `withBootclasspath​(String bootclasspath)`                                                                                                                 
          `JavacOptions`                                                                             `withBootclasspathFromContext​(ExtraClasspathProvider extraClasspathProvider)`                                                                             
          `JavacOptions`                                                                             `withExtraArguments​(com.google.common.collect.ImmutableList<String> extraArguments)`                                                                      
          `JavacOptions`                                                                             `withJavaAnnotationProcessorParams​(JavacPluginParams javaAnnotationProcessorParams)`                                                                      
          `JavacOptions`                                                                             `withLanguageLevelOptions​(JavacLanguageLevelOptions languageLevelOptions)`                                                                                

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
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

        -   #### JavacOptions

                public JavacOptions()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getSpoolMode()}

        -   #### getSpoolMode

            ``` methodSignature
            @Default
            public JavacOptions.SpoolMode getSpoolMode()
            ```

        []{#isProductionBuild()}

        -   #### isProductionBuild

            ``` methodSignature
            @Default
            protected boolean isProductionBuild()
            ```

        []{#isVerbose()}

        -   #### isVerbose

            ``` methodSignature
            @Default
            protected boolean isVerbose()
            ```

        []{#getLanguageLevelOptions()}

        -   #### getLanguageLevelOptions

            ``` methodSignature
            @Default
            public JavacLanguageLevelOptions getLanguageLevelOptions()
            ```

        []{#getJavaAnnotationProcessorParams()}

        -   #### getJavaAnnotationProcessorParams

            ``` methodSignature
            @Default
            public JavacPluginParams getJavaAnnotationProcessorParams()
            ```

        []{#getStandardJavacPluginParams()}

        -   #### getStandardJavacPluginParams

            ``` methodSignature
            @Default
            public JavacPluginParams getStandardJavacPluginParams()
            ```

        []{#getExtraArguments()}

        -   #### getExtraArguments

            ``` methodSignature
            public abstract List<String> getExtraArguments()
            ```

        []{#getBootclasspath()}

        -   #### getBootclasspath

            ``` methodSignature
            public abstract Optional<String> getBootclasspath()
            ```

        []{#getSourceToBootclasspath()}

        -   #### getSourceToBootclasspath

            ``` methodSignature
            protected abstract Map<String,​com.google.common.collect.ImmutableList<PathSourcePath>> getSourceToBootclasspath()
            ```

        []{#isDebug()}

        -   #### isDebug

            ``` methodSignature
            protected boolean isDebug()
            ```

        []{#trackClassUsage()}

        -   #### trackClassUsage

            ``` methodSignature
            @Default
            public boolean trackClassUsage()
            ```

        []{#trackJavacPhaseEvents()}

        -   #### trackJavacPhaseEvents

            ``` methodSignature
            @Default
            public boolean trackJavacPhaseEvents()
            ```

        []{#validateOptions(java.util.function.Function)}

        -   #### validateOptions

            ``` methodSignature
            public void validateOptions​(java.util.function.Function<String,​Boolean> classpathChecker)
                                 throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#withBootclasspathFromContext(com.facebook.buck.jvm.java.ExtraClasspathProvider)}

        -   #### withBootclasspathFromContext

            ``` methodSignature
            public JavacOptions withBootclasspathFromContext​(ExtraClasspathProvider extraClasspathProvider)
            ```

        []{#withExtraArguments(com.google.common.collect.ImmutableList)}

        -   #### withExtraArguments

            ``` methodSignature
            public JavacOptions withExtraArguments​(com.google.common.collect.ImmutableList<String> extraArguments)
            ```

        []{#withLanguageLevelOptions(com.facebook.buck.jvm.java.JavacLanguageLevelOptions)}

        -   #### withLanguageLevelOptions

            ``` methodSignature
            public JavacOptions withLanguageLevelOptions​(JavacLanguageLevelOptions languageLevelOptions)
            ```

        []{#withBootclasspath(java.lang.String)}

        -   #### withBootclasspath

            ``` methodSignature
            public JavacOptions withBootclasspath​(@Nullable
                                                  String bootclasspath)
            ```

        []{#withJavaAnnotationProcessorParams(com.facebook.buck.jvm.java.JavacPluginParams)}

        -   #### withJavaAnnotationProcessorParams

            ``` methodSignature
            public JavacOptions withJavaAnnotationProcessorParams​(JavacPluginParams javaAnnotationProcessorParams)
            ```

        []{#getSourceLevelBootclasspath()}

        -   #### getSourceLevelBootclasspath

            ``` methodSignature
            public com.google.common.collect.ImmutableList<SourcePath> getSourceLevelBootclasspath()
            ```

            [Returns:]{.returnLabel}
            :   a list of `SourcePaths` for a particular source level
                extracted from
                [`getSourceToBootclasspath()`](#getSourceToBootclasspath())
                or empty list if bootclasspath for a this source level
                is not defined.

        []{#appendOptionsTo(com.facebook.buck.jvm.java.OptionsConsumer,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### appendOptionsTo

            ``` methodSignature
            public void appendOptionsTo​(OptionsConsumer optionsConsumer,
                                        SourcePathResolverAdapter pathResolver,
                                        ProjectFilesystem filesystem)
            ```

        []{#builder(com.facebook.buck.jvm.java.JavacOptions)}

        -   #### builder

            ``` methodSignature
            public static JavacOptions.Builder builder​(JavacOptions options)
            ```

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static JavacOptions.Builder builder()
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

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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.android](package-summary.html)
:::

## Class WriteAppModuleMetadataStep {#class-writeappmodulemetadatastep .title title="Class WriteAppModuleMetadataStep"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.WriteAppModuleMetadataStep

::: description
-   

    All Implemented Interfaces:
    :   `Step`

    ------------------------------------------------------------------------

        public class WriteAppModuleMetadataStep
        extends Object
        implements Step
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                        Description
          ------------------- ---------------------------- -------------
          `static String`     `CLASS_SECTION_HEADER`        
          `static String`     `DEPS_SECTION_HEADER`         
          `static String`     `ITEM_INDENTATION`            
          `static String`     `LIBRARIES_SECTION_HEADER`    
          `static String`     `MODULE_INDENTATION`          
          `static String`     `TARGETS_SECTION_HEADER`      

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                     Method                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Description
          ------------------------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `StepExecutionResult`                 `execute​(ExecutionContext context)`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    
          `String`                              `getDescription​(ExecutionContext context)`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             
          `String`                              `getShortName()`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       
          `static WriteAppModuleMetadataStep`   `writeModuleMetadata​(Path metadataOut,                    com.google.common.collect.ImmutableMultimap<APKModule,​Path> apkModuleToJarPathMap,                    Optional<com.google.common.collect.ImmutableMultimap<APKModule,​String>> apkModuleToNativeLibraryMap,                    APKModuleGraph apkModuleGraph,                    ProjectFilesystem filesystem,                    Optional<Path> proguardFullConfigFile,                    Optional<Path> proguardMappingFile,                    boolean skipProguard,                    boolean shouldIncludeClasses)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
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
    -   []{#field.detail}

        ### Field Detail

        []{#CLASS_SECTION_HEADER}

        -   #### CLASS_SECTION_HEADER

                public static final String CLASS_SECTION_HEADER

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.android.WriteAppModuleMetadataStep.CLASS_SECTION_HEADER)

        []{#TARGETS_SECTION_HEADER}

        -   #### TARGETS_SECTION_HEADER

                public static final String TARGETS_SECTION_HEADER

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.android.WriteAppModuleMetadataStep.TARGETS_SECTION_HEADER)

        []{#DEPS_SECTION_HEADER}

        -   #### DEPS_SECTION_HEADER

                public static final String DEPS_SECTION_HEADER

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.android.WriteAppModuleMetadataStep.DEPS_SECTION_HEADER)

        []{#LIBRARIES_SECTION_HEADER}

        -   #### LIBRARIES_SECTION_HEADER

                public static final String LIBRARIES_SECTION_HEADER

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.android.WriteAppModuleMetadataStep.LIBRARIES_SECTION_HEADER)

        []{#MODULE_INDENTATION}

        -   #### MODULE_INDENTATION

                public static final String MODULE_INDENTATION

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.android.WriteAppModuleMetadataStep.MODULE_INDENTATION)

        []{#ITEM_INDENTATION}

        -   #### ITEM_INDENTATION

                public static final String ITEM_INDENTATION

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.android.WriteAppModuleMetadataStep.ITEM_INDENTATION)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#writeModuleMetadata(java.nio.file.Path,com.google.common.collect.ImmutableMultimap,java.util.Optional,com.facebook.buck.android.apkmodule.APKModuleGraph,com.facebook.buck.io.filesystem.ProjectFilesystem,java.util.Optional,java.util.Optional,boolean,boolean)}

        -   #### writeModuleMetadata

            ``` methodSignature
            public static WriteAppModuleMetadataStep writeModuleMetadata​(Path metadataOut,
                                                                         com.google.common.collect.ImmutableMultimap<APKModule,​Path> apkModuleToJarPathMap,
                                                                         Optional<com.google.common.collect.ImmutableMultimap<APKModule,​String>> apkModuleToNativeLibraryMap,
                                                                         APKModuleGraph apkModuleGraph,
                                                                         ProjectFilesystem filesystem,
                                                                         Optional<Path> proguardFullConfigFile,
                                                                         Optional<Path> proguardMappingFile,
                                                                         boolean skipProguard,
                                                                         boolean shouldIncludeClasses)
            ```

        []{#execute(com.facebook.buck.core.build.execution.context.ExecutionContext)}

        -   #### execute

            ``` methodSignature
            public StepExecutionResult execute​(ExecutionContext context)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `execute` in interface `Step`

        []{#getShortName()}

        -   #### getShortName

            ``` methodSignature
            public String getShortName()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getShortName` in interface `Step`

            [Returns:]{.returnLabel}
            :   a short name/description for the command, such as
                \"javac\". Should fit on one line.

        []{#getDescription(com.facebook.buck.core.build.execution.context.ExecutionContext)}

        -   #### getDescription

            ``` methodSignature
            public String getDescription​(ExecutionContext context)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDescription` in interface `Step`
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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

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
[Package]{.packageLabelInType} [com.facebook.buck.android](package-summary.html)
:::

## Class SplitZipStep {#class-splitzipstep .title title="Class SplitZipStep"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.SplitZipStep

::: description
-   

    All Implemented Interfaces:
    :   `Step`

    ------------------------------------------------------------------------

        public class SplitZipStep
        extends Object
        implements Step

    ::: block
    Split zipping tool designed to divide input code blobs into a set of
    output jar files such that none will exceed the DexOpt LinearAlloc
    limit or the dx method limit when passed through dx \--dex.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                Description
          ------------------- -------------------- -------------
          `static String`     `SECONDARY_DEX_ID`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `SplitZipStep​(ProjectFilesystem filesystem,             Set<Path> inputPathsToSplit,             Path secondaryJarMetaPath,             Path primaryJarPath,             Path secondaryJarDir,             String secondaryJarPattern,             Path addtionalDexStoreJarMetaPath,             Path additionalDexStoreJarDir,             Optional<Path> proguardFullConfigFile,             Optional<Path> proguardMappingFile,             boolean skipProguard,             com.facebook.buck.android.DexSplitMode dexSplitMode,             Optional<Path> primaryDexScenarioFile,             Optional<Path> primaryDexClassesFile,             Optional<Path> secondaryDexHeadClassesFile,             Optional<Path> secondaryDexTailClassesFile,             com.google.common.collect.ImmutableMultimap<APKModule,​Path> apkModuleToJarPathMap,             com.google.common.collect.ImmutableSortedMap<APKModule,​com.google.common.collect.ImmutableSortedSet<APKModule>> apkModuleMap,             APKModule rootAPKModule,             Path pathToReportDir)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                              Method                                                                                                          Description
          ------------------------------------------------------------------------------ --------------------------------------------------------------------------------------------------------------- -------------
          `StepExecutionResult`                                                          `execute​(ExecutionContext context)`                                                                              
          `String`                                                                       `getDescription​(ExecutionContext context)`                                                                       
          `java.util.function.Supplier<com.google.common.collect.Multimap<Path,​Path>>`   `getOutputToInputsMapSupplier​(Path secondaryOutputDir,                             Path additionalOutputDir)`    
          `String`                                                                       `getShortName()`                                                                                                 

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
    -   []{#field.detail}

        ### Field Detail

        []{#SECONDARY_DEX_ID}

        -   #### SECONDARY_DEX_ID

                public static final String SECONDARY_DEX_ID

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.android.SplitZipStep.SECONDARY_DEX_ID)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.io.filesystem.ProjectFilesystem,java.util.Set,java.nio.file.Path,java.nio.file.Path,java.nio.file.Path,java.lang.String,java.nio.file.Path,java.nio.file.Path,java.util.Optional,java.util.Optional,boolean,com.facebook.buck.android.DexSplitMode,java.util.Optional,java.util.Optional,java.util.Optional,java.util.Optional,com.google.common.collect.ImmutableMultimap,com.google.common.collect.ImmutableSortedMap,com.facebook.buck.android.apkmodule.APKModule,java.nio.file.Path)}

        -   #### SplitZipStep

                public SplitZipStep​(ProjectFilesystem filesystem,
                                    Set<Path> inputPathsToSplit,
                                    Path secondaryJarMetaPath,
                                    Path primaryJarPath,
                                    Path secondaryJarDir,
                                    String secondaryJarPattern,
                                    Path addtionalDexStoreJarMetaPath,
                                    Path additionalDexStoreJarDir,
                                    Optional<Path> proguardFullConfigFile,
                                    Optional<Path> proguardMappingFile,
                                    boolean skipProguard,
                                    com.facebook.buck.android.DexSplitMode dexSplitMode,
                                    Optional<Path> primaryDexScenarioFile,
                                    Optional<Path> primaryDexClassesFile,
                                    Optional<Path> secondaryDexHeadClassesFile,
                                    Optional<Path> secondaryDexTailClassesFile,
                                    com.google.common.collect.ImmutableMultimap<APKModule,​Path> apkModuleToJarPathMap,
                                    com.google.common.collect.ImmutableSortedMap<APKModule,​com.google.common.collect.ImmutableSortedSet<APKModule>> apkModuleMap,
                                    APKModule rootAPKModule,
                                    Path pathToReportDir)

            [Parameters:]{.paramLabel}
            :   `inputPathsToSplit` - Input paths that would otherwise
                have been passed to a single dx \--dex invocation.
            :   `secondaryJarMetaPath` - Output location for the
                metadata text file describing each secondary jar
                artifact.
            :   `primaryJarPath` - Output path for the primary jar file.
            :   `secondaryJarDir` - Output location for secondary jar
                files. Note that this directory may be empty if no
                secondary jar files are needed.
            :   `secondaryJarPattern` - Filename pattern for secondary
                jar files. Pattern contains one %d argument representing
                the enumerated secondary zip count (starting at 1).
            :   `proguardFullConfigFile` - Path to the full generated
                ProGuard configuration, generated by the
                -printconfiguration flag. This is part of the \*output\*
                of ProGuard.
            :   `proguardMappingFile` - Path to the mapping file
                generated by ProGuard\'s obfuscation.
            :   `apkModuleMap` -
            :   `rootAPKModule` -
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#execute(com.facebook.buck.core.build.execution.context.ExecutionContext)}

        -   #### execute

            ``` methodSignature
            public StepExecutionResult execute​(ExecutionContext context)
                                        throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `execute` in interface `Step`

            [Throws:]{.throwsLabel}
            :   `IOException`

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

        []{#getOutputToInputsMapSupplier(java.nio.file.Path,java.nio.file.Path)}

        -   #### getOutputToInputsMapSupplier

            ``` methodSignature
            public java.util.function.Supplier<com.google.common.collect.Multimap<Path,​Path>> getOutputToInputsMapSupplier​(Path secondaryOutputDir,
                                                                                                                                 Path additionalOutputDir)
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

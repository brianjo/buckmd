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
[Package]{.packageLabelInType} [com.facebook.buck.android](package-summary.html)
:::

## Class MergeAndroidResourcesStep {#class-mergeandroidresourcesstep .title title="Class MergeAndroidResourcesStep"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.MergeAndroidResourcesStep

::: description
-   

    All Implemented Interfaces:
    :   `Step`

    ------------------------------------------------------------------------

        public class MergeAndroidResourcesStep
        extends Object
        implements Step
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                                                    Description
          ------------------- -------------------------------------------------------- -------------
          `static class `     `MergeAndroidResourcesStep.DuplicateResourceException`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                      Method                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              Description
          ------------------------------------------------------ --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `static MergeAndroidResourcesStep`                     `createStepForDummyRDotJava​(ProjectFilesystem filesystem,                           SourcePathResolverAdapter pathResolver,                           List<HasAndroidResourceDeps> androidResourceDeps,                           Path outputDir,                           boolean forceFinalResourceIds,                           Optional<String> unionPackage,                           Optional<String> rName,                           boolean useOldStyleableFormat,                           boolean skipNonUnionRDotJava)`                                                                                                              
          `static MergeAndroidResourcesStep`                     `createStepForUberRDotJava​(ProjectFilesystem filesystem,                          SourcePathResolverAdapter pathResolver,                          List<HasAndroidResourceDeps> androidResourceDeps,                          com.google.common.collect.ImmutableList<Path> uberRDotTxt,                          Path outputDir,                          EnumSet<RDotTxtEntry.RType> bannedDuplicateResourceTypes,                          Optional<Path> duplicateResourceWhitelistPath,                          com.google.common.collect.ImmutableList<Path> overrideSymbolsPath,                          Optional<String> unionPackage)`    
          `StepExecutionResult`                                  `execute​(ExecutionContext context)`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  
          `EnumSet<RDotTxtEntry.RType>`                          `getBannedDuplicateResourceTypes()`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  
          `String`                                               `getDescription​(ExecutionContext context)`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           
          `protected Path`                                       `getPathToRDotJava​(String rDotJavaPackage)`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          
          `com.google.common.collect.ImmutableSortedSet<Path>`   `getRDotJavaFiles()`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 
          `String`                                               `getShortName()`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     

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
    -   []{#method.detail}

        ### Method Detail

        []{#createStepForDummyRDotJava(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,java.util.List,java.nio.file.Path,boolean,java.util.Optional,java.util.Optional,boolean,boolean)}

        -   #### createStepForDummyRDotJava

            ``` methodSignature
            public static MergeAndroidResourcesStep createStepForDummyRDotJava​(ProjectFilesystem filesystem,
                                                                               SourcePathResolverAdapter pathResolver,
                                                                               List<HasAndroidResourceDeps> androidResourceDeps,
                                                                               Path outputDir,
                                                                               boolean forceFinalResourceIds,
                                                                               Optional<String> unionPackage,
                                                                               Optional<String> rName,
                                                                               boolean useOldStyleableFormat,
                                                                               boolean skipNonUnionRDotJava)
            ```

        []{#createStepForUberRDotJava(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,java.util.List,com.google.common.collect.ImmutableList,java.nio.file.Path,java.util.EnumSet,java.util.Optional,com.google.common.collect.ImmutableList,java.util.Optional)}

        -   #### createStepForUberRDotJava

            ``` methodSignature
            public static MergeAndroidResourcesStep createStepForUberRDotJava​(ProjectFilesystem filesystem,
                                                                              SourcePathResolverAdapter pathResolver,
                                                                              List<HasAndroidResourceDeps> androidResourceDeps,
                                                                              com.google.common.collect.ImmutableList<Path> uberRDotTxt,
                                                                              Path outputDir,
                                                                              EnumSet<RDotTxtEntry.RType> bannedDuplicateResourceTypes,
                                                                              Optional<Path> duplicateResourceWhitelistPath,
                                                                              com.google.common.collect.ImmutableList<Path> overrideSymbolsPath,
                                                                              Optional<String> unionPackage)
            ```

        []{#getRDotJavaFiles()}

        -   #### getRDotJavaFiles

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<Path> getRDotJavaFiles()
            ```

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

        []{#getPathToRDotJava(java.lang.String)}

        -   #### getPathToRDotJava

            ``` methodSignature
            protected Path getPathToRDotJava​(String rDotJavaPackage)
            ```

        []{#getBannedDuplicateResourceTypes()}

        -   #### getBannedDuplicateResourceTypes

            ``` methodSignature
            public EnumSet<RDotTxtEntry.RType> getBannedDuplicateResourceTypes()
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

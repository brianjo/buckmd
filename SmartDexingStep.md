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

## Class SmartDexingStep {#class-smartdexingstep .title title="Class SmartDexingStep"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.SmartDexingStep

::: description
-   

    All Implemented Interfaces:
    :   `Step`

    ------------------------------------------------------------------------

        public class SmartDexingStep
        extends Object
        implements Step

    ::: block
    Optimized dx command runner which can invoke multiple dx commands in
    parallel and also avoid doing unnecessary dx invocations in the
    first place.
    This is most appropriately represented as a build rule itself (which
    depends on individual dex rules) however this would require
    significant refactoring of AndroidBinaryRule that would be
    disruptive to other initiatives in flight (namely, ApkBuilder). It
    is also debatable that it is even the right course of action given
    that it would require dynamically modifying the DAG.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type     Class                                      Description
          --------------------- ------------------------------------------ -------------
          `static interface `   `SmartDexingStep.DexInputHashesProvider`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field          Description
          ------------------- -------------- -------------
          `static String`     `SHORT_NAME`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   Description
          --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `SmartDexingStep​(AndroidPlatformTarget androidPlatformTarget,                BuildContext buildContext,                ProjectFilesystem filesystem,                Optional<Path> primaryOutputPath,                Optional<java.util.function.Supplier<Set<Path>>> primaryInputsToDex,                Optional<java.util.function.Supplier<List<String>>> primaryDexWeightsSupplier,                Optional<Path> secondaryOutputDir,                Optional<java.util.function.Supplier<com.google.common.collect.Multimap<Path,​Path>>> secondaryInputsToDex,                SmartDexingStep.DexInputHashesProvider dexInputHashesProvider,                Path successDir,                EnumSet<DxStep.Option> dxOptions,                com.google.common.util.concurrent.ListeningExecutorService executorService,                int xzCompressionLevel,                Optional<String> dxMaxHeapSize,                String dexTool,                boolean desugarInterfaceMethods,                boolean useDexBuckedId,                Optional<Set<Path>> additonalDesugarDeps,                BuildTarget buildTarget,                Optional<Integer> minSdkVersion)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type       Method                                       Description
          ----------------------- -------------------------------------------- -------------
          `static int`            `determineOptimalThreadCount()`               
          `StepExecutionResult`   `execute​(ExecutionContext context)`           
          `String`                `getDescription​(ExecutionContext context)`    
          `String`                `getShortName()`                              

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

        []{#SHORT_NAME}

        -   #### SHORT_NAME

                public static final String SHORT_NAME

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.android.SmartDexingStep.SHORT_NAME)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.android.toolchain.AndroidPlatformTarget,com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.io.filesystem.ProjectFilesystem,java.util.Optional,java.util.Optional,java.util.Optional,java.util.Optional,java.util.Optional,com.facebook.buck.android.SmartDexingStep.DexInputHashesProvider,java.nio.file.Path,java.util.EnumSet,com.google.common.util.concurrent.ListeningExecutorService,int,java.util.Optional,java.lang.String,boolean,boolean,java.util.Optional,com.facebook.buck.core.model.BuildTarget,java.util.Optional)}

        -   #### SmartDexingStep

                public SmartDexingStep​(AndroidPlatformTarget androidPlatformTarget,
                                       BuildContext buildContext,
                                       ProjectFilesystem filesystem,
                                       Optional<Path> primaryOutputPath,
                                       Optional<java.util.function.Supplier<Set<Path>>> primaryInputsToDex,
                                       Optional<java.util.function.Supplier<List<String>>> primaryDexWeightsSupplier,
                                       Optional<Path> secondaryOutputDir,
                                       Optional<java.util.function.Supplier<com.google.common.collect.Multimap<Path,​Path>>> secondaryInputsToDex,
                                       SmartDexingStep.DexInputHashesProvider dexInputHashesProvider,
                                       Path successDir,
                                       EnumSet<DxStep.Option> dxOptions,
                                       com.google.common.util.concurrent.ListeningExecutorService executorService,
                                       int xzCompressionLevel,
                                       Optional<String> dxMaxHeapSize,
                                       String dexTool,
                                       boolean desugarInterfaceMethods,
                                       boolean useDexBuckedId,
                                       Optional<Set<Path>> additonalDesugarDeps,
                                       BuildTarget buildTarget,
                                       Optional<Integer> minSdkVersion)

            [Parameters:]{.paramLabel}
            :   `primaryOutputPath` - Path for the primary dex artifact.
            :   `primaryInputsToDex` - Set of paths to include as inputs
                for the primary dex artifact.
            :   `secondaryOutputDir` - Directory path for the secondary
                dex artifacts, if there are any. Note that this
                directory will be pruned such that only those secondary
                outputs generated by this command will remain in the
                directory!
            :   `secondaryInputsToDex` - List of paths to input jar
                files, to use as dx input, keyed by the corresponding
                output dex file. Note that for each output file (key), a
                separate dx invocation will be started with the
                corresponding jar files (value) as the input.
            :   `successDir` - Directory where success artifacts are
                written.
            :   `executorService` - The thread pool to execute the dx
                command on.
            :   `minSdkVersion` -
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#determineOptimalThreadCount()}

        -   #### determineOptimalThreadCount

            ``` methodSignature
            public static int determineOptimalThreadCount()
            ```

            [Returns:]{.returnLabel}
            :   Optimal (in terms of both memory and performance) number
                of parallel threads to run dexer. The implementation
                uses running machine hardware characteristics to
                determine this.

        []{#execute(com.facebook.buck.core.build.execution.context.ExecutionContext)}

        -   #### execute

            ``` methodSignature
            public StepExecutionResult execute​(ExecutionContext context)
                                        throws IOException,
                                               InterruptedException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `execute` in interface `Step`

            [Throws:]{.throwsLabel}
            :   `IOException`
            :   `InterruptedException`

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
-   [Nested](#nested.class.summary) \| 
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

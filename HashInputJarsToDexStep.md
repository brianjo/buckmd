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
[Package]{.packageLabelInType} [com.facebook.buck.android](package-summary.html)
:::

## Class HashInputJarsToDexStep {#class-hashinputjarstodexstep .title title="Class HashInputJarsToDexStep"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.step.AbstractExecutionStep](../step/AbstractExecutionStep.html "class in com.facebook.buck.step")

    -   -   com.facebook.buck.android.HashInputJarsToDexStep

::: description
-   

    All Implemented Interfaces:
    :   `SmartDexingStep.DexInputHashesProvider`, `Step`

    ------------------------------------------------------------------------

        public class HashInputJarsToDexStep
        extends AbstractExecutionStep
        implements SmartDexingStep.DexInputHashesProvider

    ::: block
    Step responsible for hashing dex inputs to be passed to
    [`SmartDexingStep`](SmartDexingStep.html "class in com.facebook.buck.android").
    It goes through each dex input, looks at the classes that went into
    that jar, and uses the class hashes collected in
    [`AndroidPackageableCollection`](packageable/AndroidPackageableCollection.html "interface in com.facebook.buck.android.packageable")
    to calculate the final hash of the input.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                 Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `HashInputJarsToDexStep​(ProjectFilesystem filesystem,                       java.util.function.Supplier<Set<Path>> primaryInputsToDex,                       Optional<java.util.function.Supplier<com.google.common.collect.Multimap<Path,​Path>>> secondaryOutputToInputs,                       java.util.function.Supplier<com.google.common.collect.ImmutableMap<String,​com.google.common.hash.HashCode>> classNamesToHashesSupplier)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                             Method                                Description
          ------------------------------------------------------------- ------------------------------------- -------------
          `StepExecutionResult`                                         `execute​(ExecutionContext context)`    
          `com.google.common.collect.ImmutableMap<Path,​Sha1HashCode>`   `getDexInputHashes()`                  

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.step.AbstractExecutionStep}

            ### Methods inherited from class com.facebook.buck.step.[AbstractExecutionStep](../step/AbstractExecutionStep.html "class in com.facebook.buck.step")

            `getDescription, getShortName`

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

        []{#<init>(com.facebook.buck.io.filesystem.ProjectFilesystem,java.util.function.Supplier,java.util.Optional,java.util.function.Supplier)}

        -   #### HashInputJarsToDexStep

                public HashInputJarsToDexStep​(ProjectFilesystem filesystem,
                                              java.util.function.Supplier<Set<Path>> primaryInputsToDex,
                                              Optional<java.util.function.Supplier<com.google.common.collect.Multimap<Path,​Path>>> secondaryOutputToInputs,
                                              java.util.function.Supplier<com.google.common.collect.ImmutableMap<String,​com.google.common.hash.HashCode>> classNamesToHashesSupplier)
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

            [Specified by:]{.overrideSpecifyLabel}
            :   `execute` in class `AbstractExecutionStep`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getDexInputHashes()}

        -   #### getDexInputHashes

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<Path,​Sha1HashCode> getDexInputHashes()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDexInputHashes` in
                interface `SmartDexingStep.DexInputHashesProvider`
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

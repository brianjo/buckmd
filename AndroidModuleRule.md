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

-   [Overview](../../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../../index-all.html)
-   [Help](../../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.features.project.intellij.lang.android](package-summary.html)
:::

## Class AndroidModuleRule\<T extends [BuildRuleArg](../../../../../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")\> {#class-androidmodulerulet-extends-buildrulearg .title title="Class AndroidModuleRule"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.features.project.intellij.BaseIjModuleRule](../../BaseIjModuleRule.html "class in com.facebook.buck.features.project.intellij")\<T\>

    -   -   com.facebook.buck.features.project.intellij.lang.android.AndroidModuleRule\<T\>

::: description
-   

    All Implemented Interfaces:
    :   `IjModuleRule<T>`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `AndroidBinaryModuleRule`, `AndroidLibraryModuleRule`,
        `AndroidResourceModuleRule`, `RobolectricTestModuleRule`

    ------------------------------------------------------------------------

        public abstract class AndroidModuleRule<T extends BuildRuleArg>
        extends BaseIjModuleRule<T>

    ::: block
    Android IntelliJ rule
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.features.project.intellij.BaseIjModuleRule}

            ### Fields inherited from class com.facebook.buck.features.project.intellij.[BaseIjModuleRule](../../BaseIjModuleRule.html "class in com.facebook.buck.features.project.intellij")

            `moduleFactoryResolver, projectConfig, projectFilesystem`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                                                                                                                                                                                                                        Description
          -------------- ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `protected `   `AndroidModuleRule​(ProjectFilesystem projectFilesystem,                  IjModuleFactoryResolver moduleFactoryResolver,                  IjProjectConfig projectConfig,                  AndroidProjectType androidProjectType)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                           Description
          ------------------- ---------------------------------------------------------------- -------------
          `void`              `apply​(TargetNode<T> target,      ModuleBuildContext context)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.features.project.intellij.BaseIjModuleRule}

            ### Methods inherited from class com.facebook.buck.features.project.intellij.[BaseIjModuleRule](../../BaseIjModuleRule.html "class in com.facebook.buck.features.project.intellij")

            `addDepsAndSources, addDepsAndSources, addDepsAndTestSources, addDepsAndTestSources, addResourceFolders, addResourceFolders, addSourceFolders, applyDuringAggregation, getResourcePaths, getResourcePaths, getResourcesRootsToResources, getSourceFoldersToInputsIndex`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.features.project.intellij.model.IjModuleRule}

            ### Methods inherited from interface com.facebook.buck.features.project.intellij.model.[IjModuleRule](../../model/IjModuleRule.html "interface in com.facebook.buck.features.project.intellij.model")

            `detectModuleType, getDescriptionClass`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.features.project.intellij.model.IjModuleFactoryResolver,com.facebook.buck.features.project.intellij.model.IjProjectConfig,com.facebook.buck.features.project.intellij.lang.android.AndroidProjectType)}

        -   #### AndroidModuleRule

                protected AndroidModuleRule​(ProjectFilesystem projectFilesystem,
                                            IjModuleFactoryResolver moduleFactoryResolver,
                                            IjProjectConfig projectConfig,
                                            AndroidProjectType androidProjectType)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#apply(com.facebook.buck.core.model.targetgraph.TargetNode,com.facebook.buck.features.project.intellij.ModuleBuildContext)}

        -   #### apply

            ``` methodSignature
            public void apply​(TargetNode<T> target,
                              ModuleBuildContext context)
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

-   [Overview](../../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../../index-all.html)
-   [Help](../../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../../allclasses.html)

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

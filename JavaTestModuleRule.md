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
[Package]{.packageLabelInType} [com.facebook.buck.features.project.intellij.lang.java](package-summary.html)
:::

## Class JavaTestModuleRule {#class-javatestmodulerule .title title="Class JavaTestModuleRule"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.features.project.intellij.BaseIjModuleRule](../../BaseIjModuleRule.html "class in com.facebook.buck.features.project.intellij")\<[JavaTestDescription.CoreArg](../../../../../jvm/java/JavaTestDescription.CoreArg.html "interface in com.facebook.buck.jvm.java")\>

    -   -   com.facebook.buck.features.project.intellij.lang.java.JavaTestModuleRule

::: description
-   

    All Implemented Interfaces:
    :   `IjModuleRule<JavaTestDescription.CoreArg>`

    ------------------------------------------------------------------------

        public class JavaTestModuleRule
        extends BaseIjModuleRule<JavaTestDescription.CoreArg>
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

          Constructor                                                                                                                                                                                                                      Description
          -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `JavaTestModuleRule​(ProjectFilesystem projectFilesystem,                   IjModuleFactoryResolver moduleFactoryResolver,                   IjProjectConfig projectConfig,                   JavaPackageFinder packageFinder)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                  Method                                                                                                                           Description
          -------------------------------------------------- -------------------------------------------------------------------------------------------------------------------------------- -------------
          `void`                                             `apply​(TargetNode<JavaTestDescription.CoreArg> target,      ModuleBuildContext context)`                                          
          `void`                                             `applyDuringAggregation​(AggregationContext context,                       TargetNode<JavaTestDescription.CoreArg> targetNode)`    
          `IjModuleType`                                     `detectModuleType​(TargetNode<JavaTestDescription.CoreArg> targetNode)`                                                            
          `Class<? extends DescriptionWithTargetGraph<?>>`   `getDescriptionClass()`                                                                                                           

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.features.project.intellij.BaseIjModuleRule}

            ### Methods inherited from class com.facebook.buck.features.project.intellij.[BaseIjModuleRule](../../BaseIjModuleRule.html "class in com.facebook.buck.features.project.intellij")

            `addDepsAndSources, addDepsAndSources, addDepsAndTestSources, addDepsAndTestSources, addResourceFolders, addResourceFolders, addSourceFolders, getResourcePaths, getResourcePaths, getResourcesRootsToResources, getSourceFoldersToInputsIndex`

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

        []{#<init>(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.features.project.intellij.model.IjModuleFactoryResolver,com.facebook.buck.features.project.intellij.model.IjProjectConfig,com.facebook.buck.jvm.core.JavaPackageFinder)}

        -   #### JavaTestModuleRule

                public JavaTestModuleRule​(ProjectFilesystem projectFilesystem,
                                          IjModuleFactoryResolver moduleFactoryResolver,
                                          IjProjectConfig projectConfig,
                                          JavaPackageFinder packageFinder)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getDescriptionClass()}

        -   #### getDescriptionClass

            ``` methodSignature
            public Class<? extends DescriptionWithTargetGraph<?>> getDescriptionClass()
            ```

        []{#apply(com.facebook.buck.core.model.targetgraph.TargetNode,com.facebook.buck.features.project.intellij.ModuleBuildContext)}

        -   #### apply

            ``` methodSignature
            public void apply​(TargetNode<JavaTestDescription.CoreArg> target,
                              ModuleBuildContext context)
            ```

        []{#detectModuleType(com.facebook.buck.core.model.targetgraph.TargetNode)}

        -   #### detectModuleType

            ``` methodSignature
            public IjModuleType detectModuleType​(TargetNode<JavaTestDescription.CoreArg> targetNode)
            ```

        []{#applyDuringAggregation(com.facebook.buck.features.project.intellij.aggregation.AggregationContext,com.facebook.buck.core.model.targetgraph.TargetNode)}

        -   #### applyDuringAggregation

            ``` methodSignature
            public void applyDuringAggregation​(AggregationContext context,
                                               TargetNode<JavaTestDescription.CoreArg> targetNode)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `applyDuringAggregation` in
                interface `IjModuleRule<JavaTestDescription.CoreArg>`

            [Overrides:]{.overrideSpecifyLabel}
            :   `applyDuringAggregation` in
                class `BaseIjModuleRule<JavaTestDescription.CoreArg>`
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

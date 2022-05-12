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

## Class AndroidLibraryModuleRule {#class-androidlibrarymodulerule .title title="Class AndroidLibraryModuleRule"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.features.project.intellij.BaseIjModuleRule](../../BaseIjModuleRule.html "class in com.facebook.buck.features.project.intellij")\<T\>

    -   -   [com.facebook.buck.features.project.intellij.lang.android.AndroidModuleRule](AndroidModuleRule.html "class in com.facebook.buck.features.project.intellij.lang.android")\<[AndroidLibraryDescription.CoreArg](../../../../../android/AndroidLibraryDescription.CoreArg.html "interface in com.facebook.buck.android")\>

        -   -   com.facebook.buck.features.project.intellij.lang.android.AndroidLibraryModuleRule

::: description
-   

    All Implemented Interfaces:
    :   `IjModuleRule<AndroidLibraryDescription.CoreArg>`

    ------------------------------------------------------------------------

        public class AndroidLibraryModuleRule
        extends AndroidModuleRule<AndroidLibraryDescription.CoreArg>
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

          Constructor                                                                                                                                                                                     Description
          ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `AndroidLibraryModuleRule​(ProjectFilesystem projectFilesystem,                         IjModuleFactoryResolver moduleFactoryResolver,                         IjProjectConfig projectConfig)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                  Method                                                                                                                                 Description
          -------------------------------------------------- -------------------------------------------------------------------------------------------------------------------------------------- -------------
          `void`                                             `apply​(TargetNode<AndroidLibraryDescription.CoreArg> target,      ModuleBuildContext context)`                                          
          `void`                                             `applyDuringAggregation​(AggregationContext context,                       TargetNode<AndroidLibraryDescription.CoreArg> targetNode)`    
          `IjModuleType`                                     `detectModuleType​(TargetNode<AndroidLibraryDescription.CoreArg> targetNode)`                                                            
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

        []{#<init>(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.features.project.intellij.model.IjModuleFactoryResolver,com.facebook.buck.features.project.intellij.model.IjProjectConfig)}

        -   #### AndroidLibraryModuleRule

                public AndroidLibraryModuleRule​(ProjectFilesystem projectFilesystem,
                                                IjModuleFactoryResolver moduleFactoryResolver,
                                                IjProjectConfig projectConfig)
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
            public void apply​(TargetNode<AndroidLibraryDescription.CoreArg> target,
                              ModuleBuildContext context)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `apply` in
                interface `IjModuleRule<AndroidLibraryDescription.CoreArg>`

            [Overrides:]{.overrideSpecifyLabel}
            :   `apply` in
                class `AndroidModuleRule<AndroidLibraryDescription.CoreArg>`

        []{#applyDuringAggregation(com.facebook.buck.features.project.intellij.aggregation.AggregationContext,com.facebook.buck.core.model.targetgraph.TargetNode)}

        -   #### applyDuringAggregation

            ``` methodSignature
            public void applyDuringAggregation​(AggregationContext context,
                                               TargetNode<AndroidLibraryDescription.CoreArg> targetNode)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `applyDuringAggregation` in
                interface `IjModuleRule<AndroidLibraryDescription.CoreArg>`

            [Overrides:]{.overrideSpecifyLabel}
            :   `applyDuringAggregation` in
                class `BaseIjModuleRule<AndroidLibraryDescription.CoreArg>`

        []{#detectModuleType(com.facebook.buck.core.model.targetgraph.TargetNode)}

        -   #### detectModuleType

            ``` methodSignature
            public IjModuleType detectModuleType​(TargetNode<AndroidLibraryDescription.CoreArg> targetNode)
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

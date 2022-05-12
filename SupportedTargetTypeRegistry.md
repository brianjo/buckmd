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
[Package]{.packageLabelInType} [com.facebook.buck.features.project.intellij](package-summary.html)
:::

## Class SupportedTargetTypeRegistry {#class-supportedtargettyperegistry .title title="Class SupportedTargetTypeRegistry"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.project.intellij.SupportedTargetTypeRegistry

::: description
-   

    ------------------------------------------------------------------------

        public class SupportedTargetTypeRegistry
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                          Description
          -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `SupportedTargetTypeRegistry​(ProjectFilesystem projectFilesystem,                            IjModuleFactoryResolver moduleFactoryResolver,                            IjProjectConfig projectConfig,                            JavaPackageFinder packageFinder)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                  Description
          ------------------- --------------------------------------------------------------------------------------- -------------
          `static boolean`    `areTargetTypesEqual​(Set<Class<? extends DescriptionWithTargetGraph<?>>> otherTypes)`    
          `IjModuleRule<?>`   `getModuleRuleByTargetNodeType​(Class<?> targetNodeType)`                                 
          `static boolean`    `isTargetTypeSupported​(Class<?> descriptionClass)`                                       

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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.features.project.intellij.model.IjModuleFactoryResolver,com.facebook.buck.features.project.intellij.model.IjProjectConfig,com.facebook.buck.jvm.core.JavaPackageFinder)}

        -   #### SupportedTargetTypeRegistry

                public SupportedTargetTypeRegistry​(ProjectFilesystem projectFilesystem,
                                                   IjModuleFactoryResolver moduleFactoryResolver,
                                                   IjProjectConfig projectConfig,
                                                   JavaPackageFinder packageFinder)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#isTargetTypeSupported(java.lang.Class)}

        -   #### isTargetTypeSupported

            ``` methodSignature
            public static boolean isTargetTypeSupported​(Class<?> descriptionClass)
            ```

        []{#areTargetTypesEqual(java.util.Set)}

        -   #### areTargetTypesEqual

            ``` methodSignature
            public static boolean areTargetTypesEqual​(Set<Class<? extends DescriptionWithTargetGraph<?>>> otherTypes)
            ```

        []{#getModuleRuleByTargetNodeType(java.lang.Class)}

        -   #### getModuleRuleByTargetNodeType

            ``` methodSignature
            public IjModuleRule<?> getModuleRuleByTargetNodeType​(Class<?> targetNodeType)
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

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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.features.project.intellij.model](package-summary.html)
:::

## Class IjModule {#class-ijmodule .title title="Class IjModule"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.project.intellij.model.IjModule

::: description
-   

    All Implemented Interfaces:
    :   `IjProjectElement`

    ------------------------------------------------------------------------

        public abstract class IjModule
        extends Object
        implements IjProjectElement

    ::: block
    Represents a single IntelliJ module.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                Description
          ------------------- -------------------- -------------
          `static class `     `IjModule.Builder`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor    Description
          -------------- -------------
          `IjModule()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                               Method                                                                                                           Description
          ------------------------------------------------------------------------------- ---------------------------------------------------------------------------------------------------------------- -------------
          `void`                                                                          `addAsDependency​(DependencyType dependencyType,                IjDependencyListBuilder dependencyListBuilder)`    
          `static IjModule.Builder`                                                       `builder()`                                                                                                       
          `protected void`                                                                `checkDependencyConsistency()`                                                                                    
          `boolean`                                                                       `equals​(Object another)`                                                                                          
          `abstract Optional<IjModuleAndroidFacet>`                                       `getAndroidFacet()`                                                                                               
          `abstract Optional<Path>`                                                       `getCompilerOutputPath()`                                                                                         
          `abstract com.google.common.collect.ImmutableMap<BuildTarget,​DependencyType>`   `getDependencies()`                                                                                               
          `abstract com.google.common.collect.ImmutableSet<IjLibrary>`                    `getExtraLibraryDependencies()`                                                                                   
          `abstract com.google.common.collect.ImmutableSet<Path>`                         `getExtraModuleDependencies()`                                                                                    
          `abstract com.google.common.collect.ImmutableList<IjFolder>`                    `getFolders()`                                                                                                    
          `abstract com.google.common.collect.ImmutableList<IjFolder>`                    `getGeneratedSourceCodeFolders()`                                                                                 
          `abstract Optional<String>`                                                     `getLanguageLevel()`                                                                                              
          `abstract Optional<Path>`                                                       `getMetaInfDirectory()`                                                                                           
          `abstract Path`                                                                 `getModuleBasePath()`                                                                                             
          `abstract IjModuleType`                                                         `getModuleType()`                                                                                                 
          `String`                                                                        `getName()`                                                                                                       
          `abstract com.google.common.collect.ImmutableSet<BuildTarget>`                  `getNonSourceBuildTargets()`                                                                                      
          `abstract com.google.common.collect.ImmutableSet<BuildTarget>`                  `getTargets()`                                                                                                    
          `abstract Map<BuildTarget,​List<IjFolder>>`                                      `getTargetsToGeneratedSourcesMap()`                                                                               
          `int`                                                                           `hashCode()`                                                                                                      

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

            `clone, finalize, getClass, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### IjModule

                public IjModule()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getName()}

        -   #### getName

            ``` methodSignature
            @Derived
            public String getName()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getName` in interface `IjProjectElement`

            [Returns:]{.returnLabel}
            :   unique string identifying the element. This will be used
                by modules to refer to it.

        []{#getTargets()}

        -   #### getTargets

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSet<BuildTarget> getTargets()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTargets` in interface `IjProjectElement`

            [Returns:]{.returnLabel}
            :   set of targets this element corresponds to in the
                IntelliJ project.

        []{#getNonSourceBuildTargets()}

        -   #### getNonSourceBuildTargets

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSet<BuildTarget> getNonSourceBuildTargets()
            ```

        []{#getTargetsToGeneratedSourcesMap()}

        -   #### getTargetsToGeneratedSourcesMap

            ``` methodSignature
            public abstract Map<BuildTarget,​List<IjFolder>> getTargetsToGeneratedSourcesMap()
            ```

        []{#getModuleBasePath()}

        -   #### getModuleBasePath

            ``` methodSignature
            public abstract Path getModuleBasePath()
            ```

            [Returns:]{.returnLabel}
            :   path to the top-most directory the module is responsible
                for.

        []{#getFolders()}

        -   #### getFolders

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<IjFolder> getFolders()
            ```

            [Returns:]{.returnLabel}
            :   paths to various directories the module is responsible
                for.

        []{#getDependencies()}

        -   #### getDependencies

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableMap<BuildTarget,​DependencyType> getDependencies()
            ```

            [Returns:]{.returnLabel}
            :   map of
                [`BuildTarget`](../../../../core/model/BuildTarget.html "class in com.facebook.buck.core.model")s
                the module depends on and information on whether it\'s a
                test-only dependency or not.

        []{#getAndroidFacet()}

        -   #### getAndroidFacet

            ``` methodSignature
            public abstract Optional<IjModuleAndroidFacet> getAndroidFacet()
            ```

        []{#getExtraLibraryDependencies()}

        -   #### getExtraLibraryDependencies

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSet<IjLibrary> getExtraLibraryDependencies()
            ```

            [Returns:]{.returnLabel}
            :   a set of IjLibrary that the module requires to index all
                symbols correctly.

        []{#getExtraModuleDependencies()}

        -   #### getExtraModuleDependencies

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSet<Path> getExtraModuleDependencies()
            ```

            [Returns:]{.returnLabel}
            :   a set of module paths that the module requires to index
                correctly.

        []{#getGeneratedSourceCodeFolders()}

        -   #### getGeneratedSourceCodeFolders

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<IjFolder> getGeneratedSourceCodeFolders()
            ```

            [Returns:]{.returnLabel}
            :   Folders which contain the generated source code.

        []{#getLanguageLevel()}

        -   #### getLanguageLevel

            ``` methodSignature
            public abstract Optional<String> getLanguageLevel()
            ```

        []{#getModuleType()}

        -   #### getModuleType

            ``` methodSignature
            public abstract IjModuleType getModuleType()
            ```

        []{#getMetaInfDirectory()}

        -   #### getMetaInfDirectory

            ``` methodSignature
            public abstract Optional<Path> getMetaInfDirectory()
            ```

        []{#getCompilerOutputPath()}

        -   #### getCompilerOutputPath

            ``` methodSignature
            public abstract Optional<Path> getCompilerOutputPath()
            ```

        []{#checkDependencyConsistency()}

        -   #### checkDependencyConsistency

            ``` methodSignature
            @Check
            protected void checkDependencyConsistency()
            ```

        []{#addAsDependency(com.facebook.buck.features.project.intellij.model.DependencyType,com.facebook.buck.features.project.intellij.IjDependencyListBuilder)}

        -   #### addAsDependency

            ``` methodSignature
            public void addAsDependency​(DependencyType dependencyType,
                                        IjDependencyListBuilder dependencyListBuilder)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `addAsDependency` in interface `IjProjectElement`

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `Object`

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(Object another)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `Object`

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static IjModule.Builder builder()
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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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

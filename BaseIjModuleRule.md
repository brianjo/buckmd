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
[Package]{.packageLabelInType} [com.facebook.buck.features.project.intellij](package-summary.html)
:::

## Class BaseIjModuleRule\<T extends [BuildRuleArg](../../../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")\> {#class-baseijmodulerulet-extends-buildrulearg .title title="Class BaseIjModuleRule"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.project.intellij.BaseIjModuleRule\<T\>

::: description
-   

    All Implemented Interfaces:
    :   `IjModuleRule<T>`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `AndroidModuleRule`, `CxxLibraryModuleRule`,
        `CxxTestModuleRule`, `GroovyLibraryModuleRule`,
        `GroovyTestModuleRule`, `JavaBinaryModuleRule`,
        `JavaLibraryModuleRule`, `JavaTestModuleRule`,
        `KotlinLibraryModuleRule`, `KotlinTestModuleRule`,
        `PythonLibraryModuleRule`, `PythonTestModuleRule`,
        `ScalaLibraryModuleRule`, `ScalaTestModuleRule`

    ------------------------------------------------------------------------

        public abstract class BaseIjModuleRule<T extends BuildRuleArg>
        extends Object
        implements IjModuleRule<T>

    ::: block
    Base class for IntelliJ module rules
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                     Field                     Description
          ------------------------------------- ------------------------- -------------
          `protected IjModuleFactoryResolver`   `moduleFactoryResolver`    
          `protected IjProjectConfig`           `projectConfig`            
          `protected ProjectFilesystem`         `projectFilesystem`        

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                                                                                                                                                             Description
          -------------- ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `protected `   `BaseIjModuleRule​(ProjectFilesystem projectFilesystem,                 IjModuleFactoryResolver moduleFactoryResolver,                 IjProjectConfig projectConfig)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `protected void`      | `addDepsA             |                       |
        |                       | ndSources​(TargetNode< |                       |
        |                       | T> targetNode,        |                       |
        |                       |            boolean wa |                       |
        |                       | ntsPackagePrefix,     |                       |
        |                       |               ModuleB |                       |
        |                       | uildContext context)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected void`      | `a                    |                       |
        |                       | ddDepsAndSources​(Targ |                       |
        |                       | etNode<T> targetNode, |                       |
        |                       |                   boo |                       |
        |                       | lean wantsPackagePref |                       |
        |                       | ix,                   |                       |
        |                       | ModuleBuildContext co |                       |
        |                       | ntext,                |                       |
        |                       |    com.google.common. |                       |
        |                       | collect.ImmutableSet< |                       |
        |                       | Path> resourcePaths)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected void`      | `addDepsAndTestSource |                       |
        |                       | s​(TargetNode<T> targe |                       |
        |                       | tNode,                |                       |
        |                       |        boolean wantsP |                       |
        |                       | ackagePrefix,         |                       |
        |                       |               ModuleB |                       |
        |                       | uildContext context)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected void`      | `addDepsAndTestSou    |                       |
        |                       | rces​(TargetNode<T> ta |                       |
        |                       | rgetNode,             |                       |
        |                       |           boolean wan |                       |
        |                       | tsPackagePrefix,      |                       |
        |                       |                  Modu |                       |
        |                       | leBuildContext contex |                       |
        |                       | t,                    |                       |
        |                       |    com.google.common. |                       |
        |                       | collect.ImmutableSet< |                       |
        |                       | Path> resourcePaths)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected void`      | `                     |                       |
        |                       | addResourceFolders​(Ij |                       |
        |                       | ResourceFolderType ij |                       |
        |                       | ResourceFolderType,   |                       |
        |                       |                  com. |                       |
        |                       | google.common.collect |                       |
        |                       | .ImmutableCollection< |                       |
        |                       | Path> resourcePaths,  |                       |
        |                       |                   Pat |                       |
        |                       | h resourcesRoot,      |                       |
        |                       |               ModuleB |                       |
        |                       | uildContext context)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected void`      | `addResourceFolders​(  |                       |
        |                       | ResourceFolderFactory |                       |
        |                       |  factory,             |                       |
        |                       |        com.google.com |                       |
        |                       | mon.collect.Immutable |                       |
        |                       | Multimap<Path,​Path> f |                       |
        |                       | oldersToInputsIndex,  |                       |
        |                       |                   Pat |                       |
        |                       | h resourcesRoot,      |                       |
        |                       |               ModuleB |                       |
        |                       | uildContext context)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected void`      | `addSourceFold        | ::: block             |
        |                       | ers​(IJFolderFactory f | Add the set of input  |
        |                       | actory,               | paths to the          |
        |                       |    com.google.common. | [`IjM                 |
        |                       | collect.ImmutableMult | odule.Builder`](model |
        |                       | imap<Path,​Path> folde | /IjModule.Builder.htm |
        |                       | rsToInputsIndex,      | l "class in com.faceb |
        |                       |             boolean w | ook.buck.features.pro |
        |                       | antsPackagePrefix,    | ject.intellij.model") |
        |                       |               ModuleB | as source folders.    |
        |                       | uildContext context)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `applyDuringAggr      |                       |
        |                       | egation​(AggregationCo |                       |
        |                       | ntext context,        |                       |
        |                       |                 Targe |                       |
        |                       | tNode<T> targetNode)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected com        | `getResour            |                       |
        | .google.common.collec | cePaths​(Collection<So |                       |
        | t.ImmutableSet<Path>` | urcePath> resources)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected com        | `get                  |                       |
        | .google.common.collec | ResourcePaths​(Collect |                       |
        | t.ImmutableSet<Path>` | ion<SourcePath> resou |                       |
        |                       | rces,                 |                       |
        |                       |  Path resourcesRoot)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `pr                   | `get                  |                       |
        | otected com.google.co | ResourcesRootsToResou |                       |
        | mmon.collect.Immutabl | rces​(JavaPackageFinde |                       |
        | eMultimap<Path,​Path>` | r packageFinder,      |                       |
        |                       |                       |                       |
        |                       |    com.google.common. |                       |
        |                       | collect.ImmutableSet< |                       |
        |                       | Path> resourcePaths)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected            | `getSo                | ::: block             |
        |  static com.google.co | urceFoldersToInputsIn | Calculate the set of  |
        | mmon.collect.Immutabl | dex​(com.google.common | directories           |
        | eMultimap<Path,​Path>` | .collect.ImmutableCol | containing inputs to  |
        |                       | lection<Path> paths)` | the target.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.features.project.intellij.model.IjModuleRule}

            ### Methods inherited from interface com.facebook.buck.features.project.intellij.model.[IjModuleRule](model/IjModuleRule.html "interface in com.facebook.buck.features.project.intellij.model")

            `apply, detectModuleType, getDescriptionClass`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#projectFilesystem}

        -   #### projectFilesystem

                protected final ProjectFilesystem projectFilesystem

        []{#moduleFactoryResolver}

        -   #### moduleFactoryResolver

                protected final IjModuleFactoryResolver moduleFactoryResolver

        []{#projectConfig}

        -   #### projectConfig

                protected final IjProjectConfig projectConfig
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.features.project.intellij.model.IjModuleFactoryResolver,com.facebook.buck.features.project.intellij.model.IjProjectConfig)}

        -   #### BaseIjModuleRule

                protected BaseIjModuleRule​(ProjectFilesystem projectFilesystem,
                                           IjModuleFactoryResolver moduleFactoryResolver,
                                           IjProjectConfig projectConfig)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getSourceFoldersToInputsIndex(com.google.common.collect.ImmutableCollection)}

        -   #### getSourceFoldersToInputsIndex

            ``` methodSignature
            protected static com.google.common.collect.ImmutableMultimap<Path,​Path> getSourceFoldersToInputsIndex​(com.google.common.collect.ImmutableCollection<Path> paths)
            ```

            ::: block
            Calculate the set of directories containing inputs to the
            target.
            :::

            [Parameters:]{.paramLabel}
            :   `paths` - inputs to a given target.

            [Returns:]{.returnLabel}
            :   index of path to set of inputs in that path

        []{#addSourceFolders(com.facebook.buck.features.project.intellij.model.folders.IJFolderFactory,com.google.common.collect.ImmutableMultimap,boolean,com.facebook.buck.features.project.intellij.ModuleBuildContext)}

        -   #### addSourceFolders

            ``` methodSignature
            protected void addSourceFolders​(IJFolderFactory factory,
                                            com.google.common.collect.ImmutableMultimap<Path,​Path> foldersToInputsIndex,
                                            boolean wantsPackagePrefix,
                                            ModuleBuildContext context)
            ```

            ::: block
            Add the set of input paths to the
            [`IjModule.Builder`](model/IjModule.Builder.html "class in com.facebook.buck.features.project.intellij.model")
            as source folders.
            :::

            [Parameters:]{.paramLabel}
            :   `foldersToInputsIndex` - mapping of source folders to
                their inputs.
            :   `wantsPackagePrefix` - whether folders should be
                annotated with a package prefix. This only makes sense
                when the source folder is Java source code.
            :   `context` - the module to add the folders to.

        []{#addResourceFolders(com.facebook.buck.features.project.intellij.model.folders.ResourceFolderFactory,com.google.common.collect.ImmutableMultimap,java.nio.file.Path,com.facebook.buck.features.project.intellij.ModuleBuildContext)}

        -   #### addResourceFolders

            ``` methodSignature
            protected void addResourceFolders​(ResourceFolderFactory factory,
                                              com.google.common.collect.ImmutableMultimap<Path,​Path> foldersToInputsIndex,
                                              Path resourcesRoot,
                                              ModuleBuildContext context)
            ```

        []{#addDepsAndSources(com.facebook.buck.core.model.targetgraph.TargetNode,boolean,com.facebook.buck.features.project.intellij.ModuleBuildContext,com.google.common.collect.ImmutableSet)}

        -   #### addDepsAndSources

            ``` methodSignature
            protected void addDepsAndSources​(TargetNode<T> targetNode,
                                             boolean wantsPackagePrefix,
                                             ModuleBuildContext context,
                                             com.google.common.collect.ImmutableSet<Path> resourcePaths)
            ```

        []{#addDepsAndSources(com.facebook.buck.core.model.targetgraph.TargetNode,boolean,com.facebook.buck.features.project.intellij.ModuleBuildContext)}

        -   #### addDepsAndSources

            ``` methodSignature
            protected void addDepsAndSources​(TargetNode<T> targetNode,
                                             boolean wantsPackagePrefix,
                                             ModuleBuildContext context)
            ```

        []{#addDepsAndTestSources(com.facebook.buck.core.model.targetgraph.TargetNode,boolean,com.facebook.buck.features.project.intellij.ModuleBuildContext,com.google.common.collect.ImmutableSet)}

        -   #### addDepsAndTestSources

            ``` methodSignature
            protected void addDepsAndTestSources​(TargetNode<T> targetNode,
                                                 boolean wantsPackagePrefix,
                                                 ModuleBuildContext context,
                                                 com.google.common.collect.ImmutableSet<Path> resourcePaths)
            ```

        []{#addDepsAndTestSources(com.facebook.buck.core.model.targetgraph.TargetNode,boolean,com.facebook.buck.features.project.intellij.ModuleBuildContext)}

        -   #### addDepsAndTestSources

            ``` methodSignature
            protected void addDepsAndTestSources​(TargetNode<T> targetNode,
                                                 boolean wantsPackagePrefix,
                                                 ModuleBuildContext context)
            ```

        []{#getResourcePaths(java.util.Collection)}

        -   #### getResourcePaths

            ``` methodSignature
            protected com.google.common.collect.ImmutableSet<Path> getResourcePaths​(Collection<SourcePath> resources)
            ```

        []{#getResourcePaths(java.util.Collection,java.nio.file.Path)}

        -   #### getResourcePaths

            ``` methodSignature
            protected com.google.common.collect.ImmutableSet<Path> getResourcePaths​(Collection<SourcePath> resources,
                                                                                    Path resourcesRoot)
            ```

        []{#getResourcesRootsToResources(com.facebook.buck.jvm.core.JavaPackageFinder,com.google.common.collect.ImmutableSet)}

        -   #### getResourcesRootsToResources

            ``` methodSignature
            protected com.google.common.collect.ImmutableMultimap<Path,​Path> getResourcesRootsToResources​(JavaPackageFinder packageFinder,
                                                                                                                com.google.common.collect.ImmutableSet<Path> resourcePaths)
            ```

        []{#addResourceFolders(com.facebook.buck.features.project.intellij.model.folders.IjResourceFolderType,com.google.common.collect.ImmutableCollection,java.nio.file.Path,com.facebook.buck.features.project.intellij.ModuleBuildContext)}

        -   #### addResourceFolders

            ``` methodSignature
            protected void addResourceFolders​(IjResourceFolderType ijResourceFolderType,
                                              com.google.common.collect.ImmutableCollection<Path> resourcePaths,
                                              Path resourcesRoot,
                                              ModuleBuildContext context)
            ```

        []{#applyDuringAggregation(com.facebook.buck.features.project.intellij.aggregation.AggregationContext,com.facebook.buck.core.model.targetgraph.TargetNode)}

        -   #### applyDuringAggregation

            ``` methodSignature
            public void applyDuringAggregation​(AggregationContext context,
                                               TargetNode<T> targetNode)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `applyDuringAggregation` in
                interface `IjModuleRule<T extends BuildRuleArg>`
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

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

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../deprecated-list.html)
-   [Index](../../../../../index-all.html)
-   [Help](../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.android.apkmodule](package-summary.html)
:::

## Class APKModuleGraph {#class-apkmodulegraph .title title="Class APKModuleGraph"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.apkmodule.APKModuleGraph

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`

    ------------------------------------------------------------------------

        public class APKModuleGraph
        extends Object
        implements AddsToRuleKey

    ::: block
    Utility class for grouping sets of targets and their dependencies
    into APK Modules containing their exclusive dependencies. Targets
    that are dependencies of the root target are included in the root.
    Targets that have dependencies in two are more groups are put the
    APKModule that represents the dependent modules minimal cover based
    on the declared dependencies given. If the minimal cover contains
    more than one APKModule, the target will belong to a new shared
    APKModule that is a dependency of all APKModules in the minimal
    cover.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                   Description
          ------------------- ----------------------- -------------
          `static String`     `ROOT_APKMODULE_NAME`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `APKModul                         | ::: block                         |
        | eGraph​(TargetGraph targetGraph,   | Constructor for the `APKModule`   |
        |              BuildTarget target)` | graph generator object that       |
        |                                   | produces a graph with only a root |
        |                                   | module.                           |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `APKModuleGraph​(TargetGraph ta    | ::: block                         |
        | rgetGraph,               BuildTar | Constructor for the `APKModule`   |
        | get target,               Optiona | graph generator object            |
        | l<Set<BuildTarget>> seedTargets)` | :::                               |
        +-----------------------------------+-----------------------------------+
        | `APKModuleGraph​(Op                | ::: block                         |
        | tional<com.google.common.collect. | Constructor for the `APKModule`   |
        | ImmutableMap<String,​com.google.co | graph generator object            |
        | mmon.collect.ImmutableList<BuildT | :::                               |
        | arget>>> seedConfigMap,           |                                   |
        |      Optional<com.google.common.c |                                   |
        | ollect.ImmutableMap<String,​com.go |                                   |
        | ogle.common.collect.ImmutableList |                                   |
        | <String>>> appModuleDependencies, |                                   |
        |                Optional<List<Buil |                                   |
        | dTarget>> blacklistedModules,     |                                   |
        |            Set<String> modulesWit |                                   |
        | hResources,               Set<Str |                                   |
        | ing> modulesWithManifest,         |                                   |
        |        TargetGraph targetGraph,   |                                   |
        |              BuildTarget target)` |                                   |
        +-----------------------------------+-----------------------------------+

        : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static Optiona       | `extractTargetsF      | ::: block             |
        | l<List<BuildTarget>>` | romQueries​(Optional<L | Utility method for    |
        |                       | ist<Query>> queries)` | flattening a list of  |
        |                       |                       | queries into the a    |
        |                       |                       | list of the build     |
        |                       |                       | targets they resolve  |
        |                       |                       | to.                   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `APKModule`           | `findMa               | ::: block             |
        |                       | nifestModuleForTarget | Get the Module that   |
        |                       | ​(BuildTarget target)` | should contain the    |
        |                       |                       | manifest for the      |
        |                       |                       | given target or else  |
        |                       |                       | fallback to the same  |
        |                       |                       | logic of              |
        |                       |                       | findRes               |
        |                       |                       | ourceModuleForTarget. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `APKModule`           | `findModuleForTarget  | ::: block             |
        |                       | ​(BuildTarget target)` | Get the Module that   |
        |                       |                       | contains the given    |
        |                       |                       | target                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `APKModule`           | `findRe               | ::: block             |
        |                       | sourceModuleForTarget | Get the Module that   |
        |                       | ​(BuildTarget target)` | should contain the    |
        |                       |                       | resources for the     |
        |                       |                       | given target          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.goog             | `getAPKModules()`     |                       |
        | le.common.collect.Imm |                       |                       |
        | utableSet<APKModule>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `getAPKModuleToClas   | ::: block             |
        |  com.google.common.co | sesMap​(com.google.com | Group the classes in  |
        | llect.ImmutableMultim | mon.collect.Immutable | the input jars into a |
        | ap<APKModule,​String>` | Multimap<APKModule,​Pa | multimap based on the |
        |                       | th> apkModuleToJarPat | APKModule they belong |
        |                       | hMap,                 | to                    |
        |                       |          java.util.fu | :::                   |
        |                       | nction.Function<Strin |                       |
        |                       | g,​String> translatorF |                       |
        |                       | unction,              |                       |
        |                       |             ProjectFi |                       |
        |                       | lesystem filesystem)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Set<BuildTarget>`    | `getBuildTarge        |                       |
        |                       | ts​(APKModule module)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `DirectedAcy          | `getGraph()`          | ::: block             |
        | clicGraph<APKModule>` |                       | Lazy generate the     |
        |                       |                       | graph on first use    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `APKModule`           | `getRootAPKModule()`  | ::: block             |
        |                       |                       | Get the APKModule     |
        |                       |                       | representing the core |
        |                       |                       | application that is   |
        |                       |                       | always included in    |
        |                       |                       | the apk               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optio                | `getSeedConfigMap()`  |                       |
        | nal<com.google.common |                       |                       |
        | .collect.ImmutableMap |                       |                       |
        | <String,​com.google.co |                       |                       |
        | mmon.collect.Immutabl |                       |                       |
        | eList<BuildTarget>>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.goo              | `                     |                       |
        | gle.common.collect.Im | toOutgoingEdgesMap()` |                       |
        | mutableSortedMap<APKM |                       |                       |
        | odule,​com.google.comm |                       |                       |
        | on.collect.ImmutableS |                       |                       |
        | ortedSet<APKModule>>` |                       |                       |
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
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#ROOT_APKMODULE_NAME}

        -   #### ROOT_APKMODULE_NAME

                public static final String ROOT_APKMODULE_NAME

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.android.apkmodule.APKModuleGraph.ROOT_APKMODULE_NAME)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.targetgraph.TargetGraph,com.facebook.buck.core.model.BuildTarget)}

        -   #### APKModuleGraph

                public APKModuleGraph​(TargetGraph targetGraph,
                                      BuildTarget target)

            ::: block
            Constructor for the `APKModule` graph generator object that
            produces a graph with only a root module.
            :::

        []{#<init>(java.util.Optional,java.util.Optional,java.util.Optional,java.util.Set,java.util.Set,com.facebook.buck.core.model.targetgraph.TargetGraph,com.facebook.buck.core.model.BuildTarget)}

        -   #### APKModuleGraph

                public APKModuleGraph​(Optional<com.google.common.collect.ImmutableMap<String,​com.google.common.collect.ImmutableList<BuildTarget>>> seedConfigMap,
                                      Optional<com.google.common.collect.ImmutableMap<String,​com.google.common.collect.ImmutableList<String>>> appModuleDependencies,
                                      Optional<List<BuildTarget>> blacklistedModules,
                                      Set<String> modulesWithResources,
                                      Set<String> modulesWithManifest,
                                      TargetGraph targetGraph,
                                      BuildTarget target)

            ::: block
            Constructor for the `APKModule` graph generator object
            :::

            [Parameters:]{.paramLabel}
            :   `seedConfigMap` - A map of names to seed targets to use
                for creating `APKModule`.
            :   `appModuleDependencies` -

                a mapping of declared dependencies between module names.
                If a APKModule **m1** depends on **m2**, it implies to
                buck that in order for **m1** to be available for
                execution **m2** must be available for use as well.
                Because of this, we can say that including a buck target
                in **m2** effectively includes the buck-target in
                **m2\'s** dependent **m1**. In other words, **m2**
                covers **m1**. Therefore, if a buck target is required
                by both these modules, we can safely place it in the
                minimal cover which is the APKModule **m2**.
            :   `blacklistedModules` - A list of targets that will NOT
                be included in any module.
            :   `modulesWithResources` - A list of modules with
                resources
            :   `modulesWithManifest` - A list of modules with
                manifests. This parameter will be later used to fetch
                Manifest information for each module.
            :   `targetGraph` - The full target graph of the build
            :   `target` - The root target to use to traverse the graph

        []{#<init>(com.facebook.buck.core.model.targetgraph.TargetGraph,com.facebook.buck.core.model.BuildTarget,java.util.Optional)}

        -   #### APKModuleGraph

                public APKModuleGraph​(TargetGraph targetGraph,
                                      BuildTarget target,
                                      Optional<Set<BuildTarget>> seedTargets)

            ::: block
            Constructor for the `APKModule` graph generator object
            :::

            [Parameters:]{.paramLabel}
            :   `targetGraph` - The full target graph of the build
            :   `target` - The root target to use to traverse the graph
            :   `seedTargets` - The set of seed targets to use for
                creating `APKModule`.
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#toOutgoingEdgesMap()}

        -   #### toOutgoingEdgesMap

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedMap<APKModule,​com.google.common.collect.ImmutableSortedSet<APKModule>> toOutgoingEdgesMap()
            ```

        []{#extractTargetsFromQueries(java.util.Optional)}

        -   #### extractTargetsFromQueries

            ``` methodSignature
            public static Optional<List<BuildTarget>> extractTargetsFromQueries​(Optional<List<Query>> queries)
            ```

            ::: block
            Utility method for flattening a list of queries into the a
            list of the build targets they resolve to.
            :::

            [Parameters:]{.paramLabel}
            :   `queries` - list of queries, they are expected to have
                already been resolved

            [Returns:]{.returnLabel}
            :   list of build targets queries resolve to joined together

        []{#getGraph()}

        -   #### getGraph

            ``` methodSignature
            public DirectedAcyclicGraph<APKModule> getGraph()
            ```

            ::: block
            Lazy generate the graph on first use
            :::

            [Returns:]{.returnLabel}
            :   the DAG representing APKModules and their dependency
                relationships

        []{#getRootAPKModule()}

        -   #### getRootAPKModule

            ``` methodSignature
            public APKModule getRootAPKModule()
            ```

            ::: block
            Get the APKModule representing the core application that is
            always included in the apk
            :::

            [Returns:]{.returnLabel}
            :   the root APK Module

        []{#getAPKModules()}

        -   #### getAPKModules

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<APKModule> getAPKModules()
            ```

        []{#getSeedConfigMap()}

        -   #### getSeedConfigMap

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableMap<String,​com.google.common.collect.ImmutableList<BuildTarget>>> getSeedConfigMap()
            ```

        []{#findModuleForTarget(com.facebook.buck.core.model.BuildTarget)}

        -   #### findModuleForTarget

            ``` methodSignature
            public APKModule findModuleForTarget​(BuildTarget target)
            ```

            ::: block
            Get the Module that contains the given target
            :::

            [Parameters:]{.paramLabel}
            :   `target` - target to serach for in modules

            [Returns:]{.returnLabel}
            :   the module that contains the target

        []{#findResourceModuleForTarget(com.facebook.buck.core.model.BuildTarget)}

        -   #### findResourceModuleForTarget

            ``` methodSignature
            public APKModule findResourceModuleForTarget​(BuildTarget target)
            ```

            ::: block
            Get the Module that should contain the resources for the
            given target
            :::

            [Parameters:]{.paramLabel}
            :   `target` - target to serach for in modules

            [Returns:]{.returnLabel}
            :   the module that contains the target

        []{#findManifestModuleForTarget(com.facebook.buck.core.model.BuildTarget)}

        -   #### findManifestModuleForTarget

            ``` methodSignature
            public APKModule findManifestModuleForTarget​(BuildTarget target)
            ```

            ::: block
            Get the Module that should contain the manifest for the
            given target or else fallback to the same logic of
            findResourceModuleForTarget.
            :::

            [Parameters:]{.paramLabel}
            :   `target` - target to search for in modules

            [Returns:]{.returnLabel}
            :   the module that contains the target

        []{#getAPKModuleToClassesMap(com.google.common.collect.ImmutableMultimap,java.util.function.Function,com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### getAPKModuleToClassesMap

            ``` methodSignature
            public static com.google.common.collect.ImmutableMultimap<APKModule,​String> getAPKModuleToClassesMap​(com.google.common.collect.ImmutableMultimap<APKModule,​Path> apkModuleToJarPathMap,
                                                                                                                       java.util.function.Function<String,​String> translatorFunction,
                                                                                                                       ProjectFilesystem filesystem)
                                                                                                                throws IOException
            ```

            ::: block
            Group the classes in the input jars into a multimap based on
            the APKModule they belong to
            :::

            [Parameters:]{.paramLabel}
            :   `apkModuleToJarPathMap` - the mapping of APKModules to
                the path for the jar files
            :   `translatorFunction` - function used to translate the
                class names to obfuscated names
            :   `filesystem` - filesystem representation for resolving
                paths

            [Returns:]{.returnLabel}
            :   The mapping of APKModules to the class names they
                contain

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getBuildTargets(com.facebook.buck.android.apkmodule.APKModule)}

        -   #### getBuildTargets

            ``` methodSignature
            public Set<BuildTarget> getBuildTargets​(APKModule module)
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

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../deprecated-list.html)
-   [Index](../../../../../index-all.html)
-   [Help](../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../allclasses.html)

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

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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.apple](package-summary.html)
:::

## Class AppleBuildRules {#class-applebuildrules .title title="Class AppleBuildRules"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.AppleBuildRules

::: description
-   

    ------------------------------------------------------------------------

        public final class AppleBuildRules
        extends Object

    ::: block
    Helpers for reading properties of Apple target build rules.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                                         Description
          ------------------- --------------------------------------------- -------------
          `static class `     `AppleBuildRules.RecursiveDependenciesMode`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                                                                      Field                                   Description
          -------------------------------------------------------------------------------------- --------------------------------------- -------------
          `static com.google.common.collect.ImmutableSet<Class<? extends BaseDescription<?>>>`   `CORE_DATA_MODEL_DESCRIPTION_CLASSES`    
          `static com.google.common.collect.ImmutableSet<Class<? extends BaseDescription<?>>>`   `SCENEKIT_ASSETS_DESCRIPTION_CLASSES`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static com.googl     | `collectDirectAssetCa |                       |
        | e.common.collect.Immu | talogs​(TargetGraph ta |                       |
        | tableSet<AppleAssetCa | rgetGraph,            |                       |
        | talogDescriptionArg>` |                 Targe |                       |
        |                       | tNode<?> targetNode)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `collectRecurs        | ::: block             |
        | static <T extends Con | iveAssetCatalogs​(XCod | Collect recursive     |
        | structorArg>com.googl | eDescriptions xcodeDe | asset catalogs        |
        | e.common.collect.Immu | scriptions,           | :::                   |
        | tableSet<AppleAssetCa |                     T |                       |
        | talogDescriptionArg>` | argetGraph targetGrap |                       |
        |                       | h,                    |                       |
        |                       |            Optional<A |                       |
        |                       | ppleDependenciesCache |                       |
        |                       | > cache,              |                       |
        |                       |                  Iter |                       |
        |                       | able<TargetNode<T>> t |                       |
        |                       | argetNodes,           |                       |
        |                       |                     A |                       |
        |                       | ppleBuildRules.Recurs |                       |
        |                       | iveDependenciesMode m |                       |
        |                       | ode,                  |                       |
        |                       |              java.uti |                       |
        |                       | l.function.Predicate< |                       |
        |                       | BuildTarget> filter)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static <T ext        | `collectRecur         | ::: block             |
        | ends ConstructorArg>c | siveWrapperResources​( | Collect recursive     |
        | om.google.common.coll | XCodeDescriptions xco | wrapper resources     |
        | ect.ImmutableSet<Appl | deDescriptions,       | :::                   |
        | eWrapperResourceArg>` |                       |                       |
        |                       |       TargetGraph tar |                       |
        |                       | getGraph,             |                       |
        |                       |                       |                       |
        |                       | Optional<AppleDepende |                       |
        |                       | nciesCache> cache,    |                       |
        |                       |                       |                       |
        |                       |          Iterable<Tar |                       |
        |                       | getNode<T>> targetNod |                       |
        |                       | es,                   |                       |
        |                       |                AppleB |                       |
        |                       | uildRules.RecursiveDe |                       |
        |                       | pendenciesMode mode)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static <T exten      | `c                    | ::: block             |
        | ds ConstructorArg,​V e | ollectTransitiveBuild | Collects transitive   |
        | xtends TargetNode<T>> | RuleTargets​(XCodeDesc | target nodes of type  |
        | com.google.common.col | riptions xcodeDescrip | included in           |
        | lect.ImmutableSet<V>` | tions,                | descriptionClasses    |
        |                       |                    Ta | :::                   |
        |                       | rgetGraph targetGraph |                       |
        |                       | ,                     |                       |
        |                       |               Optiona |                       |
        |                       | l<AppleDependenciesCa |                       |
        |                       | che> cache,           |                       |
        |                       |                       |                       |
        |                       |    com.google.common. |                       |
        |                       | collect.ImmutableSet< |                       |
        |                       | Class<? extends BaseD |                       |
        |                       | escription<?>>> descr |                       |
        |                       | iptionClasses,        |                       |
        |                       |                       |                       |
        |                       |       Collection<Targ |                       |
        |                       | etNode<?>> targetNode |                       |
        |                       | s,                    |                       |
        |                       |                AppleB |                       |
        |                       | uildRules.RecursiveDe |                       |
        |                       | pendenciesMode mode)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static <T>           | `coll                 | ::: block             |
        | com.google.common.col | ectTransitiveBuildRul | Collect the           |
        | lect.ImmutableSet<T>` | eTargetsWithTransform | transitive target     |
        |                       | ​(XCodeDescriptions xc | node dependencies     |
        |                       | odeDescriptions,      | using some            |
        |                       |                       | Recur                 |
        |                       |                       | siveDependenciesMode. |
        |                       | TargetGraph targetGra | :::                   |
        |                       | ph,                   |                       |
        |                       |                       |                       |
        |                       |         Optional<Appl |                       |
        |                       | eDependenciesCache> c |                       |
        |                       | ache,                 |                       |
        |                       |                       |                       |
        |                       |           com.google. |                       |
        |                       | common.collect.Immuta |                       |
        |                       | bleSet<Class<? extend |                       |
        |                       | s BaseDescription<?>> |                       |
        |                       | > descriptionClasses, |                       |
        |                       |                       |                       |
        |                       |                       |                       |
        |                       |      Collection<Targe |                       |
        |                       | tNode<?>> targetNodes |                       |
        |                       | ,                     |                       |
        |                       |                       |                       |
        |                       |       AppleBuildRules |                       |
        |                       | .RecursiveDependencie |                       |
        |                       | sMode mode,           |                       |
        |                       |                       |                       |
        |                       |                 java. |                       |
        |                       | util.function.Functio |                       |
        |                       | n<TargetNode<?>,​T> tr |                       |
        |                       | ansform,              |                       |
        |                       |                       |                       |
        |                       |              java.uti |                       |
        |                       | l.function.Predicate< |                       |
        |                       | BuildTarget> filter)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static <T ex         | `collect              |                       |
        | tends ConstructorArg> | TransitiveBuildTarget |                       |
        | com.google.common.col | Arg​(XCodeDescriptions |                       |
        | lect.ImmutableSet<T>` |  xcodeDescriptions,   |                       |
        |                       |                       |                       |
        |                       |          TargetGraph  |                       |
        |                       | targetGraph,          |                       |
        |                       |                       |                       |
        |                       |   Optional<AppleDepen |                       |
        |                       | denciesCache> cache,  |                       |
        |                       |                       |                       |
        |                       |           com.google. |                       |
        |                       | common.collect.Immuta |                       |
        |                       | bleSet<Class<? extend |                       |
        |                       | s BaseDescription<?>> |                       |
        |                       | > descriptionClasses, |                       |
        |                       |                       |                       |
        |                       |            Collection |                       |
        |                       | <TargetNode<?>> targe |                       |
        |                       | tNodes,               |                       |
        |                       |                   App |                       |
        |                       | leBuildRules.Recursiv |                       |
        |                       | eDependenciesMode mod |                       |
        |                       | e,                    |                       |
        |                       |              java.uti |                       |
        |                       | l.function.Predicate< |                       |
        |                       | BuildTarget> filter)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `getOutputFileName    |                       |
        |                       | FormatForLibrary​(bool |                       |
        |                       | ean isSharedLibrary)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static com.google.c  | `getRecursi           |                       |
        | ommon.collect.Immutab | veTargetNodeDependenc |                       |
        | leSet<TargetNode<?>>` | iesOfTypes​(XCodeDescr |                       |
        |                       | iptions xcodeDescript |                       |
        |                       | ions,                 |                       |
        |                       |                       |                       |
        |                       |      TargetGraph targ |                       |
        |                       | etGraph,              |                       |
        |                       |                       |                       |
        |                       |         Optional<Appl |                       |
        |                       | eDependenciesCache> c |                       |
        |                       | ache,                 |                       |
        |                       |                       |                       |
        |                       |      AppleBuildRules. |                       |
        |                       | RecursiveDependencies |                       |
        |                       | Mode mode,            |                       |
        |                       |                       |                       |
        |                       |           TargetNode< |                       |
        |                       | ?> input,             |                       |
        |                       |                       |                       |
        |                       |          com.google.c |                       |
        |                       | ommon.collect.Immutab |                       |
        |                       | leSet<Class<? extends |                       |
        |                       |  BaseDescription<?>>> |                       |
        |                       |  descriptionClasses)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static com.google.c  | `getR                 |                       |
        | ommon.collect.Immutab | ecursiveTargetNodeDep |                       |
        | leSet<TargetNode<?>>` | endenciesOfTypes​(XCod |                       |
        |                       | eDescriptions xcodeDe |                       |
        |                       | scriptions,           |                       |
        |                       |                       |                       |
        |                       |            TargetGrap |                       |
        |                       | h targetGraph,        |                       |
        |                       |                       |                       |
        |                       |               Optiona |                       |
        |                       | l<AppleDependenciesCa |                       |
        |                       | che> cache,           |                       |
        |                       |                       |                       |
        |                       |            AppleBuild |                       |
        |                       | Rules.RecursiveDepend |                       |
        |                       | enciesMode mode,      |                       |
        |                       |                       |                       |
        |                       |                 Targe |                       |
        |                       | tNode<?> targetNode,  |                       |
        |                       |                       |                       |
        |                       |                     j |                       |
        |                       | ava.util.function.Pre |                       |
        |                       | dicate<TargetNode<?>> |                       |
        |                       |  isDependencyNode,    |                       |
        |                       |                       |                       |
        |                       |                   Opt |                       |
        |                       | ional<AppleCxxPlatfor |                       |
        |                       | m> appleCxxPlatform)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static com.google.c  | `getR                 |                       |
        | ommon.collect.Immutab | ecursiveTargetNodeDep |                       |
        | leSet<TargetNode<?>>` | endenciesOfTypes​(XCod |                       |
        |                       | eDescriptions xcodeDe |                       |
        |                       | scriptions,           |                       |
        |                       |                       |                       |
        |                       |            TargetGrap |                       |
        |                       | h targetGraph,        |                       |
        |                       |                       |                       |
        |                       |               Optiona |                       |
        |                       | l<AppleDependenciesCa |                       |
        |                       | che> cache,           |                       |
        |                       |                       |                       |
        |                       |            AppleBuild |                       |
        |                       | Rules.RecursiveDepend |                       |
        |                       | enciesMode mode,      |                       |
        |                       |                       |                       |
        |                       |                 Targe |                       |
        |                       | tNode<?> targetNode,  |                       |
        |                       |                       |                       |
        |                       |                     O |                       |
        |                       | ptional<com.google.co |                       |
        |                       | mmon.collect.Immutabl |                       |
        |                       | eSet<Class<? extends  |                       |
        |                       | BaseDescription<?>>>> |                       |
        |                       |  descriptionClasses)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static com.google.c  | `getSchemeBuild       |                       |
        | ommon.collect.Immutab | ableTargetNodes​(XCode |                       |
        | leSet<TargetNode<?>>` | Descriptions xcodeDes |                       |
        |                       | criptions,            |                       |
        |                       |                    Ta |                       |
        |                       | rgetGraph targetGraph |                       |
        |                       | ,                     |                       |
        |                       |           Optional<Ap |                       |
        |                       | pleDependenciesCache> |                       |
        |                       |  cache,               |                       |
        |                       |                 Targe |                       |
        |                       | tNode<?> targetNode)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `i                    | ::: block             |
        |                       | sXcodeTargetTestBuild | Whether the build     |
        |                       | Rule​(BuildRule rule)` | rule type is a test   |
        |                       |                       | target.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `is                   | ::: block             |
        |                       | XcodeTargetTestBundle | Whether the bundle    |
        |                       | Extension​(AppleBundle | extension is a test   |
        |                       | Extension extension)` | bundle extension.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
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

        []{#CORE_DATA_MODEL_DESCRIPTION_CLASSES}

        -   #### CORE_DATA_MODEL_DESCRIPTION_CLASSES

                public static final com.google.common.collect.ImmutableSet<Class<? extends BaseDescription<?>>> CORE_DATA_MODEL_DESCRIPTION_CLASSES

        []{#SCENEKIT_ASSETS_DESCRIPTION_CLASSES}

        -   #### SCENEKIT_ASSETS_DESCRIPTION_CLASSES

                public static final com.google.common.collect.ImmutableSet<Class<? extends BaseDescription<?>>> SCENEKIT_ASSETS_DESCRIPTION_CLASSES
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#isXcodeTargetTestBuildRule(com.facebook.buck.core.rules.BuildRule)}

        -   #### isXcodeTargetTestBuildRule

            ``` methodSignature
            public static boolean isXcodeTargetTestBuildRule​(BuildRule rule)
            ```

            ::: block
            Whether the build rule type is a test target.
            :::

        []{#isXcodeTargetTestBundleExtension(com.facebook.buck.apple.AppleBundleExtension)}

        -   #### isXcodeTargetTestBundleExtension

            ``` methodSignature
            public static boolean isXcodeTargetTestBundleExtension​(AppleBundleExtension extension)
            ```

            ::: block
            Whether the bundle extension is a test bundle extension.
            :::

        []{#getOutputFileNameFormatForLibrary(boolean)}

        -   #### getOutputFileNameFormatForLibrary

            ``` methodSignature
            public static String getOutputFileNameFormatForLibrary​(boolean isSharedLibrary)
            ```

        []{#getRecursiveTargetNodeDependenciesOfTypes(com.facebook.buck.apple.XCodeDescriptions,com.facebook.buck.core.model.targetgraph.TargetGraph,java.util.Optional,com.facebook.buck.apple.AppleBuildRules.RecursiveDependenciesMode,com.facebook.buck.core.model.targetgraph.TargetNode,java.util.Optional)}

        -   #### getRecursiveTargetNodeDependenciesOfTypes

            ``` methodSignature
            public static com.google.common.collect.ImmutableSet<TargetNode<?>> getRecursiveTargetNodeDependenciesOfTypes​(XCodeDescriptions xcodeDescriptions,
                                                                                                                          TargetGraph targetGraph,
                                                                                                                          Optional<AppleDependenciesCache> cache,
                                                                                                                          AppleBuildRules.RecursiveDependenciesMode mode,
                                                                                                                          TargetNode<?> targetNode,
                                                                                                                          Optional<com.google.common.collect.ImmutableSet<Class<? extends BaseDescription<?>>>> descriptionClasses)
            ```

        []{#getRecursiveTargetNodeDependenciesOfTypes(com.facebook.buck.apple.XCodeDescriptions,com.facebook.buck.core.model.targetgraph.TargetGraph,java.util.Optional,com.facebook.buck.apple.AppleBuildRules.RecursiveDependenciesMode,com.facebook.buck.core.model.targetgraph.TargetNode,java.util.function.Predicate,java.util.Optional)}

        -   #### getRecursiveTargetNodeDependenciesOfTypes

            ``` methodSignature
            public static com.google.common.collect.ImmutableSet<TargetNode<?>> getRecursiveTargetNodeDependenciesOfTypes​(XCodeDescriptions xcodeDescriptions,
                                                                                                                          TargetGraph targetGraph,
                                                                                                                          Optional<AppleDependenciesCache> cache,
                                                                                                                          AppleBuildRules.RecursiveDependenciesMode mode,
                                                                                                                          TargetNode<?> targetNode,
                                                                                                                          java.util.function.Predicate<TargetNode<?>> isDependencyNode,
                                                                                                                          Optional<AppleCxxPlatform> appleCxxPlatform)
            ```

        []{#getRecursiveTargetNodeDependenciesOfTypes(com.facebook.buck.apple.XCodeDescriptions,com.facebook.buck.core.model.targetgraph.TargetGraph,java.util.Optional,com.facebook.buck.apple.AppleBuildRules.RecursiveDependenciesMode,com.facebook.buck.core.model.targetgraph.TargetNode,com.google.common.collect.ImmutableSet)}

        -   #### getRecursiveTargetNodeDependenciesOfTypes

            ``` methodSignature
            public static com.google.common.collect.ImmutableSet<TargetNode<?>> getRecursiveTargetNodeDependenciesOfTypes​(XCodeDescriptions xcodeDescriptions,
                                                                                                                          TargetGraph targetGraph,
                                                                                                                          Optional<AppleDependenciesCache> cache,
                                                                                                                          AppleBuildRules.RecursiveDependenciesMode mode,
                                                                                                                          TargetNode<?> input,
                                                                                                                          com.google.common.collect.ImmutableSet<Class<? extends BaseDescription<?>>> descriptionClasses)
            ```

        []{#getSchemeBuildableTargetNodes(com.facebook.buck.apple.XCodeDescriptions,com.facebook.buck.core.model.targetgraph.TargetGraph,java.util.Optional,com.facebook.buck.core.model.targetgraph.TargetNode)}

        -   #### getSchemeBuildableTargetNodes

            ``` methodSignature
            public static com.google.common.collect.ImmutableSet<TargetNode<?>> getSchemeBuildableTargetNodes​(XCodeDescriptions xcodeDescriptions,
                                                                                                              TargetGraph targetGraph,
                                                                                                              Optional<AppleDependenciesCache> cache,
                                                                                                              TargetNode<?> targetNode)
            ```

        []{#collectRecursiveAssetCatalogs(com.facebook.buck.apple.XCodeDescriptions,com.facebook.buck.core.model.targetgraph.TargetGraph,java.util.Optional,java.lang.Iterable,com.facebook.buck.apple.AppleBuildRules.RecursiveDependenciesMode,java.util.function.Predicate)}

        -   #### collectRecursiveAssetCatalogs

            ``` methodSignature
            public static <T extends ConstructorArg> com.google.common.collect.ImmutableSet<AppleAssetCatalogDescriptionArg> collectRecursiveAssetCatalogs​(XCodeDescriptions xcodeDescriptions,
                                                                                                                                                           TargetGraph targetGraph,
                                                                                                                                                           Optional<AppleDependenciesCache> cache,
                                                                                                                                                           Iterable<TargetNode<T>> targetNodes,
                                                                                                                                                           AppleBuildRules.RecursiveDependenciesMode mode,
                                                                                                                                                           java.util.function.Predicate<BuildTarget> filter)
            ```

            ::: block
            Collect recursive asset catalogs
            :::

        []{#collectRecursiveWrapperResources(com.facebook.buck.apple.XCodeDescriptions,com.facebook.buck.core.model.targetgraph.TargetGraph,java.util.Optional,java.lang.Iterable,com.facebook.buck.apple.AppleBuildRules.RecursiveDependenciesMode)}

        -   #### collectRecursiveWrapperResources

            ``` methodSignature
            public static <T extends ConstructorArg> com.google.common.collect.ImmutableSet<AppleWrapperResourceArg> collectRecursiveWrapperResources​(XCodeDescriptions xcodeDescriptions,
                                                                                                                                                      TargetGraph targetGraph,
                                                                                                                                                      Optional<AppleDependenciesCache> cache,
                                                                                                                                                      Iterable<TargetNode<T>> targetNodes,
                                                                                                                                                      AppleBuildRules.RecursiveDependenciesMode mode)
            ```

            ::: block
            Collect recursive wrapper resources
            :::

        []{#collectTransitiveBuildTargetArg(com.facebook.buck.apple.XCodeDescriptions,com.facebook.buck.core.model.targetgraph.TargetGraph,java.util.Optional,com.google.common.collect.ImmutableSet,java.util.Collection,com.facebook.buck.apple.AppleBuildRules.RecursiveDependenciesMode,java.util.function.Predicate)}

        -   #### collectTransitiveBuildTargetArg

            ``` methodSignature
            public static <T extends ConstructorArg> com.google.common.collect.ImmutableSet<T> collectTransitiveBuildTargetArg​(XCodeDescriptions xcodeDescriptions,
                                                                                                                               TargetGraph targetGraph,
                                                                                                                               Optional<AppleDependenciesCache> cache,
                                                                                                                               com.google.common.collect.ImmutableSet<Class<? extends BaseDescription<?>>> descriptionClasses,
                                                                                                                               Collection<TargetNode<?>> targetNodes,
                                                                                                                               AppleBuildRules.RecursiveDependenciesMode mode,
                                                                                                                               java.util.function.Predicate<BuildTarget> filter)
            ```

        []{#collectTransitiveBuildRuleTargets(com.facebook.buck.apple.XCodeDescriptions,com.facebook.buck.core.model.targetgraph.TargetGraph,java.util.Optional,com.google.common.collect.ImmutableSet,java.util.Collection,com.facebook.buck.apple.AppleBuildRules.RecursiveDependenciesMode)}

        -   #### collectTransitiveBuildRuleTargets

            ``` methodSignature
            public static <T extends ConstructorArg,​V extends TargetNode<T>> com.google.common.collect.ImmutableSet<V> collectTransitiveBuildRuleTargets​(XCodeDescriptions xcodeDescriptions,
                                                                                                                                                               TargetGraph targetGraph,
                                                                                                                                                               Optional<AppleDependenciesCache> cache,
                                                                                                                                                               com.google.common.collect.ImmutableSet<Class<? extends BaseDescription<?>>> descriptionClasses,
                                                                                                                                                               Collection<TargetNode<?>> targetNodes,
                                                                                                                                                               AppleBuildRules.RecursiveDependenciesMode mode)
            ```

            ::: block
            Collects transitive target nodes of type included in
            descriptionClasses
            :::

        []{#collectTransitiveBuildRuleTargetsWithTransform(com.facebook.buck.apple.XCodeDescriptions,com.facebook.buck.core.model.targetgraph.TargetGraph,java.util.Optional,com.google.common.collect.ImmutableSet,java.util.Collection,com.facebook.buck.apple.AppleBuildRules.RecursiveDependenciesMode,java.util.function.Function,java.util.function.Predicate)}

        -   #### collectTransitiveBuildRuleTargetsWithTransform

            ``` methodSignature
            public static <T> com.google.common.collect.ImmutableSet<T> collectTransitiveBuildRuleTargetsWithTransform​(XCodeDescriptions xcodeDescriptions,
                                                                                                                       TargetGraph targetGraph,
                                                                                                                       Optional<AppleDependenciesCache> cache,
                                                                                                                       com.google.common.collect.ImmutableSet<Class<? extends BaseDescription<?>>> descriptionClasses,
                                                                                                                       Collection<TargetNode<?>> targetNodes,
                                                                                                                       AppleBuildRules.RecursiveDependenciesMode mode,
                                                                                                                       java.util.function.Function<TargetNode<?>,​T> transform,
                                                                                                                       java.util.function.Predicate<BuildTarget> filter)
            ```

            ::: block
            Collect the transitive target node dependencies using some
            RecursiveDependenciesMode. Apply a transform on the
            dependencies
            :::

        []{#collectDirectAssetCatalogs(com.facebook.buck.core.model.targetgraph.TargetGraph,com.facebook.buck.core.model.targetgraph.TargetNode)}

        -   #### collectDirectAssetCatalogs

            ``` methodSignature
            public static com.google.common.collect.ImmutableSet<AppleAssetCatalogDescriptionArg> collectDirectAssetCatalogs​(TargetGraph targetGraph,
                                                                                                                             TargetNode<?> targetNode)
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
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

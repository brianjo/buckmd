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
-   Package
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

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
# Package com.facebook.buck.features.js {#package-com.facebook.buck.features.js .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [HasBundleName                    | ::: block                         |
    | ](HasBundleName.html "interface i | Common interface for rule args    |
    | n com.facebook.buck.features.js") | that have a bundle name that can  |
    |                                   | optionally be overridden          |
    |                                   | depending on the flavors a rule   |
    |                                   | is built with.                    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [HasExtraJso                      | ::: block                         |
    | n](HasExtraJson.html "interface i | Common interface for rule args    |
    | n com.facebook.buck.features.js") | that have used-defined JSON that  |
    |                                   | is passed on to the worker.       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JsBundleOutputs](                | ::: block                         |
    | JsBundleOutputs.html "interface i | Represents output paths of JS     |
    | n com.facebook.buck.features.js") | builds, consisting of JavaScript  |
    |                                   | build output, a corresponding     |
    |                                   | source map, \"misc\" directory    |
    |                                   | that can contain diverse assets   |
    |                                   | not meant to be part of the app   |
    |                                   | being shipped and                 |
    |                                   | assets/resources used from within |
    |                                   | the packaged JS source code.      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JsBundleO                        | ::: block                         |
    | utputsDescription](JsBundleOutput | Empty interface to mark           |
    | sDescription.html "interface in c | [`DescriptionWithTargetGr         |
    | om.facebook.buck.features.js")\<T | aph`](../../core/rules/Descriptio |
    | extends                           | nWithTargetGraph.html "interface  |
    | [BuildRuleArg](..                 | in com.facebook.buck.core.rules") |
    | /../core/description/arg/BuildRul | subclasses that return            |
    | eArg.html "interface in com.faceb | [`JsBundleOutputs`](              |
    | ook.buck.core.description.arg")\> | JsBundleOutputs.html "interface i |
    |                                   | n com.facebook.buck.features.js") |
    |                                   | instances from their              |
    |                                   | [`                                |
    |                                   | DescriptionWithTargetGraph.create |
    |                                   | BuildRule(com.facebook.buck.core. |
    |                                   | rules.BuildRuleCreationContextWit |
    |                                   | hTargetGraph, com.facebook.buck.c |
    |                                   | ore.model.BuildTarget, com.facebo |
    |                                   | ok.buck.core.rules.BuildRuleParam |
    |                                   | s, T)`](../../core/rules/Descript |
    |                                   | ionWithTargetGraph.html#createBui |
    |                                   | ldRule(com.facebook.buck.core.rul |
    |                                   | es.BuildRuleCreationContextWithTa |
    |                                   | rgetGraph,com.facebook.buck.core. |
    |                                   | model.BuildTarget,com.facebook.bu |
    |                                   | ck.core.rules.BuildRuleParams,T)) |
    |                                   | method.                           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JsDependenciesOutputs](JsDepe    | ::: block                         |
    | ndenciesOutputs.html "interface i | Represents output paths of JS     |
    | n com.facebook.buck.features.js") | #dependecy-flavored builds.       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [JsBundle](JsBundle.html "class i |                                   |
    | n com.facebook.buck.features.js") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JsBundleAndro                    | ::: block                         |
    | id](JsBundleAndroid.html "class i | Represents a combination of a     |
    | n com.facebook.buck.features.js") | JavaScript bundle \*and\* Android |
    |                                   | resources.                        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JsBundleDescription](            |                                   |
    | JsBundleDescription.html "class i |                                   |
    | n com.facebook.buck.features.js") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JsBundleDescriptionArg](JsB      | ::: block                         |
    | undleDescriptionArg.html "class i | Immutable implementation of       |
    | n com.facebook.buck.features.js") | `JsBundleDescription              |
    |                                   | .AbstractJsBundleDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JsBundleDe                       | ::: block                         |
    | scriptionArg.Builder](JsBundleDes | Builds instances of type          |
    | criptionArg.Builder.html "class i | [`JsBundleDescriptionArg`](JsBu   |
    | n com.facebook.buck.features.js") | ndleDescriptionArg.html "class in |
    |                                   |  com.facebook.buck.features.js"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JsBundleGenru                    | ::: block                         |
    | le](JsBundleGenrule.html "class i | Genrule specialized for the       |
    | n com.facebook.buck.features.js") | creation of JS bundles.           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Js                               |                                   |
    | BundleGenruleDescription](JsBundl |                                   |
    | eGenruleDescription.html "class i |                                   |
    | n com.facebook.buck.features.js") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JsBundle                         | ::: block                         |
    | GenruleDescriptionArg](JsBundleGe | Immutable implementation of       |
    | nruleDescriptionArg.html "class i | `                                 |
    | n com.facebook.buck.features.js") | JsBundleGenruleDescription.Abstra |
    |                                   | ctJsBundleGenruleDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JsBundleGenruleDescripti         | ::: block                         |
    | onArg.Builder](JsBundleGenruleDes | Builds instances of type          |
    | criptionArg.Builder.html "class i | [`JsBundleGe                      |
    | n com.facebook.buck.features.js") | nruleDescriptionArg`](JsBundleGen |
    |                                   | ruleDescriptionArg.html "class in |
    |                                   |  com.facebook.buck.features.js"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JsDependenciesFile]              |                                   |
    | (JsDependenciesFile.html "class i |                                   |
    | n com.facebook.buck.features.js") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JsDescriptionsProvider](JsD      |                                   |
    | escriptionsProvider.html "class i |                                   |
    | n com.facebook.buck.features.js") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JsFile](JsFile.html "class in c  | ::: block                         |
    | om.facebook.buck.features.js")\<T | JS file rule converted to MBR     |
    | extends                           | :::                               |
    | com.facebook.buck.                |                                   |
    | features.js.JsFile.AbstractImpl\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [J                                |                                   |
    | sFlavors](JsFlavors.html "class i |                                   |
    | n com.facebook.buck.features.js") |                                   |
    +-----------------------------------+-----------------------------------+
    | [J                                | ::: block                         |
    | sLibrary](JsLibrary.html "class i | JsLibrary rule                    |
    | n com.facebook.buck.features.js") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JsLibraryDescription](J          |                                   |
    | sLibraryDescription.html "class i |                                   |
    | n com.facebook.buck.features.js") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JsLibraryDescriptionArg](JsLi    | ::: block                         |
    | braryDescriptionArg.html "class i | Immutable implementation of       |
    | n com.facebook.buck.features.js") | `JsLibraryDescription.            |
    |                                   | AbstractJsLibraryDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JsLibraryDes                     | ::: block                         |
    | criptionArg.Builder](JsLibraryDes | Builds instances of type          |
    | criptionArg.Builder.html "class i | [`JsLibraryDescriptionArg`](JsLib |
    | n com.facebook.buck.features.js") | raryDescriptionArg.html "class in |
    |                                   |  com.facebook.buck.features.js"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JsModule](JsModule.html "class i |                                   |
    | n com.facebook.buck.features.js") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JsModuleAdapterPlugin](Js        |                                   |
    | ModuleAdapterPlugin.html "class i |                                   |
    | n com.facebook.buck.features.js") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JsUtil](JsUtil.html "class i     |                                   |
    | n com.facebook.buck.features.js") |                                   |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}
:::
:::

::: bottomNav
[]{#navbar.bottom}

::: skipNav
[Skip navigation links](#skip.navbar.bottom "Skip navigation links")
:::

[]{#navbar.bottom.firstrow}

-   [Overview](../../../../../index.html)
-   Package
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

[]{#skip.navbar.bottom}
:::

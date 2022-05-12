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

-   [Overview](index.html)
-   Package
-   Class
-   [Tree](overview-tree.html)
-   Deprecated
-   [Index](index-all.html)
-   [Help](help-doc.html)
:::

::: subNav
-   [All Classes](allclasses.html)

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
# Deprecated API {#deprecated-api .title title="Deprecated API"}

## Contents {#contents title="Contents"}

-   [Interfaces](#interface)
-   [Classes](#class)
-   [Fields](#field)
-   [Methods](#method)
:::

::: contentContainer
[]{#interface}

-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [com.facebook.buck.core.rules.    |                                   |
    | attr.HasCustomDepsLogic](com/face |                                   |
    | book/buck/core/rules/attr/HasCust |                                   |
    | omDepsLogic.html "interface in co |                                   |
    | m.facebook.buck.core.rules.attr") |                                   |
    +-----------------------------------+-----------------------------------+
    | [com.face                         | ::: deprecationComment            |
    | book.buck.core.rules.pipeline.Sup | Rule pipelining couples rules in  |
    | portsPipelining](com/facebook/buc | a way that makes it very easy to  |
    | k/core/rules/pipeline/SupportsPip | violate buck\'s assumptions and   |
    | elining.html "interface in com.fa | makes it nearly impossible for    |
    | cebook.buck.core.rules.pipeline") | buck to understand and restrict   |
    |                                   | what rules are doing.             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [com.facebook                     |                                   |
    | .buck.rules.keys.RuleKeyAppendabl |                                   |
    | e](com/facebook/buck/rules/keys/R |                                   |
    | uleKeyAppendable.html "interface  |                                   |
    | in com.facebook.buck.rules.keys") |                                   |
    +-----------------------------------+-----------------------------------+
    | [com.facebook.buck.rules          |                                   |
    | .keys.RuleKeyAppendable.RuleKeyAp |                                   |
    | pendableSink](com/facebook/buck/r |                                   |
    | ules/keys/RuleKeyAppendable.RuleK |                                   |
    | eyAppendableSink.html "interface  |                                   |
    | in com.facebook.buck.rules.keys") |                                   |
    +-----------------------------------+-----------------------------------+

    : Interfaces[ ]{.tabEnd}

[]{#class}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [com.fac                          |                                   |
    | ebook.buck.android.NdkLibraryDesc |                                   |
    | ription](com/facebook/buck/androi |                                   |
    | d/NdkLibraryDescription.html "cla |                                   |
    | ss in com.facebook.buck.android") |                                   |
    +-----------------------------------+-----------------------------------+
    | [com.facebook.buck.cor            | ::: deprecationComment            |
    | e.model.impl.BuildTargetPaths](co | use                               |
    | m/facebook/buck/core/model/impl/B | [`BuildPath                       |
    | uildTargetPaths.html "class in co | s`](com/facebook/buck/core/model/ |
    | m.facebook.buck.core.model.impl") | impl/BuildPaths.html "class in co |
    |                                   | m.facebook.buck.core.model.impl") |
    |                                   | instead, which handles flavoured  |
    |                                   | and unflavoured                   |
    |                                   | [`Bu                              |
    |                                   | ildTarget`](com/facebook/buck/cor |
    |                                   | e/model/BuildTarget.html "class i |
    |                                   | n com.facebook.buck.core.model")s |
    |                                   | in the paths the same way as      |
    |                                   | RE/[`ModernBuildRul               |
    |                                   | e`](com/facebook/buck/rules/moder |
    |                                   | n/ModernBuildRule.html "class in  |
    |                                   | com.facebook.buck.rules.modern")s |
    |                                   | do.                               |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [c                                |                                   |
    | om.facebook.buck.event.ThrowableC |                                   |
    | onsoleEvent](com/facebook/buck/ev |                                   |
    | ent/ThrowableConsoleEvent.html "c |                                   |
    | lass in com.facebook.buck.event") |                                   |
    +-----------------------------------+-----------------------------------+

    : Classes[ ]{.tabEnd}

[]{#field}

-   
      Field                                                                                                                                 Description
      ------------------------------------------------------------------------------------------------------------------------------------- -------------
      [com.facebook.buck.cli.AbstractQueryCommand.generateJsonOutput](com/facebook/buck/cli/AbstractQueryCommand.html#generateJsonOutput)   

      : Fields[ ]{.tabEnd}

[]{#method}

-   +-----------------------------------+-----------------------------------+
    | Method                            | Description                       |
    +===================================+===================================+
    | [com.face                         |                                   |
    | book.buck.core.filesystems.PathWr |                                   |
    | apper.equals​(Path)](com/facebook/ |                                   |
    | buck/core/filesystems/PathWrapper |                                   |
    | .html#equals(java.nio.file.Path)) |                                   |
    +-----------------------------------+-----------------------------------+
    | [com.facebook.buck.core.rules.Ac  |                                   |
    | tionGraphBuilder.addToIndex​(T)](c |                                   |
    | om/facebook/buck/core/rules/Actio |                                   |
    | nGraphBuilder.html#addToIndex(T)) |                                   |
    +-----------------------------------+-----------------------------------+
    | [com.facebook.buck.c              |                                   |
    | ore.rules.resolver.impl.MultiThre |                                   |
    | adedActionGraphBuilder.addToIndex |                                   |
    | ​(T)](com/facebook/buck/core/rules |                                   |
    | /resolver/impl/MultiThreadedActio |                                   |
    | nGraphBuilder.html#addToIndex(T)) |                                   |
    +-----------------------------------+-----------------------------------+
    | [com.facebook.buck.core.r         |                                   |
    | ules.resolver.impl.RuleAnalysisCo |                                   |
    | mpatibleDelegatingActionGraphBuil |                                   |
    | der.addToIndex​(T)](com/facebook/b |                                   |
    | uck/core/rules/resolver/impl/Rule |                                   |
    | AnalysisCompatibleDelegatingActio |                                   |
    | nGraphBuilder.html#addToIndex(T)) |                                   |
    +-----------------------------------+-----------------------------------+
    | [com.facebook.bu                  |                                   |
    | ck.core.test.rule.TestXRule.inter |                                   |
    | pretTestResults​(ExecutionContext, |                                   |
    | SourcePathResolverAdapter,        |                                   |
    | boolean)](com/facebook/           |                                   |
    | buck/core/test/rule/TestXRule.htm |                                   |
    | l#interpretTestResults(com.facebo |                                   |
    | ok.buck.core.build.execution.cont |                                   |
    | ext.ExecutionContext,com.facebook |                                   |
    | .buck.core.sourcepath.resolver.So |                                   |
    | urcePathResolverAdapter,boolean)) |                                   |
    +-----------------------------------+-----------------------------------+
    | [com.facebook                     |                                   |
    | .buck.core.test.rule.TestXRule.on |                                   |
    | PreTest​(BuildContext)](com/facebo |                                   |
    | ok/buck/core/test/rule/TestXRule. |                                   |
    | html#onPreTest(com.facebook.buck. |                                   |
    | core.build.context.BuildContext)) |                                   |
    +-----------------------------------+-----------------------------------+
    | [com                              |                                   |
    | .facebook.buck.core.test.rule.Tes |                                   |
    | tXRule.runTests​(ExecutionContext, |                                   |
    | TestRunningOptions, BuildContext, |                                   |
    | TestRule.TestR                    |                                   |
    | eportingCallback)](com/facebook/b |                                   |
    | uck/core/test/rule/TestXRule.html |                                   |
    | #runTests(com.facebook.buck.core. |                                   |
    | build.execution.context.Execution |                                   |
    | Context,com.facebook.buck.test.Te |                                   |
    | stRunningOptions,com.facebook.buc |                                   |
    | k.core.build.context.BuildContext |                                   |
    | ,com.facebook.buck.core.test.rule |                                   |
    | .TestRule.TestReportingCallback)) |                                   |
    +-----------------------------------+-----------------------------------+
    | [                                 |                                   |
    | com.facebook.buck.core.test.rule. |                                   |
    | TestXRule.runTestSeparately()](co |                                   |
    | m/facebook/buck/core/test/rule/Te |                                   |
    | stXRule.html#runTestSeparately()) |                                   |
    +-----------------------------------+-----------------------------------+
    | [com.facebo                       |                                   |
    | ok.buck.core.test.rule.TestXRule. |                                   |
    | supportsStreamingTests()](com/fac |                                   |
    | ebook/buck/core/test/rule/TestXRu |                                   |
    | le.html#supportsStreamingTests()) |                                   |
    +-----------------------------------+-----------------------------------+
    | [com.faceb                        | ::: deprecationComment            |
    | ook.buck.core.util.graph.Topologi | This is silly. You should just    |
    | calSort.snowflakeSort​(Iterable\<? | use the normal sort. This is here |
    | extends T\>,                      | because c/c++ link command lines  |
    | TopologicalSort.Traversable\<T\>, | are sensitive to argument order,  |
    | Comparator\<T\>)](com/fac         | but aren\'t strict about it being |
    | ebook/buck/core/util/graph/Topolo | correct. Since they aren\'t       |
    | gicalSort.html#snowflakeSort(java | strict, code has evolved to       |
    | .lang.Iterable,com.facebook.buck. | depend on the specific order that |
    | core.util.graph.TopologicalSort.T | Buck has been ordering link       |
    | raversable,java.util.Comparator)) | lines, and so this preserves that |
    |                                   | legacy behavior until code that   |
    |                                   | depends on it is fixed.           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [c                                | ::: deprecationComment            |
    | om.facebook.buck.cxx.toolchain.Ar | Use the non-legacy type.          |
    | chiverProvider.from​(ToolProvider, | :::                               |
    | Platform,                         |                                   |
    | O                                 |                                   |
    | ptional\<ArchiverProvider.LegacyA |                                   |
    | rchiverType\>)](com/facebook/buck |                                   |
    | /cxx/toolchain/ArchiverProvider.h |                                   |
    | tml#from(com.facebook.buck.core.t |                                   |
    | oolchain.toolprovider.ToolProvide |                                   |
    | r,com.facebook.buck.util.environm |                                   |
    | ent.Platform,java.util.Optional)) |                                   |
    +-----------------------------------+-----------------------------------+
    | [com.facebook.b                   |                                   |
    | uck.cxx.toolchain.nativelink.Lega |                                   |
    | cyNativeLinkableGroup.forceLinkWh |                                   |
    | oleForHaskellOmnibus()](com/faceb |                                   |
    | ook/buck/cxx/toolchain/nativelink |                                   |
    | /LegacyNativeLinkableGroup.html#f |                                   |
    | orceLinkWholeForHaskellOmnibus()) |                                   |
    +-----------------------------------+-----------------------------------+
    | [com.f                            |                                   |
    | acebook.buck.cxx.toolchain.native |                                   |
    | link.LegacyNativeLinkableGroup.ge |                                   |
    | tExportedLinkerFlags​(CxxPlatform, |                                   |
    | ActionGraphBu                     |                                   |
    | ilder)](com/facebook/buck/cxx/too |                                   |
    | lchain/nativelink/LegacyNativeLin |                                   |
    | kableGroup.html#getExportedLinker |                                   |
    | Flags(com.facebook.buck.cxx.toolc |                                   |
    | hain.CxxPlatform,com.facebook.buc |                                   |
    | k.core.rules.ActionGraphBuilder)) |                                   |
    +-----------------------------------+-----------------------------------+
    | [com.faceb                        |                                   |
    | ook.buck.cxx.toolchain.nativelink |                                   |
    | .LegacyNativeLinkableGroup.getExp |                                   |
    | ortedPostLinkerFlags​(CxxPlatform, |                                   |
    | ActionGraphBuilde                 |                                   |
    | r)](com/facebook/buck/cxx/toolcha |                                   |
    | in/nativelink/LegacyNativeLinkabl |                                   |
    | eGroup.html#getExportedPostLinker |                                   |
    | Flags(com.facebook.buck.cxx.toolc |                                   |
    | hain.CxxPlatform,com.facebook.buc |                                   |
    | k.core.rules.ActionGraphBuilder)) |                                   |
    +-----------------------------------+-----------------------------------+
    | [com.facebook.bu                  |                                   |
    | ck.cxx.toolchain.nativelink.Legac |                                   |
    | yNativeLinkableGroup.getNativeLin |                                   |
    | kableDepsForPlatform​(CxxPlatform, |                                   |
    | BuildRuleResolver)](c             |                                   |
    | om/facebook/buck/cxx/toolchain/na |                                   |
    | tivelink/LegacyNativeLinkableGrou |                                   |
    | p.html#getNativeLinkableDepsForPl |                                   |
    | atform(com.facebook.buck.cxx.tool |                                   |
    | chain.CxxPlatform,com.facebook.bu |                                   |
    | ck.core.rules.BuildRuleResolver)) |                                   |
    +-----------------------------------+-----------------------------------+
    | [com.facebook.buck.cxx.t          |                                   |
    | oolchain.nativelink.LegacyNativeL |                                   |
    | inkableGroup.getNativeLinkableExp |                                   |
    | ortedDepsForPlatform​(CxxPlatform, |                                   |
    | ActionGraphBuilder)](com/facebo   |                                   |
    | ok/buck/cxx/toolchain/nativelink/ |                                   |
    | LegacyNativeLinkableGroup.html#ge |                                   |
    | tNativeLinkableExportedDepsForPla |                                   |
    | tform(com.facebook.buck.cxx.toolc |                                   |
    | hain.CxxPlatform,com.facebook.buc |                                   |
    | k.core.rules.ActionGraphBuilder)) |                                   |
    +-----------------------------------+-----------------------------------+
    | [com.f                            |                                   |
    | acebook.buck.cxx.toolchain.native |                                   |
    | link.LegacyNativeLinkableGroup.ge |                                   |
    | tNativeLinkableInput​(CxxPlatform, |                                   |
    | Linker.LinkableDepType, boolean,  |                                   |
    | ActionGraphBuilder,               |                                   |
    | T                                 |                                   |
    | argetConfiguration)](com/facebook |                                   |
    | /buck/cxx/toolchain/nativelink/Le |                                   |
    | gacyNativeLinkableGroup.html#getN |                                   |
    | ativeLinkableInput(com.facebook.b |                                   |
    | uck.cxx.toolchain.CxxPlatform,com |                                   |
    | .facebook.buck.cxx.toolchain.link |                                   |
    | er.Linker.LinkableDepType,boolean |                                   |
    | ,com.facebook.buck.core.rules.Act |                                   |
    | ionGraphBuilder,com.facebook.buck |                                   |
    | .core.model.TargetConfiguration)) |                                   |
    +-----------------------------------+-----------------------------------+
    | [co                               |                                   |
    | m.facebook.buck.cxx.toolchain.nat |                                   |
    | ivelink.LegacyNativeLinkableGroup |                                   |
    | .getNativeLinkTarget​(CxxPlatform, |                                   |
    | ActionGrap                        |                                   |
    | hBuilder)](com/facebook/buck/cxx/ |                                   |
    | toolchain/nativelink/LegacyNative |                                   |
    | LinkableGroup.html#getNativeLinkT |                                   |
    | arget(com.facebook.buck.cxx.toolc |                                   |
    | hain.CxxPlatform,com.facebook.buc |                                   |
    | k.core.rules.ActionGraphBuilder)) |                                   |
    +-----------------------------------+-----------------------------------+
    | [com.faceboo                      |                                   |
    | k.buck.cxx.toolchain.nativelink.L |                                   |
    | egacyNativeLinkableGroup.getPrefe |                                   |
    | rredLinkage​(CxxPlatform)](com/fac |                                   |
    | ebook/buck/cxx/toolchain/nativeli |                                   |
    | nk/LegacyNativeLinkableGroup.html |                                   |
    | #getPreferredLinkage(com.facebook |                                   |
    | .buck.cxx.toolchain.CxxPlatform)) |                                   |
    +-----------------------------------+-----------------------------------+
    | [com.fac                          |                                   |
    | ebook.buck.cxx.toolchain.nativeli |                                   |
    | nk.LegacyNativeLinkableGroup.getR |                                   |
    | uleType()](com/facebook/buck/cxx/ |                                   |
    | toolchain/nativelink/LegacyNative |                                   |
    | LinkableGroup.html#getRuleType()) |                                   |
    +-----------------------------------+-----------------------------------+
    | [c                                |                                   |
    | om.facebook.buck.cxx.toolchain.na |                                   |
    | tivelink.LegacyNativeLinkableGrou |                                   |
    | p.getSharedLibraries​(CxxPlatform, |                                   |
    | ActionGra                         |                                   |
    | phBuilder)](com/facebook/buck/cxx |                                   |
    | /toolchain/nativelink/LegacyNativ |                                   |
    | eLinkableGroup.html#getSharedLibr |                                   |
    | aries(com.facebook.buck.cxx.toolc |                                   |
    | hain.CxxPlatform,com.facebook.buc |                                   |
    | k.core.rules.ActionGraphBuilder)) |                                   |
    +-----------------------------------+-----------------------------------+
    | [com.facebook                     |                                   |
    | .buck.cxx.toolchain.nativelink.Le |                                   |
    | gacyNativeLinkableGroup.isPrebuil |                                   |
    | tSOForHaskellOmnibus​(CxxPlatform, |                                   |
    | ActionGraphBuilder)]              |                                   |
    | (com/facebook/buck/cxx/toolchain/ |                                   |
    | nativelink/LegacyNativeLinkableGr |                                   |
    | oup.html#isPrebuiltSOForHaskellOm |                                   |
    | nibus(com.facebook.buck.cxx.toolc |                                   |
    | hain.CxxPlatform,com.facebook.buc |                                   |
    | k.core.rules.ActionGraphBuilder)) |                                   |
    +-----------------------------------+-----------------------------------+
    | [com.facebook.buc                 |                                   |
    | k.cxx.toolchain.nativelink.Legacy |                                   |
    | NativeLinkableGroup.shouldBeLinke |                                   |
    | dInAppleTestAndHost()](com/facebo |                                   |
    | ok/buck/cxx/toolchain/nativelink/ |                                   |
    | LegacyNativeLinkableGroup.html#sh |                                   |
    | ouldBeLinkedInAppleTestAndHost()) |                                   |
    +-----------------------------------+-----------------------------------+
    | [com.facebook.buck                |                                   |
    | .cxx.toolchain.nativelink.LegacyN |                                   |
    | ativeLinkableGroup.supportsOmnibu |                                   |
    | sLinking​(CxxPlatform)](com/facebo |                                   |
    | ok/buck/cxx/toolchain/nativelink/ |                                   |
    | LegacyNativeLinkableGroup.html#su |                                   |
    | pportsOmnibusLinking(com.facebook |                                   |
    | .buck.cxx.toolchain.CxxPlatform)) |                                   |
    +-----------------------------------+-----------------------------------+
    | [com.                             |                                   |
    | facebook.buck.cxx.toolchain.nativ |                                   |
    | elink.LegacyNativeLinkableGroup.s |                                   |
    | upportsOmnibusLinkingForHaskell​(C |                                   |
    | xxPlatform)](com/facebook/buck/cx |                                   |
    | x/toolchain/nativelink/LegacyNati |                                   |
    | veLinkableGroup.html#supportsOmni |                                   |
    | busLinkingForHaskell(com.facebook |                                   |
    | .buck.cxx.toolchain.CxxPlatform)) |                                   |
    +-----------------------------------+-----------------------------------+
    | [com.face                         | ::: deprecationComment            |
    | book.buck.cxx.toolchain.nativelin | Convert to a                      |
    | k.LegacyNativeLinkTargetGroup.get | [`NativeLink                      |
    | NativeLinkTargetDeps​(CxxPlatform, | Target`](com/facebook/buck/cxx/to |
    | ActionGraphBuild                  | olchain/nativelink/NativeLinkTarg |
    | er)](com/facebook/buck/cxx/toolch | et.html "interface in com.faceboo |
    | ain/nativelink/LegacyNativeLinkTa | k.buck.cxx.toolchain.nativelink") |
    | rgetGroup.html#getNativeLinkTarge | and use                           |
    | tDeps(com.facebook.buck.cxx.toolc | [`Nat                             |
    | hain.CxxPlatform,com.facebook.buc | iveLinkTarget.getNativeLinkTarget |
    | k.core.rules.ActionGraphBuilder)) | Deps(ActionGraphBuilder)`](com/fa |
    |                                   | cebook/buck/cxx/toolchain/nativel |
    |                                   | ink/NativeLinkTarget.html#getNati |
    |                                   | veLinkTargetDeps(com.facebook.buc |
    |                                   | k.core.rules.ActionGraphBuilder)) |
    |                                   | instead.                          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [com.facebook.buck.cxx.t          | ::: deprecationComment            |
    | oolchain.nativelink.LegacyNativeL | Convert to a                      |
    | inkTargetGroup.getNativeLinkTarge | [`NativeLink                      |
    | tMode​(CxxPlatform)](com/facebook/ | Target`](com/facebook/buck/cxx/to |
    | buck/cxx/toolchain/nativelink/Leg | olchain/nativelink/NativeLinkTarg |
    | acyNativeLinkTargetGroup.html#get | et.html "interface in com.faceboo |
    | NativeLinkTargetMode(com.facebook | k.buck.cxx.toolchain.nativelink") |
    | .buck.cxx.toolchain.CxxPlatform)) | and use                           |
    |                                   | [`Nati                            |
    |                                   | veLinkTarget.getNativeLinkTargetM |
    |                                   | ode()`](com/facebook/buck/cxx/too |
    |                                   | lchain/nativelink/NativeLinkTarge |
    |                                   | t.html#getNativeLinkTargetMode()) |
    |                                   | instead.                          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [com.facebook.b                   | ::: deprecationComment            |
    | uck.cxx.toolchain.nativelink.Lega | Convert to a                      |
    | cyNativeLinkTargetGroup.getNative | [`NativeLink                      |
    | LinkTargetOutputPath()](com/faceb | Target`](com/facebook/buck/cxx/to |
    | ook/buck/cxx/toolchain/nativelink | olchain/nativelink/NativeLinkTarg |
    | /LegacyNativeLinkTargetGroup.html | et.html "interface in com.faceboo |
    | #getNativeLinkTargetOutputPath()) | k.buck.cxx.toolchain.nativelink") |
    |                                   | and use                           |
    |                                   | [`Nati                            |
    |                                   | veLinkTarget.getNativeLinkTargetM |
    |                                   | ode()`](com/facebook/buck/cxx/too |
    |                                   | lchain/nativelink/NativeLinkTarge |
    |                                   | t.html#getNativeLinkTargetMode()) |
    |                                   | instead.                          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [com.facebook.buck.event.listen   |                                   |
    | er.AbstractConsoleEventBusListene |                                   |
    | r.getWorkingTimeFromLastStartUnti |                                   |
    | lNow​(Collection\<EventInterval\>, |                                   |
    | long)](c                          |                                   |
    | om/facebook/buck/event/listener/A |                                   |
    | bstractConsoleEventBusListener.ht |                                   |
    | ml#getWorkingTimeFromLastStartUnt |                                   |
    | ilNow(java.util.Collection,long)) |                                   |
    +-----------------------------------+-----------------------------------+
    | [com.facebook.buck.event          |                                   |
    | .listener.AbstractConsoleEventBus |                                   |
    | Listener.logEventInterval​(String, |                                   |
    | Optional\<String\>, long, long,   |                                   |
    | Collection\<EventInterval\>,      |                                   |
    | Optional\<Double\>,               |                                   |
    | Optional\<Long\>,                 |                                   |
    | ImmutableLi                       |                                   |
    | st.Builder\<String\>)](com/facebo |                                   |
    | ok/buck/event/listener/AbstractCo |                                   |
    | nsoleEventBusListener.html#logEve |                                   |
    | ntInterval(java.lang.String,java. |                                   |
    | util.Optional,long,long,java.util |                                   |
    | .Collection,java.util.Optional,ja |                                   |
    | va.util.Optional,com.google.commo |                                   |
    | n.collect.ImmutableList.Builder)) |                                   |
    +-----------------------------------+-----------------------------------+
    | [com.facebook.buck.event.list     |                                   |
    | ener.RenderingConsole.printToStdO |                                   |
    | ut​(String)](com/facebook/buck/eve |                                   |
    | nt/listener/RenderingConsole.html |                                   |
    | #printToStdOut(java.lang.String)) |                                   |
    +-----------------------------------+-----------------------------------+
    | [com.faceb                        |                                   |
    | ook.buck.io.filesystem.ProjectFil |                                   |
    | esystem.getDirectoryContents​(Path |                                   |
    | )](com/facebook/buck/io/filesyste |                                   |
    | m/ProjectFilesystem.html#getDirec |                                   |
    | toryContents(java.nio.file.Path)) |                                   |
    +-----------------------------------+-----------------------------------+
    | [com                              |                                   |
    | .facebook.buck.io.filesystem.Proj |                                   |
    | ectFilesystem.getFilesUnderPath​(P |                                   |
    | ath)](com/facebook/buck/io/filesy |                                   |
    | stem/ProjectFilesystem.html#getFi |                                   |
    | lesUnderPath(java.nio.file.Path)) |                                   |
    +-----------------------------------+-----------------------------------+
    | [com.facebook.b                   |                                   |
    | uck.io.filesystem.ProjectFilesyst |                                   |
    | em.isIgnored​(RelPath)](com/facebo |                                   |
    | ok/buck/io/filesystem/ProjectFile |                                   |
    | system.html#isIgnored(com.faceboo |                                   |
    | k.buck.core.filesystems.RelPath)) |                                   |
    +-----------------------------------+-----------------------------------+
    | [co                               |                                   |
    | m.facebook.buck.io.filesystem.Pro |                                   |
    | jectFilesystem.walkFileTree​(Path, |                                   |
    | File                              |                                   |
    | Visitor\<Path\>)](com/facebook/bu |                                   |
    | ck/io/filesystem/ProjectFilesyste |                                   |
    | m.html#walkFileTree(java.nio.file |                                   |
    | .Path,java.nio.file.FileVisitor)) |                                   |
    +-----------------------------------+-----------------------------------+
    | [com.facebo                       |                                   |
    | ok.buck.io.filesystem.ProjectFile |                                   |
    | system.walkRelativeFileTree​(Path, |                                   |
    | FileVisitor\                      |                                   |
    | <Path\>)](com/facebook/buck/io/fi |                                   |
    | lesystem/ProjectFilesystem.html#w |                                   |
    | alkRelativeFileTree(java.nio.file |                                   |
    | .Path,java.nio.file.FileVisitor)) |                                   |
    +-----------------------------------+-----------------------------------+
    | [com.face                         | ::: deprecationComment            |
    | book.buck.parser.Parser.getTarget | Prefer                            |
    | NodeRawAttributes​(ParsingContext, | [`                                |
    | TargetNode\<?\>,                  | Parser.getTargetNodeRawAttributes |
    | DependencyStack)](com/faceb       | (PerBuildState, Cell, TargetNode, |
    | ook/buck/parser/Parser.html#getTa |       DependencyStack)`](com/face |
    | rgetNodeRawAttributes(com.faceboo | book/buck/parser/Parser.html#getT |
    | k.buck.parser.ParsingContext,com. | argetNodeRawAttributes(com.facebo |
    | facebook.buck.core.model.targetgr | ok.buck.parser.PerBuildState,com. |
    | aph.TargetNode,com.facebook.buck. | facebook.buck.core.cell.Cell,com. |
    | core.exceptions.DependencyStack)) | facebook.buck.core.model.targetgr |
    |                                   | aph.TargetNode,com.facebook.buck. |
    |                                   | core.exceptions.DependencyStack)) |
    |                                   | and reusing a PerBuildState       |
    |                                   | instance, especially when calling |
    |                                   | in a loop.                        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [com.facebook                     |                                   |
    | .buck.rules.keys.RuleKeyAppendabl |                                   |
    | e.appendToRuleKey​(RuleKeyAppendab |                                   |
    | le.RuleKeyAppendableSink)](com/fa |                                   |
    | cebook/buck/rules/keys/RuleKeyApp |                                   |
    | endable.html#appendToRuleKey(com. |                                   |
    | facebook.buck.rules.keys.RuleKeyA |                                   |
    | ppendable.RuleKeyAppendableSink)) |                                   |
    +-----------------------------------+-----------------------------------+
    | [com.facebook.buck                |                                   |
    | .rules.keys.RuleKeyAppendable.Rul |                                   |
    | eKeyAppendableSink.addValue​(Path, |                                   |
    | SourcePath)](com/facebook/buc     |                                   |
    | k/rules/keys/RuleKeyAppendable.Ru |                                   |
    | leKeyAppendableSink.html#addValue |                                   |
    | (java.nio.file.Path,com.facebook. |                                   |
    | buck.core.sourcepath.SourcePath)) |                                   |
    +-----------------------------------+-----------------------------------+

    : Methods[ ]{.tabEnd}
:::
:::

::: bottomNav
[]{#navbar.bottom}

::: skipNav
[Skip navigation links](#skip.navbar.bottom "Skip navigation links")
:::

[]{#navbar.bottom.firstrow}

-   [Overview](index.html)
-   Package
-   Class
-   [Tree](overview-tree.html)
-   Deprecated
-   [Index](index-all.html)
-   [Help](help-doc.html)
:::

::: subNav
-   [All Classes](allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

[]{#skip.navbar.bottom}
:::

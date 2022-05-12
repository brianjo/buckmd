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
# Package com.facebook.buck.rules.modern {#package-com.facebook.buck.rules.modern .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [Builda                           | ::: block                         |
    | ble](Buildable.html "interface in | A Buildable is the core of a      |
    |  com.facebook.buck.rules.modern") | ModernBuildRule.                  |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuildCellRe                      |                                   |
    | lativePathFactory](BuildCellRelat |                                   |
    | ivePathFactory.html "interface in |                                   |
    |  com.facebook.buck.rules.modern") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ClassInfo                        | ::: block                         |
    | ](ClassInfo.html "interface in co | ClassInfo is used by              |
    | m.facebook.buck.rules.modern")\<T | ModernBuildRule to extract        |
    | extends                           | information from an AddsToRuleKey |
    | [Ad                               | instance.                         |
    | dsToRuleKey](../../core/rulekey/A | :::                               |
    | ddsToRuleKey.html "interface in c |                                   |
    | om.facebook.buck.core.rulekey")\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [Custom                           | ::: block                         |
    | ClassSerialization](CustomClassSe | Allows a class to follow specify  |
    | rialization.html "interface in co | its serialization/deserialization |
    | m.facebook.buck.rules.modern")\<T | in terms of calls to the          |
    | extends                           | ValueVisitor/ValueCreator.        |
    | [Ad                               | :::                               |
    | dsToRuleKey](../../core/rulekey/A |                                   |
    | ddsToRuleKey.html "interface in c |                                   |
    | om.facebook.buck.core.rulekey")\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [CustomFieldDeps](Custom          | ::: block                         |
    | FieldDeps.html "interface in com. | Allows custom derivation of the   |
    | facebook.buck.rules.modern")\<T\> | deps corresponding to a field.    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CustomFieldInputs](CustomFi      | ::: block                         |
    | eldInputs.html "interface in com. | Allows custom derivation of the   |
    | facebook.buck.rules.modern")\<T\> | inputs corresponding to a field.  |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CustomFi                         | ::: block                         |
    | eldSerialization](CustomFieldSeri | Allows the                        |
    | alization.html "interface in com. | serialization/deserialization of  |
    | facebook.buck.rules.modern")\<T\> | a specific field to be specified  |
    |                                   | in terms of calls to the          |
    |                                   | ValueVisitor/Creator.             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Des                              | ::: block                         |
    | erializer.ClassFinder](Deserializ | Used for looking up classes.      |
    | er.ClassFinder.html "interface in | :::                               |
    |  com.facebook.buck.rules.modern") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Deser                            | ::: block                         |
    | ializer.DataProvider](Deserialize | DataProviders are used for        |
    | r.DataProvider.html "interface in | deserializing \"dynamic\"         |
    |  com.facebook.buck.rules.modern") | objects.                          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [HasBrok                          | ::: block                         |
    | enInputBasedRuleKey](HasBrokenInp | Used to indicate that this        |
    | utBasedRuleKey.html "interface in | Buildable\'s input-based key      |
    |  com.facebook.buck.rules.modern") | doesn\'t properly reflect all the |
    |                                   | inputs to this rule.              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [InputRuleResolver](Inp           |                                   |
    | utRuleResolver.html "interface in |                                   |
    |  com.facebook.buck.rules.modern") |                                   |
    +-----------------------------------+-----------------------------------+
    | [InputRuleResolver.Uns            | ::: block                         |
    | afeInternals](InputRuleResolver.U | Encapsulates some exposed         |
    | nsafeInternals.html "interface in | internal implementation details.  |
    |  com.facebook.buck.rules.modern") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [OutputPathResolver](Outp         | ::: block                         |
    | utPathResolver.html "interface in | Provides Buildable\'s a way to    |
    |  com.facebook.buck.rules.modern") | construct Paths to outputs.       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PipelinedBuildable](PipelinedBu  | ::: block                         |
    | ildable.html "interface in com.fa | Interface for the buildable of a  |
    | cebook.buck.rules.modern")\<State | PipelinedModernBuildRule.         |
    | extends                           | :::                               |
    | [RulePipelineState](../..         |                                   |
    | /core/rules/pipeline/RulePipeline |                                   |
    | State.html "interface in com.face |                                   |
    | book.buck.core.rules.pipeline")\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [Serializer.Delegate](Seria       | ::: block                         |
    | lizer.Delegate.html "interface in | The first time a \"dynamic\"      |
    |  com.facebook.buck.rules.modern") | object is encountered (including  |
    |                                   | Buildables themselves),           |
    |                                   | registerNewValue will be called.  |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ValueCreator](V                  | ::: block                         |
    | alueCreator.html "interface in co | A ValueCreator can be used to     |
    | m.facebook.buck.rules.modern")\<E | create the values referenced from |
    | extends                           | a Buildable.                      |
    | [Exception](ht                    | :::                               |
    | tp://docs.oracle.com/javase/7/doc |                                   |
    | s/api/java/lang/Exception.html?is |                                   |
    | -external=true "class or interfac |                                   |
    | e in java.lang"){.externalLink}\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [ValueTypeInfo](Valu              | ::: block                         |
    | eTypeInfo.html "interface in com. | ValueTypeInfo\<T\> provides       |
    | facebook.buck.rules.modern")\<T\> | methods to extract deps, outputs, |
    |                                   | rulekeys from values of type T.   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ValueVisitor](V                  | ::: block                         |
    | alueVisitor.html "interface in co | A ValueVisitor can be used to     |
    | m.facebook.buck.rules.modern")\<E | visit all the values referenced   |
    | extends                           | from a Buildable.                 |
    | [Exception](ht                    | :::                               |
    | tp://docs.oracle.com/javase/7/doc |                                   |
    | s/api/java/lang/Exception.html?is |                                   |
    | -external=true "class or interfac |                                   |
    | e in java.lang"){.externalLink}\> |                                   |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [CustomBehaviorUtils](C           | ::: block                         |
    | ustomBehaviorUtils.html "class in | Utilities for dealing with        |
    |  com.facebook.buck.rules.modern") | CustomFieldBehavior and           |
    |                                   | CustomClassBehavior.              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [DefaultBuildCellRelat            |                                   |
    | ivePathFactory](DefaultBuildCellR |                                   |
    | elativePathFactory.html "class in |                                   |
    |  com.facebook.buck.rules.modern") |                                   |
    +-----------------------------------+-----------------------------------+
    | [D                                | ::: block                         |
    | efaultOutputPathResolver](Default | Default OutputPathResolver        |
    | OutputPathResolver.html "class in | implementation.                   |
    |  com.facebook.buck.rules.modern") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Deserial                         | ::: block                         |
    | izer](Deserializer.html "class in | Implements deserialization of     |
    |  com.facebook.buck.rules.modern") | Buildables.                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [EmptyMemoize                     | ::: block                         |
    | rDeserialization](EmptyMemoizerDe | Supports deserialization of a     |
    | serialization.html "class in com. | memoizer as just a                |
    | facebook.buck.rules.modern")\<T\> | default-constructed empty         |
    |                                   | Memoizer.                         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [FieldIn                          | ::: block                         |
    | fo](FieldInfo.html "class in com. | Holds a java.lang.reflect.Field   |
    | facebook.buck.rules.modern")\<T\> | and a ValueTypeInfo for a field   |
    |                                   | referenced from a Buildable.      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ModernBuildRule](                | ::: block                         |
    | ModernBuildRule.html "class in co | ModernBuildRule wraps a Buildable |
    | m.facebook.buck.rules.modern")\<T | into something that implements    |
    | extends                           | BuildRule (and various other      |
    | [Buildabl                         | interfaces used by the build      |
    | e](Buildable.html "interface in c | engine).                          |
    | om.facebook.buck.rules.modern")\> | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Outp                             | ::: block                         |
    | utPath](OutputPath.html "class in | Represents an output path of a    |
    |  com.facebook.buck.rules.modern") | Buildable.                        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [OutputPath.Internals](Ou         | ::: block                         |
    | tputPath.Internals.html "class in | Provides access to internal       |
    |  com.facebook.buck.rules.modern") | implementation details of         |
    |                                   | OutputPaths.                      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PathSerialization]               | ::: block                         |
    | (PathSerialization.html "class in | This can be used for              |
    |  com.facebook.buck.rules.modern") | serialization/deserialization of  |
    |                                   | Paths (in such a way that         |
    |                                   | absolute paths will be updated    |
    |                                   | for the new context).             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Pipeli                           | ::: block                         |
    | nedModernBuildRule](PipelinedMode | A ModernBuildRule that            |
    | rnBuildRule.html "class in com.fa | \@SupportsPipelining.             |
    | cebook.buck.rules.modern")\<State | :::                               |
    | extends                           |                                   |
    | [RulePipelineState](../..         |                                   |
    | /core/rules/pipeline/RulePipeline |                                   |
    | State.html "interface in com.face |                                   |
    | book.buck.core.rules.pipeline"),​T |                                   |
    | extends                           |                                   |
    | [Pi                               |                                   |
    | pelinedBuildable](PipelinedBuilda |                                   |
    | ble.html "interface in com.facebo |                                   |
    | ok.buck.rules.modern")\<State\>\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [PlatformSerialization](Pla       | ::: block                         |
    | tformSerialization.html "class in | This can be used for              |
    |  com.facebook.buck.rules.modern") | serialization/deserialization of  |
    |                                   | Platform.                         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PublicOutputPath                 | ::: block                         |
    | ](PublicOutputPath.html "class in | Used for an output path that is   |
    |  com.facebook.buck.rules.modern") | not contained within a rule\'s    |
    |                                   | unique output directories.        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RemoteExecutionEnabled](Remo     | ::: block                         |
    | teExecutionEnabled.html "class in | A                                 |
    |  com.facebook.buck.rules.modern") | [`Cust                            |
    |                                   | omFieldSerialization`](CustomFiel |
    |                                   | dSerialization.html "interface in |
    |                                   |  com.facebook.buck.rules.modern") |
    |                                   | that will disable remote          |
    |                                   | execution for the referencing     |
    |                                   | rule if the field holds a false   |
    |                                   | value.                            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Seri                             | ::: block                         |
    | alizer](Serializer.html "class in | Implementation of Serialization   |
    |  com.facebook.buck.rules.modern") | of Buildables.                    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [SourcePathRes                    | ::: block                         |
    | olverSerialization](SourcePathRes | Uses ValueCreator.createSpecial() |
    | olverSerialization.html "class in | to create a                       |
    |  com.facebook.buck.rules.modern") | SourcePathResolverAdapter.        |
    |                                   | :::                               |
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

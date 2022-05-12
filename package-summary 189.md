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
# Package com.facebook.buck.rules.coercer {#package-com.facebook.buck.rules.coercer .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [Cons                             | ::: block                         |
    | tructorArgMarshaller](Constructor | Used to derive information from   |
    | ArgMarshaller.html "interface in  | the constructor args returned by  |
    | com.facebook.buck.rules.coercer") | [`DescriptionWithTargetGr         |
    |                                   | aph`](../../core/rules/Descriptio |
    |                                   | nWithTargetGraph.html "interface  |
    |                                   | in com.facebook.buck.core.rules") |
    |                                   | instances.                        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [DataTransferObjectDescript       | ::: block                         |
    | or.BuilderBuildFunction](DataTran | A function to build a builder     |
    | sferObjectDescriptor.BuilderBuild | returned by                       |
    | Function.html "interface in com.f | [`DataTr                          |
    | acebook.buck.rules.coercer")\<T\> | ansferObjectDescriptor.getBuilder |
    |                                   | Factory()`](DataTransferObjectDes |
    |                                   | criptor.html#getBuilderFactory()) |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ParamInfo](P                     | ::: block                         |
    | aramInfo.html "interface in com.f | Represents a single field that    |
    | acebook.buck.rules.coercer")\<T\> | can be represented in buck build  |
    |                                   | files.                            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ParamInfo.Traversal](ParamI      | ::: block                         |
    | nfo.Traversal.html "interface in  | Traversal interface used when     |
    | com.facebook.buck.rules.coercer") | coercing values                   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [TypeCoercer](TypeC               | ::: block                         |
    | oercer.html "interface in com.fac | Class defining an interpretation  |
    | ebook.buck.rules.coercer")\<U,​T\> | of some dynamically typed Java    |
    |                                   | object as a specific class.       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [TypeCoercer.Traversal](TypeCoer  |                                   |
    | cer.Traversal.html "interface in  |                                   |
    | com.facebook.buck.rules.coercer") |                                   |
    +-----------------------------------+-----------------------------------+
    | [TypeCoercerFactory](TypeC        |                                   |
    | oercerFactory.html "interface in  |                                   |
    | com.facebook.buck.rules.coercer") |                                   |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [AbsoluteOutp                     | ::: block                         |
    | utMacroTypeCoercer](AbsoluteOutpu | Handles \'\$(output \...)\'       |
    | tMacroTypeCoercer.html "class in  | macro.                            |
    | com.facebook.buck.rules.coercer") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AbstractParamInfo](Abstr         | ::: block                         |
    | actParamInfo.html "class in com.f | Represents a single field that    |
    | acebook.buck.rules.coercer")\<T\> | can be represented in buck build  |
    |                                   | files.                            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuildConfigFields](              | ::: block                         |
    | BuildConfigFields.html "class in  | List of fields to add to a        |
    | com.facebook.buck.rules.coercer") | generated `BuildConfig.java`      |
    |                                   | file.                             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuildConfigFields.Field](BuildC  | ::: block                         |
    | onfigFields.Field.html "class in  | An individual field in a          |
    | com.facebook.buck.rules.coercer") | [`BuildConfigFields`](B           |
    |                                   | uildConfigFields.html "class in c |
    |                                   | om.facebook.buck.rules.coercer"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuildCon                         | ::: block                         |
    | figFieldsTypeCoercer](BuildConfig | [`TypeCoercer`                    |
    | FieldsTypeCoercer.html "class in  | ](TypeCoercer.html "interface in  |
    | com.facebook.buck.rules.coercer") | com.facebook.buck.rules.coercer") |
    |                                   | that takes a list of strings and  |
    |                                   | transforms it into a              |
    |                                   | [`BuildConfigFields`](B           |
    |                                   | uildConfigFields.html "class in c |
    |                                   | om.facebook.buck.rules.coercer"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuildTarg                        | ::: block                         |
    | etMacroTypeCoercer](BuildTargetMa | Coercer for macros which take a   |
    | croTypeCoercer.html "class in com | single                            |
    | .facebook.buck.rules.coercer")\<M | [`BuildTarget`](../../co          |
    | extends                           | re/model/BuildTarget.html "class  |
    | [BuildTargetMacro](../macros/     | in com.facebook.buck.core.model") |
    | BuildTargetMacro.html "class in c | arg.                              |
    | om.facebook.buck.rules.macros")\> | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuildTargetTypeCoercer](Build    | ::: block                         |
    | TargetTypeCoercer.html "class in  | Coerce to                         |
    | com.facebook.buck.rules.coercer") | [`BuildTarget`](../../cor         |
    |                                   | e/model/BuildTarget.html "class i |
    |                                   | n com.facebook.buck.core.model"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuildTargetWithOut               | ::: block                         |
    | putsTypeCoercer](BuildTargetWithO | Coercer for                       |
    | utputsTypeCoercer.html "class in  | [`BuildTarget`](../../co          |
    | com.facebook.buck.rules.coercer") | re/model/BuildTarget.html "class  |
    |                                   | in com.facebook.buck.core.model") |
    |                                   | instances that can optionally     |
    |                                   | have output labels.               |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CollectionTypeCoercer](Collect   | ::: block                         |
    | ionTypeCoercer.html "class in com | Base class for                    |
    | .facebook.buck.rules.coercer")\<D | `ImmutableCollection` subclasses  |
    | extends                           | coercers.                         |
    | com.google.common.c               | :::                               |
    | ollect.ImmutableCollection\<U\>,​C |                                   |
    | extends                           |                                   |
    | com.google.common.colle           |                                   |
    | ct.ImmutableCollection\<T\>,​U,​T\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [ConstraintTypeCoercer](Cons      | ::: block                         |
    | traintTypeCoercer.html "class in  | Coerce to                         |
    | com.facebook.buck.rules.coercer") | [`Constraint`](../../ve           |
    |                                   | rsions/Constraint.html "interface |
    |                                   |  in com.facebook.buck.versions"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CxxGen                           | ::: block                         |
    | ruleFilterAndTargetsMacroTypeCoer | Coercer for `cxx_genrule`         |
    | cer](CxxGenruleFilterAndTargetsMa | flag-based macros.                |
    | croTypeCoercer.html "class in com | :::                               |
    | .facebook.buck.rules.coercer")\<M |                                   |
    | extends                           |                                   |
    | [CxxGenruleFilterAndTarget        |                                   |
    | sMacro](../macros/CxxGenruleFilte |                                   |
    | rAndTargetsMacro.html "class in c |                                   |
    | om.facebook.buck.rules.macros")\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [CxxL                             | ::: block                         |
    | inkGroupMappingCoercer](CxxLinkGr | [`TypeCoercer`                    |
    | oupMappingCoercer.html "class in  | ](TypeCoercer.html "interface in  |
    | com.facebook.buck.rules.coercer") | com.facebook.buck.rules.coercer") |
    |                                   | for                               |
    |                                   | [`CxxLinkGroupMa                  |
    |                                   | pping`](../../core/linkgroup/CxxL |
    |                                   | inkGroupMapping.html "class in co |
    |                                   | m.facebook.buck.core.linkgroup"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CxxLinkGroupMapp                 | ::: block                         |
    | ingTargetCoercer](CxxLinkGroupMap | [`TypeCoercer`                    |
    | pingTargetCoercer.html "class in  | ](TypeCoercer.html "interface in  |
    | com.facebook.buck.rules.coercer") | com.facebook.buck.rules.coercer") |
    |                                   | for                               |
    |                                   | [`CxxLinkGroupMappingTarget`      |
    |                                   | ](../../core/linkgroup/CxxLinkGro |
    |                                   | upMappingTarget.html "class in co |
    |                                   | m.facebook.buck.core.linkgroup"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [C                                | ::: block                         |
    | xxLinkGroupMappingTargetTraversal | [`TypeCoercer`                    |
    | Coercer](CxxLinkGroupMappingTarge | ](TypeCoercer.html "interface in  |
    | tTraversalCoercer.html "class in  | com.facebook.buck.rules.coercer") |
    | com.facebook.buck.rules.coercer") | for                               |
    |                                   | [`CxxLinkGroup                    |
    |                                   | MappingTarget.Traversal`](../../c |
    |                                   | ore/linkgroup/CxxLinkGroupMapping |
    |                                   | Target.Traversal.html "enum in co |
    |                                   | m.facebook.buck.core.linkgroup"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [DataTransfe                      | ::: block                         |
    | rObjectDescriptor](DataTransferOb | Class that contains the values    |
    | jectDescriptor.html "class in com | needed to build a DescriptionArg  |
    | .facebook.buck.rules.coercer")\<T | :::                               |
    | extends                           |                                   |
    | [DataTransferObject](../../co     |                                   |
    | re/description/arg/DataTransferOb |                                   |
    | ject.html "interface in com.faceb |                                   |
    | ook.buck.core.description.arg")\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [DefaultConstru                   |                                   |
    | ctorArgMarshaller](DefaultConstru |                                   |
    | ctorArgMarshaller.html "class in  |                                   |
    | com.facebook.buck.rules.coercer") |                                   |
    +-----------------------------------+-----------------------------------+
    | [De                               | ::: block                         |
    | faultTypeCoercerFactory](DefaultT | Create                            |
    | ypeCoercerFactory.html "class in  | [`TypeCoercer`]                   |
    | com.facebook.buck.rules.coercer") | (TypeCoercer.html "interface in c |
    |                                   | om.facebook.buck.rules.coercer")s |
    |                                   | that can convert incoming java    |
    |                                   | structures (from json) into       |
    |                                   | particular types.                 |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Either                           | ::: block                         |
    | TypeCoercer](EitherTypeCoercer.ht | Coerces a type to either type,    |
    | ml "class in com.facebook.buck.ru | trying the left type before the   |
    | les.coercer")\<LU,​RU,​Left,​Right\> | right.                            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [EnumTypeCoercer](E               | ::: block                         |
    | numTypeCoercer.html "class in com | Coerce a string to java enum.     |
    | .facebook.buck.rules.coercer")\<E | :::                               |
    | extends                           |                                   |
    | [Enum](ht                         |                                   |
    | tp://docs.oracle.com/javase/7/doc |                                   |
    | s/api/java/lang/Enum.html?is-exte |                                   |
    | rnal=true "class or interface in  |                                   |
    | java.lang"){.externalLink}\<E\>\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [EnvMacroTypeCoercer](En          | ::: block                         |
    | vMacroTypeCoercer.html "class in  | Coercer for `env` macros.         |
    | com.facebook.buck.rules.coercer") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [FlavorTypeCoercer](              | ::: block                         |
    | FlavorTypeCoercer.html "class in  | Coerce to                         |
    | com.facebook.buck.rules.coercer") | [`Flavor`](../../co               |
    |                                   | re/model/Flavor.html "interface i |
    |                                   | n com.facebook.buck.core.model"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [FrameworkPa                      | ::: block                         |
    | th](FrameworkPath.html "class in  | Frameworks can be specified as    |
    | com.facebook.buck.rules.coercer") | either a path to a file, or a     |
    |                                   | path prefixed by a build setting. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [                                 | ::: block                         |
    | FrameworkPathTypeCoercer](Framewo | Coerce to                         |
    | rkPathTypeCoercer.html "class in  | [`FrameworkPath                   |
    | com.facebook.buck.rules.coercer") | `](FrameworkPath.html "class in c |
    |                                   | om.facebook.buck.rules.coercer"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [IdentityTypeCoercer](Identit     | ::: block                         |
    | yTypeCoercer.html "class in com.f | Coercer that just expect JSON     |
    | acebook.buck.rules.coercer")\<T\> | type is already what we expect.   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ImmutableTypeCoercer](Immuta     | ::: block                         |
    | bleTypeCoercer.html "class in com | A coercer for Immutables using    |
    | .facebook.buck.rules.coercer")\<T | the same flow as Description\'s   |
    | extends                           | args                              |
    | [DataTransferObject](../../co     | :::                               |
    | re/description/arg/DataTransferOb |                                   |
    | ject.html "interface in com.faceb |                                   |
    | ook.buck.core.description.arg")\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [LeafTypeCoercer](Lea             | ::: block                         |
    | fTypeCoercer.html "class in com.f | Superclass of coercers for        |
    | acebook.buck.rules.coercer")\<T\> | non-collection/map types.         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [LeafTypeNewCoercer](LeafType     | ::: block                         |
    | NewCoercer.html "class in com.fac | Superclass of coercers for        |
    | ebook.buck.rules.coercer")\<U,​T\> | non-collection/map types.         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [LeafUnconfi                      | ::: block                         |
    | guredOnlyCoercer](LeafUnconfigure | Second phase coercion is          |
    | dOnlyCoercer.html "class in com.f | identity.                         |
    | acebook.buck.rules.coercer")\<T\> | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ListTypeCoercer](ListT           | ::: block                         |
    | ypeCoercer.html "class in com.fac | Coere to `ImmutableList`.         |
    | ebook.buck.rules.coercer")\<U,​T\> | :::                               |
    +-----------------------------------+-----------------------------------+
    | [LogLevelTypeCoercer](Lo          | ::: block                         |
    | gLevelTypeCoercer.html "class in  | Coercer for                       |
    | com.facebook.buck.rules.coercer") | [`Level`](http://docs.o           |
    |                                   | racle.com/javase/7/docs/api/java/ |
    |                                   | util/logging/Level.html?is-extern |
    |                                   | al=true "class or interface in ja |
    |                                   | va.util.logging"){.externalLink}. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ManifestEntries                  | ::: block                         |
    | ](ManifestEntries.html "class in  | Manifest entries to be injected   |
    | com.facebook.buck.rules.coercer") | into the AndroidManifest.xml file |
    |                                   | via AAPT command line flags.      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ManifestEntries.Builder](Manife  |                                   |
    | stEntries.Builder.html "class in  |                                   |
    | com.facebook.buck.rules.coercer") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Mani                             | ::: block                         |
    | festEntriesTypeCoercer](ManifestE | [`TypeCoercer`                    |
    | ntriesTypeCoercer.html "class in  | ](TypeCoercer.html "interface in  |
    | com.facebook.buck.rules.coercer") | com.facebook.buck.rules.coercer") |
    |                                   | that takes a dict object          |
    |                                   | generated by the                  |
    |                                   | manifest_entries() python         |
    |                                   | function and coverts it to        |
    |                                   | [`ManifestEntries`]               |
    |                                   | (ManifestEntries.html "class in c |
    |                                   | om.facebook.buck.rules.coercer"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [MapTypeCoercer](MapTypeCoe       | ::: block                         |
    | rcer.html "class in com.facebook. | Coerce to `ImmutableMap`.         |
    | buck.rules.coercer")\<KU,​VU,​K,​V\> | :::                               |
    +-----------------------------------+-----------------------------------+
    | [NeededCoverageSpec](N            |                                   |
    | eededCoverageSpec.html "class in  |                                   |
    | com.facebook.buck.rules.coercer") |                                   |
    +-----------------------------------+-----------------------------------+
    | [NeededCove                       | ::: block                         |
    | rageSpecTypeCoercer](NeededCovera | A type coercer to handle needed   |
    | geSpecTypeCoercer.html "class in  | coverage specification for        |
    | com.facebook.buck.rules.coercer") | python_test.                      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [NumberTypeCoercer](Num           | ::: block                         |
    | berTypeCoercer.html "class in com | Coerces numbers with              |
    | .facebook.buck.rules.coercer")\<T | rounding/truncation/extension.    |
    | extends                           | :::                               |
    | [Number]                          |                                   |
    | (http://docs.oracle.com/javase/7/ |                                   |
    | docs/api/java/lang/Number.html?is |                                   |
    | -external=true "class or interfac |                                   |
    | e in java.lang"){.externalLink}\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [OptionalTypeCoercer](OptionalT   | ::: block                         |
    | ypeCoercer.html "class in com.fac | Coerce to                         |
    | ebook.buck.rules.coercer")\<U,​T\> | [`Optional`](                     |
    |                                   | http://docs.oracle.com/javase/7/d |
    |                                   | ocs/api/java/util/Optional.html?i |
    |                                   | s-external=true "class or interfa |
    |                                   | ce in java.util"){.externalLink}. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [OutputMacroTypeCoercer](Outpu    | ::: block                         |
    | tMacroTypeCoercer.html "class in  | Handles \'\$(output \...)\'       |
    | com.facebook.buck.rules.coercer") | macro.                            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Pair                             | ::: block                         |
    | TypeCoercer](PairTypeCoercer.html | Coerces from a 2-element          |
    |  "class in com.facebook.buck.rule | collection into a pair.           |
    | s.coercer")\<FU,​SU,​FIRST,​SECOND\> | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PathTypeCoercer                  | ::: block                         |
    | ](PathTypeCoercer.html "class in  | Coerce to                         |
    | com.facebook.buck.rules.coercer") | [`Path`](http                     |
    |                                   | ://docs.oracle.com/javase/7/docs/ |
    |                                   | api/java/nio/file/Path.html?is-ex |
    |                                   | ternal=true "class or interface i |
    |                                   | n java.nio.file"){.externalLink}. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Patte                            |                                   |
    | rnMatchedCollection](PatternMatch |                                   |
    | edCollection.html "class in com.f |                                   |
    | acebook.buck.rules.coercer")\<T\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [PatternMatchedCollect            |                                   |
    | ion.Builder](PatternMatchedCollec |                                   |
    | tion.Builder.html "class in com.f |                                   |
    | acebook.buck.rules.coercer")\<T\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [PatternMatchedCollectionTyp      |                                   |
    | eCoercer](PatternMatchedCollectio |                                   |
    | nTypeCoercer.html "class in com.f |                                   |
    | acebook.buck.rules.coercer")\<T\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [PatternTypeCoercer](P            | ::: block                         |
    | atternTypeCoercer.html "class in  | Coerce a string to                |
    | com.facebook.buck.rules.coercer") | [`Pattern`](http://docs           |
    |                                   | .oracle.com/javase/7/docs/api/jav |
    |                                   | a/util/regex/Pattern.html?is-exte |
    |                                   | rnal=true "class or interface in  |
    |                                   | java.util.regex"){.externalLink}. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [QueryCoer                        | ::: block                         |
    | cer](QueryCoercer.html "class in  | Coercer for                       |
    | com.facebook.buck.rules.coercer") | [`Query                           |
    |                                   | `](../query/Query.html "class in  |
    |                                   | com.facebook.buck.rules.query")s. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ReflectionParamInfo](Reflect     | ::: block                         |
    | ionParamInfo.html "class in com.f | Represents a single field that    |
    | acebook.buck.rules.coercer")\<T\> | can be represented in buck build  |
    |                                   | files, backed by an Immutable     |
    |                                   | DescriptionArg class              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [SetTypeCoercer](SetT             | ::: block                         |
    | ypeCoercer.html "class in com.fac | Coerce to `ImmutableSet`.         |
    | ebook.buck.rules.coercer")\<U,​T\> | :::                               |
    +-----------------------------------+-----------------------------------+
    | [SortedMapTypeCoercer](SortedM    | ::: block                         |
    | apTypeCoercer.html "class in com. | Coere to `ImmutableSortedMap`.    |
    | facebook.buck.rules.coercer")\<KU | :::                               |
    | extends                           |                                   |
    | [Comparable](http://docs.         |                                   |
    | oracle.com/javase/7/docs/api/java |                                   |
    | /lang/Comparable.html?is-external |                                   |
    | =true "class or interface in java |                                   |
    | .lang"){.externalLink}\<KU\>,​VU,​K |                                   |
    | extends                           |                                   |
    | [Comparable](http://doc           |                                   |
    | s.oracle.com/javase/7/docs/api/ja |                                   |
    | va/lang/Comparable.html?is-extern |                                   |
    | al=true "class or interface in ja |                                   |
    | va.lang"){.externalLink}\<K\>,​V\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [SortedSetConcatable](SortedS     |                                   |
    | etConcatable.html "class in com.f |                                   |
    | acebook.buck.rules.coercer")\<T\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [SortedSetTypeCoercer](SortedSe   | ::: block                         |
    | tTypeCoercer.html "class in com.f | Coerce to `ImmutableSortedSet`.   |
    | acebook.buck.rules.coercer")\<U,​T | :::                               |
    | extends                           |                                   |
    | [Comparable](http                 |                                   |
    | ://docs.oracle.com/javase/7/docs/ |                                   |
    | api/java/lang/Comparable.html?is- |                                   |
    | external=true "class or interface |                                   |
    |  in java.lang"){.externalLink}\<? |                                   |
    | super T\>\>                       |                                   |
    +-----------------------------------+-----------------------------------+
    | [SourcePathTypeCoercer](Sour      | ::: block                         |
    | cePathTypeCoercer.html "class in  | Coerce to                         |
    | com.facebook.buck.rules.coercer") | [`So                              |
    |                                   | urcePath`](../../core/sourcepath/ |
    |                                   | SourcePath.html "interface in com |
    |                                   | .facebook.buck.core.sourcepath"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Sou                              | ::: block                         |
    | rceSet](SourceSet.html "class in  | A group of ordered sources,       |
    | com.facebook.buck.rules.coercer") | stored as either a                |
    |                                   | [`                                |
    |                                   | Set`](http://docs.oracle.com/java |
    |                                   | se/7/docs/api/java/util/Set.html? |
    |                                   | is-external=true "class or interf |
    |                                   | ace in java.util"){.externalLink} |
    |                                   | of unnamed                        |
    |                                   | [`So                              |
    |                                   | urcePath`](../../core/sourcepath/ |
    |                                   | SourcePath.html "interface in com |
    |                                   | .facebook.buck.core.sourcepath")s |
    |                                   | or a                              |
    |                                   | [`                                |
    |                                   | Map`](http://docs.oracle.com/java |
    |                                   | se/7/docs/api/java/util/Map.html? |
    |                                   | is-external=true "class or interf |
    |                                   | ace in java.util"){.externalLink} |
    |                                   | of names to                       |
    |                                   | [`Sou                             |
    |                                   | rcePath`](../../core/sourcepath/S |
    |                                   | ourcePath.html "interface in com. |
    |                                   | facebook.buck.core.sourcepath")s. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [SourceSetConcatable](So          |                                   |
    | urceSetConcatable.html "class in  |                                   |
    | com.facebook.buck.rules.coercer") |                                   |
    +-----------------------------------+-----------------------------------+
    | [SourceSetTypeCoercer](Sou        | ::: block                         |
    | rceSetTypeCoercer.html "class in  | Coerce to                         |
    | com.facebook.buck.rules.coercer") | [`Sourc                           |
    |                                   | eSet`](SourceSet.html "class in c |
    |                                   | om.facebook.buck.rules.coercer"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [SourceSortedSet                  | ::: block                         |
    | ](SourceSortedSet.html "class in  | A group of sources, stored as     |
    | com.facebook.buck.rules.coercer") | either a                          |
    |                                   | [`SortedSet`](                    |
    |                                   | http://docs.oracle.com/javase/7/d |
    |                                   | ocs/api/java/util/SortedSet.html? |
    |                                   | is-external=true "class or interf |
    |                                   | ace in java.util"){.externalLink} |
    |                                   | of unnamed                        |
    |                                   | [`So                              |
    |                                   | urcePath`](../../core/sourcepath/ |
    |                                   | SourcePath.html "interface in com |
    |                                   | .facebook.buck.core.sourcepath")s |
    |                                   | or a                              |
    |                                   | [`SortedMap`](                    |
    |                                   | http://docs.oracle.com/javase/7/d |
    |                                   | ocs/api/java/util/SortedMap.html? |
    |                                   | is-external=true "class or interf |
    |                                   | ace in java.util"){.externalLink} |
    |                                   | of names to                       |
    |                                   | [`Sou                             |
    |                                   | rcePath`](../../core/sourcepath/S |
    |                                   | ourcePath.html "interface in com. |
    |                                   | facebook.buck.core.sourcepath")s. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [So                               |                                   |
    | urceSortedSetConcatable](SourceSo |                                   |
    | rtedSetConcatable.html "class in  |                                   |
    | com.facebook.buck.rules.coercer") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Sour                             |                                   |
    | ceSortedSetTypeCoercer](SourceSor |                                   |
    | tedSetTypeCoercer.html "class in  |                                   |
    | com.facebook.buck.rules.coercer") |                                   |
    +-----------------------------------+-----------------------------------+
    | [SourceWithFlagsList](So          | ::: block                         |
    | urceWithFlagsList.html "class in  | Simple type representing a list   |
    | com.facebook.buck.rules.coercer") | of                                |
    |                                   | [`SourceWi                        |
    |                                   | thFlags`](../../core/sourcepath/S |
    |                                   | ourceWithFlags.html "class in com |
    |                                   | .facebook.buck.core.sourcepath"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [SourceWithFl                     | ::: block                         |
    | agsListTypeCoercer](SourceWithFla | Coerce to                         |
    | gsListTypeCoercer.html "class in  | [`SourceWithFlagsList`](Sou       |
    | com.facebook.buck.rules.coercer") | rceWithFlagsList.html "class in c |
    |                                   | om.facebook.buck.rules.coercer"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Sour                             | ::: block                         |
    | ceWithFlagsTypeCoercer](SourceWit | A type coercer to handle source   |
    | hFlagsTypeCoercer.html "class in  | entries with a list of flags.     |
    | com.facebook.buck.rules.coercer") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [StringTypeCoercer](              | ::: block                         |
    | StringTypeCoercer.html "class in  | Coercer that turns objects into   |
    | com.facebook.buck.rules.coercer") | Strings, or throws an exception   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [String                           | ::: block                         |
    | WithMacrosTypeCoercer](StringWith | Coerce to                         |
    | MacrosTypeCoercer.html "class in  | [`StringWithMacros`](../macros    |
    | com.facebook.buck.rules.coercer") | /StringWithMacros.html "class in  |
    |                                   | com.facebook.buck.rules.macros"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [TestRunnerSpecCoercer](Test      | ::: block                         |
    | RunnerSpecCoercer.html "class in  | Coerces a freeform JSON as a      |
    | com.facebook.buck.rules.coercer") | [`Test                            |
    |                                   | RunnerSpec`](../../core/test/rule |
    |                                   | /TestRunnerSpec.html "class in co |
    |                                   | m.facebook.buck.core.test.rule"), |
    |                                   | which is basically a JSON         |
    |                                   | containing                        |
    |                                   | [`StringWithMacros`](../macro     |
    |                                   | s/StringWithMacros.html "class in |
    |                                   |  com.facebook.buck.rules.macros") |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [UnconfiguredBuildTar             | ::: block                         |
    | getTypeCoercer](UnconfiguredBuild | [`TypeCoercer`                    |
    | TargetTypeCoercer.html "class in  | ](TypeCoercer.html "interface in  |
    | com.facebook.buck.rules.coercer") | com.facebook.buck.rules.coercer") |
    |                                   | for                               |
    |                                   | [`UnconfiguredB                   |
    |                                   | uildTarget`](../../core/model/Unc |
    |                                   | onfiguredBuildTarget.html "class  |
    |                                   | in com.facebook.buck.core.model") |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Unconfigu                        | ::: block                         |
    | redBuildTargetWithOutputsTypeCoer | Coercer for                       |
    | cer](UnconfiguredBuildTargetWithO | [`UnconfiguredB                   |
    | utputsTypeCoercer.html "class in  | uildTarget`](../../core/model/Unc |
    | com.facebook.buck.rules.coercer") | onfiguredBuildTarget.html "class  |
    |                                   | in com.facebook.buck.core.model") |
    |                                   | instances that can optionally     |
    |                                   | have output labels.               |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Versi                            |                                   |
    | onMatchedCollection](VersionMatch |                                   |
    | edCollection.html "class in com.f |                                   |
    | acebook.buck.rules.coercer")\<T\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [VersionMatchedCollect            |                                   |
    | ion.Builder](VersionMatchedCollec |                                   |
    | tion.Builder.html "class in com.f |                                   |
    | acebook.buck.rules.coercer")\<T\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [VersionMatchedCollectionTyp      |                                   |
    | eCoercer](VersionMatchedCollectio |                                   |
    | nTypeCoercer.html "class in com.f |                                   |
    | acebook.buck.rules.coercer")\<T\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [Z                                | ::: block                         |
    | eroArgMacroTypeCoercer](ZeroArgMa | A coercer for                     |
    | croTypeCoercer.html "class in com | [`Macro`](..                      |
    | .facebook.buck.rules.coercer")\<M | /macros/Macro.html "interface in  |
    | extends                           | com.facebook.buck.rules.macros")s |
    | [Macro](../                       | which take zero arguments.        |
    | macros/Macro.html "interface in c | :::                               |
    | om.facebook.buck.rules.macros")\> |                                   |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Enum                              | Description                       |
    +===================================+===================================+
    | [BuildTargetMacroTypeCoercer.Tar  | ::: block                         |
    | getOrHost](BuildTargetMacroTypeCo | Should target be resolved for     |
    | ercer.TargetOrHost.html "enum in  | host platform or target           |
    | com.facebook.buck.rules.coercer") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [FrameworkPath.Type](             | ::: block                         |
    | FrameworkPath.Type.html "enum in  | The type of framework entry this  |
    | com.facebook.buck.rules.coercer") | object represents.                |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PathType                         |                                   |
    | Coercer.PathExistenceVerification |                                   |
    | Mode](PathTypeCoercer.PathExisten |                                   |
    | ceVerificationMode.html "enum in  |                                   |
    | com.facebook.buck.rules.coercer") |                                   |
    +-----------------------------------+-----------------------------------+
    | [SourceSet.Ty                     |                                   |
    | pe](SourceSet.Type.html "enum in  |                                   |
    | com.facebook.buck.rules.coercer") |                                   |
    +-----------------------------------+-----------------------------------+
    | [SourceSortedSet.Type](So         |                                   |
    | urceSortedSet.Type.html "enum in  |                                   |
    | com.facebook.buck.rules.coercer") |                                   |
    +-----------------------------------+-----------------------------------+
    | [SourceWithFlagsList.Type](Source |                                   |
    | WithFlagsList.Type.html "enum in  |                                   |
    | com.facebook.buck.rules.coercer") |                                   |
    +-----------------------------------+-----------------------------------+

    : Enum Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Exception                         | Description                       |
    +===================================+===================================+
    | [CoerceFailedException](Coer      |                                   |
    | ceFailedException.html "class in  |                                   |
    | com.facebook.buck.rules.coercer") |                                   |
    +-----------------------------------+-----------------------------------+
    | [DataTransferObjectDescriptor.Bu  | ::: block                         |
    | ilderBuildFailedException](DataTr | Checked exception thrown by       |
    | ansferObjectDescriptor.BuilderBui | [`DataTransferObjectDesc          |
    | ldFailedException.html "class in  | riptor.BuilderBuildFunction`](Dat |
    | com.facebook.buck.rules.coercer") | aTransferObjectDescriptor.Builder |
    |                                   | BuildFunction.html "interface in  |
    |                                   | com.facebook.buck.rules.coercer") |
    |                                   | when a user error (not internal   |
    |                                   | error) occurs.                    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ParamInfoException](P            | ::: block                         |
    | aramInfoException.html "class in  | Exception type thrown from        |
    | com.facebook.buck.rules.coercer") | \`ParamInfo\` methods.            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Exception Summary[ ]{.tabEnd}
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

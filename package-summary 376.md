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
# Package com.facebook.buck.rules.macros {#package-com.facebook.buck.rules.macros .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [CcFlagsMacro                     | ::: block                         |
    | ](CcFlagsMacro.html "interface in | `$(cflags)` macro type.           |
    |  com.facebook.buck.rules.macros") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Cc                               | ::: block                         |
    | Macro](CcMacro.html "interface in | `$(cc)` macro type.               |
    |  com.facebook.buck.rules.macros") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CxxFlagsMacro]                   | ::: block                         |
    | (CxxFlagsMacro.html "interface in | `$(cxxflags)` macro type.         |
    |  com.facebook.buck.rules.macros") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CxxM                             | ::: block                         |
    | acro](CxxMacro.html "interface in | `$(cxx)` macro type.              |
    |  com.facebook.buck.rules.macros") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [EnvM                             | ::: block                         |
    | acro](EnvMacro.html "interface in | `$(env)` macro type.              |
    |  com.facebook.buck.rules.macros") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Macro](Macro.html "interface in  | ::: block                         |
    |  com.facebook.buck.rules.macros") | Base class for strongly typed     |
    |                                   | macros.                           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [MacroExpander](MacroE            |                                   |
    | xpander.html "interface in com.fa |                                   |
    | cebook.buck.rules.macros")\<T,​P\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [PlatformNameMacro](Pla           | ::: block                         |
    | tformNameMacro.html "interface in | `$(platform-name)` macro type.    |
    |  com.facebook.buck.rules.macros") | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [AbsoluteOutputMacro](A           | ::: block                         |
    | bsoluteOutputMacro.html "class in | Macro used to denote the absolute |
    |  com.facebook.buck.rules.macros") | path of an output of a rule.      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Absol                            | ::: block                         |
    | uteOutputMacroExpander](AbsoluteO | Handles \'\$(abs_output \...)\'   |
    | utputMacroExpander.html "class in | macro which expands to the path   |
    |  com.facebook.buck.rules.macros") | of a named supplementary output.  |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AbstractExecutableTar            | ::: block                         |
    | getOrHostMacro](AbstractExecutabl | Marker for macros which expand to |
    | eTargetOrHostMacro.html "class in | executable.                       |
    |  com.facebook.buck.rules.macros") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AbstractLoca                     | ::: block                         |
    | tionMacroExpander](AbstractLocati | Expands to the path of a build    |
    | onMacroExpander.html "class in co | rules output.                     |
    | m.facebook.buck.rules.macros")\<T | :::                               |
    | extends                           |                                   |
    | [BaseLocationMacro](B             |                                   |
    | aseLocationMacro.html "class in c |                                   |
    | om.facebook.buck.rules.macros")\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [AbstractM                        |                                   |
    | acroExpanderWithoutPrecomputedWor |                                   |
    | k](AbstractMacroExpanderWithoutPr |                                   |
    | ecomputedWork.html "class in com. |                                   |
    | facebook.buck.rules.macros")\<T\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [ArgExpand                        | ::: block                         |
    | er](ArgExpander.html "class in co | Expands macros into fixed Arg .   |
    | m.facebook.buck.rules.macros")\<M | :::                               |
    | extends                           |                                   |
    | [                                 |                                   |
    | Macro](Macro.html "interface in c |                                   |
    | om.facebook.buck.rules.macros")\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [BaseLocationMacro]               | ::: block                         |
    | (BaseLocationMacro.html "class in | Macro that resolves to the output |
    |  com.facebook.buck.rules.macros") | location of a build rule.         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuildTargetMacro                 | ::: block                         |
    | ](BuildTargetMacro.html "class in | Base class for macros wrapping a  |
    |  com.facebook.buck.rules.macros") | single                            |
    |                                   | [`BuildTarget`](../../cor         |
    |                                   | e/model/BuildTarget.html "class i |
    |                                   | n com.facebook.buck.core.model"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Bu                               | ::: block                         |
    | ildTargetMacroExpander](BuildTarg | Abstract expander which resolves  |
    | etMacroExpander.html "class in co | using a references to another     |
    | m.facebook.buck.rules.macros")\<M | [`BuildRule`](../../core/         |
    | extends                           | rules/BuildRule.html "interface i |
    | [BuildTargetMacro](               | n com.facebook.buck.core.rules"). |
    | BuildTargetMacro.html "class in c | :::                               |
    | om.facebook.buck.rules.macros")\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [ClasspathAbiMacro]               |                                   |
    | (ClasspathAbiMacro.html "class in |                                   |
    |  com.facebook.buck.rules.macros") |                                   |
    +-----------------------------------+-----------------------------------+
    | [C                                | ::: block                         |
    | lasspathAbiMacroExpander](Classpa | Used to expand the macro          |
    | thAbiMacroExpander.html "class in | \$(classpath_abi //some:target)   |
    |  com.facebook.buck.rules.macros") | to the transitive abi\'s jars     |
    |                                   | path of that target, expanding    |
    |                                   | all paths to be absolute.         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ClasspathMac                     |                                   |
    | ro](ClasspathMacro.html "class in |                                   |
    |  com.facebook.buck.rules.macros") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ClasspathMacroExpander](Clas     | ::: block                         |
    | spathMacroExpander.html "class in | Used to expand the macro          |
    |  com.facebook.buck.rules.macros") | \$(classpath //some:target) to    |
    |                                   | the transitive classpath of that  |
    |                                   | target, expanding all paths to be |
    |                                   | absolute.                         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CppFlagsMa                       | ::: block                         |
    | cro](CppFlagsMacro.html "class in | `$(cppflags ...)` macro type.     |
    |  com.facebook.buck.rules.macros") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CxxGenruleFil                    | ::: block                         |
    | terAndTargetsMacro](CxxGenruleFil | Base class for `cxx_genrule`      |
    | terAndTargetsMacro.html "class in | flags-based macros.               |
    |  com.facebook.buck.rules.macros") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CxxppFlagsMacr                   | ::: block                         |
    | o](CxxppFlagsMacro.html "class in | `$(cxxppflags ...)` macro type.   |
    |  com.facebook.buck.rules.macros") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [EnvironmentVari                  | ::: block                         |
    | ableMacroExpander](EnvironmentVar | Expands \$(env XYZ) to use the    |
    | iableMacroExpander.html "class in | appropriate shell expansion for   |
    |  com.facebook.buck.rules.macros") | the current platform.             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ExecutableMacr                   |                                   |
    | o](ExecutableMacro.html "class in |                                   |
    |  com.facebook.buck.rules.macros") |                                   |
    +-----------------------------------+-----------------------------------+
    | [                                 | ::: block                         |
    | ExecutableMacroExpander](Executab | Resolves to the executable        |
    | leMacroExpander.html "class in co | command for a build target        |
    | m.facebook.buck.rules.macros")\<M | referencing a                     |
    | extends                           | [`BinaryBuildR                    |
    | [AbstractExecutableTarge          | ule`](../../core/rules/tool/Binar |
    | tOrHostMacro](AbstractExecutableT | yBuildRule.html "interface in com |
    | argetOrHostMacro.html "class in c | .facebook.buck.core.rules.tool"). |
    | om.facebook.buck.rules.macros")\> | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ExecutableTargetMacro](Exe       | ::: block                         |
    | cutableTargetMacro.html "class in | Like `exe` macro but does not     |
    |  com.facebook.buck.rules.macros") | switch to host platform           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [FunctionMacroReplacer](Function  | ::: block                         |
    | MacroReplacer.html "class in com. | A \@{link MacroReplacer} wrapping |
    | facebook.buck.rules.macros")\<T\> | a \@{link Function}.              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [LdflagsSharedFilterMacro](Ldflag | ::: block                         |
    | sSharedFilterMacro.html "class in | `$(ldflags-shared-filter ...)`    |
    |  com.facebook.buck.rules.macros") | macro type.                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [LdflagsSharedMacro](             | ::: block                         |
    | LdflagsSharedMacro.html "class in | `$(ldflags-shared ...)` macro     |
    |  com.facebook.buck.rules.macros") | type.                             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [LdflagsStaticFilterMacro](Ldflag | ::: block                         |
    | sStaticFilterMacro.html "class in | `$(ldflags-static-filter ...)`    |
    |  com.facebook.buck.rules.macros") | macro type.                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [LdflagsStaticMacro](             | ::: block                         |
    | LdflagsStaticMacro.html "class in | `$(ldflags-static ...)` macro     |
    |  com.facebook.buck.rules.macros") | type.                             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Ldfla                            | ::: block                         |
    | gsStaticPicFilterMacro](LdflagsSt | `                                 |
    | aticPicFilterMacro.html "class in | $(ldflags-static-pic-filter ...)` |
    |  com.facebook.buck.rules.macros") | macro type.                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [LdflagsStaticPicMacro](Ldf       | ::: block                         |
    | lagsStaticPicMacro.html "class in | `$(ldflags-static-pic ...)` macro |
    |  com.facebook.buck.rules.macros") | type.                             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [LdMacro](LdMacro.html "class in  | ::: block                         |
    |  com.facebook.buck.rules.macros") | `$(ld)` macro type.               |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [LocationMa                       | ::: block                         |
    | cro](LocationMacro.html "class in | Macro that resolves to the output |
    |  com.facebook.buck.rules.macros") | location of a build rule.         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [LocationMacroExpander](Loc       | ::: block                         |
    | ationMacroExpander.html "class in | Expands to the path of a build    |
    |  com.facebook.buck.rules.macros") | rules output.                     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [LocationPlatformMacro](Loc       | ::: block                         |
    | ationPlatformMacro.html "class in | Macro that resolves to the output |
    |  com.facebook.buck.rules.macros") | location of a build rule.         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [LocationP                        | ::: block                         |
    | latformMacroExpander](LocationPla | Expands to the path of a build    |
    | tformMacroExpander.html "class in | rules output.                     |
    |  com.facebook.buck.rules.macros") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [MacroContain                     | ::: block                         |
    | er](MacroContainer.html "class in | Packages up a                     |
    |  com.facebook.buck.rules.macros") | [                                 |
    |                                   | `Macro`](Macro.html "interface in |
    |                                   |  com.facebook.buck.rules.macros") |
    |                                   | along some configuration.         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [MacroContainer.Builder](Macr     |                                   |
    | oContainer.Builder.html "class in |                                   |
    |  com.facebook.buck.rules.macros") |                                   |
    +-----------------------------------+-----------------------------------+
    | [MavenCoordinatesMacro](Mav       |                                   |
    | enCoordinatesMacro.html "class in |                                   |
    |  com.facebook.buck.rules.macros") |                                   |
    +-----------------------------------+-----------------------------------+
    | [MavenCoor                        | ::: block                         |
    | dinatesMacroExpander](MavenCoordi | Resolves to the maven coordinates |
    | natesMacroExpander.html "class in | for a build target referencing a  |
    |  com.facebook.buck.rules.macros") | [`HasMav                          |
    |                                   | enCoordinates`](../../jvm/core/Ha |
    |                                   | sMavenCoordinates.html "interface |
    |                                   |  in com.facebook.buck.jvm.core"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Output                           | ::: block                         |
    | Macro](OutputMacro.html "class in | Macro used to denote the path of  |
    |  com.facebook.buck.rules.macros") | an output of a rule.              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [OutputMacroExpander](O           | ::: block                         |
    | utputMacroExpander.html "class in | Handles \'\$(output \...)\' macro |
    |  com.facebook.buck.rules.macros") | which expands to the path of a    |
    |                                   | named supplementary output.       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Quer                             | ::: block                         |
    | yMacro](QueryMacro.html "class in | Base class for macros that embed  |
    |  com.facebook.buck.rules.macros") | a query string.                   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [QueryMacroExpander](Que          | ::: block                         |
    | ryMacroExpander.html "class in co | Abstract base class for the       |
    | m.facebook.buck.rules.macros")\<T | query_targets and query_outputs   |
    | extends                           | macros                            |
    | [QueryM                           | :::                               |
    | acro](QueryMacro.html "class in c |                                   |
    | om.facebook.buck.rules.macros")\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [QueryMacroExp                    |                                   |
    | ander.QueryResults](QueryMacroExp |                                   |
    | ander.QueryResults.html "class in |                                   |
    |  com.facebook.buck.rules.macros") |                                   |
    +-----------------------------------+-----------------------------------+
    | [QueryOutputsMacro]               | ::: block                         |
    | (QueryOutputsMacro.html "class in | Class providing the type for      |
    |  com.facebook.buck.rules.macros") | macros used in \`\$(query_outputs |
    |                                   | \...)\` macro strings.            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Q                                | ::: block                         |
    | ueryOutputsMacroExpander](QueryOu | Used to expand the macro          |
    | tputsMacroExpander.html "class in | \$(query_outputs                  |
    |  com.facebook.buck.rules.macros") | \"some(query(:expression))\") to  |
    |                                   | the set of the outputs of the     |
    |                                   | targets matching the query.       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [QueryPathsMacr                   | ::: block                         |
    | o](QueryPathsMacro.html "class in | Class providing the type for      |
    |  com.facebook.buck.rules.macros") | macros used in \`\$(query_paths   |
    |                                   | \...)\` macro strings.            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [QueryPathsMacroExpander](Query   |                                   |
    | PathsMacroExpander.html "class in |                                   |
    |  com.facebook.buck.rules.macros") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Query                            | ::: block                         |
    | TargetsAndOutputsMacro](QueryTarg | Class providing the type for      |
    | etsAndOutputsMacro.html "class in | macros used in                    |
    |  com.facebook.buck.rules.macros") | \`\$(query_targets_and_outputs    |
    |                                   | \...)\` macro strings.            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [QueryTargetsAndOutput            | ::: block                         |
    | sMacroExpander](QueryTargetsAndOu | Used to expand the macro          |
    | tputsMacroExpander.html "class in | \$(query_targets_and_outputs      |
    |  com.facebook.buck.rules.macros") | \"some(query(:expression))\") to  |
    |                                   | the full target names and the set |
    |                                   | of the outputs of the targets     |
    |                                   | matching the query separated by a |
    |                                   | space.                            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [QueryTargetsMacro]               | ::: block                         |
    | (QueryTargetsMacro.html "class in | Class providing the type for      |
    |  com.facebook.buck.rules.macros") | macros used in \`\$(query_targets |
    |                                   | \...)\` macro strings.            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Q                                | ::: block                         |
    | ueryTargetsMacroExpander](QueryTa | Used to expand the macro          |
    | rgetsMacroExpander.html "class in | \$(query_targets                  |
    |  com.facebook.buck.rules.macros") | \"some(query(:expression))\") to  |
    |                                   | the set of targets matching the   |
    |                                   | query.                            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [SimpleMacroExpander](Simp        | ::: block                         |
    | leMacroExpander.html "class in co | A macro expander with no inputs   |
    | m.facebook.buck.rules.macros")\<M | or precomputed work               |
    | extends                           | :::                               |
    | [                                 |                                   |
    | Macro](Macro.html "interface in c |                                   |
    | om.facebook.buck.rules.macros")\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [StringExpander]                  | ::: block                         |
    | (StringExpander.html "class in co | Expands macros into fixed         |
    | m.facebook.buck.rules.macros")\<M | strings.                          |
    | extends                           | :::                               |
    | [                                 |                                   |
    | Macro](Macro.html "interface in c |                                   |
    | om.facebook.buck.rules.macros")\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [StringWithMacros                 | ::: block                         |
    | ](StringWithMacros.html "class in | A class representing a string     |
    |  com.facebook.buck.rules.macros") | containing ordered, embedded,     |
    |                                   | strongly typed macros.            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [S                                | ::: block                         |
    | tringWithMacrosConverter](StringW | Converts a                        |
    | ithMacrosConverter.html "class in | [`StringWithMacros`               |
    |  com.facebook.buck.rules.macros") | ](StringWithMacros.html "class in |
    |                                   |  com.facebook.buck.rules.macros") |
    |                                   | into an                           |
    |                                   | [`Ar                              |
    |                                   | g`](../args/Arg.html "interface i |
    |                                   | n com.facebook.buck.rules.args"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Worker                           | ::: block                         |
    | Macro](WorkerMacro.html "class in | Type for the \`\$(worker \...)\`  |
    |  com.facebook.buck.rules.macros") | macro.                            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [WorkerMacroA                     | ::: block                         |
    | rg](WorkerMacroArg.html "class in | Worker macro wrapper which        |
    |  com.facebook.buck.rules.macros") | extracts/verifies details from    |
    |                                   | the an underlying                 |
    |                                   | [`WorkerTool`](..                 |
    |                                   | /../shell/WorkerTool.html "interf |
    |                                   | ace in com.facebook.buck.shell"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [WorkerMacroExpander](W           | ::: block                         |
    | orkerMacroExpander.html "class in | Macro expander for the            |
    |  com.facebook.buck.rules.macros") | \`\$(worker \...)\` macro.        |
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

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
[Package]{.packageLabelInType} [com.facebook.buck.cxx](package-summary.html)
:::

## Class CxxSymlinkTreeHeaders {#class-cxxsymlinktreeheaders .title title="Class CxxSymlinkTreeHeaders"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.cxx.CxxHeaders](CxxHeaders.html "class in com.facebook.buck.cxx")

    -   -   com.facebook.buck.cxx.CxxSymlinkTreeHeaders

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`, `HasCustomDepsLogic`, `RuleKeyAppendable`

    ------------------------------------------------------------------------

        public abstract class CxxSymlinkTreeHeaders
        extends CxxHeaders
        implements RuleKeyAppendable

    ::: block
    Encapsulates headers modeled using a
    [`HeaderSymlinkTree`](toolchain/HeaderSymlinkTree.html "class in com.facebook.buck.cxx.toolchain").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.rules.keys.RuleKeyAppendable}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.rules.keys.[RuleKeyAppendable](../rules/keys/RuleKeyAppendable.html "interface in com.facebook.buck.rules.keys")

            `RuleKeyAppendable.RuleKeyAppendableSink`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                 Description
          --------------------------- -------------
          `CxxSymlinkTreeHeaders()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `ad                   | ::: block             |
        |                       | dToHeaderPathNormaliz | Add this header pack  |
        |                       | er​(com.facebook.buck. | to the given          |
        |                       | cxx.HeaderPathNormali | `HeaderPat            |
        |                       | zer.Builder builder)` | hNormalizer.Builder`. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `appendToRuleKey​(Rule | ::: block             |
        |                       | KeyAppendable.RuleKey | Deprecated.           |
        |                       | AppendableSink sink)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static C             | `                     |                       |
        | xxSymlinkTreeHeaders` | from​(HeaderSymlinkTre |                       |
        |                       | e symlinkTree,     Cx |                       |
        |                       | xPreprocessables.Incl |                       |
        |                       | udeType includeType)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `java.util.stre       | `getDeps​(SourcePathRu |                       |
        | am.Stream<BuildRule>` | leFinder ruleFinder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract             | `getHeaderMap()`      |                       |
        | Optional<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `a                    | `getIncludeRoot()`    |                       |
        | bstract Either<PathSo |                       |                       |
        | urcePath,​SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract CxxPreproc  | `getIncludeType()`    |                       |
        | essables.IncludeType` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract             | `getNameToPathMap()`  |                       |
        |  com.google.common.co |                       |                       |
        | llect.ImmutableSorted |                       |                       |
        | Map<Path,​SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Path>`      | `getResolvedInclud    |                       |
        |                       | eRoot​(SourcePathResol |                       |
        |                       | verAdapter resolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract SourcePath` | `getRoot()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract String`     | `g                    |                       |
        |                       | etSymlinkTreeClass()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static C             | `of​(CxxPreproc        |                       |
        | xxSymlinkTreeHeaders` | essables.IncludeType  |                       |
        |                       | includeType,   Source |                       |
        |                       | Path root,   Either<P |                       |
        |                       | athSourcePath,​SourceP |                       |
        |                       | ath> includeRoot,   O |                       |
        |                       | ptional<? extends Sou |                       |
        |                       | rcePath> headerMap,   |                       |
        |                       |  com.google.common.co |                       |
        |                       | llect.ImmutableSorted |                       |
        |                       | Map<Path,​SourcePath>  |                       |
        |                       | nameToPathMap,   Stri |                       |
        |                       | ng symlinkTreeClass)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.cxx.CxxHeaders}

            ### Methods inherited from class com.facebook.buck.cxx.[CxxHeaders](CxxHeaders.html "class in com.facebook.buck.cxx")

            `getArgs`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### CxxSymlinkTreeHeaders

                public CxxSymlinkTreeHeaders()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getIncludeType()}

        -   #### getIncludeType

            ``` methodSignature
            public abstract CxxPreprocessables.IncludeType getIncludeType()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getIncludeType` in class `CxxHeaders`

        []{#getRoot()}

        -   #### getRoot

            ``` methodSignature
            public abstract SourcePath getRoot()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRoot` in class `CxxHeaders`

            [Returns:]{.returnLabel}
            :   the root of the includes.

        []{#getIncludeRoot()}

        -   #### getIncludeRoot

            ``` methodSignature
            public abstract Either<PathSourcePath,​SourcePath> getIncludeRoot()
            ```

            [Returns:]{.returnLabel}
            :   the path to add to the preprocessor search path to find
                the includes. This defaults to the root, but can be
                overridden to use an alternate path.

        []{#getResolvedIncludeRoot(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### getResolvedIncludeRoot

            ``` methodSignature
            public Optional<Path> getResolvedIncludeRoot​(SourcePathResolverAdapter resolver)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `getResolvedIncludeRoot` in class `CxxHeaders`

            [Returns:]{.returnLabel}
            :   the path to add to the preprocessor search path to find
                the includes. This defaults to the root, but can be
                overridden to use an alternate path.

        []{#getHeaderMap()}

        -   #### getHeaderMap

            ``` methodSignature
            public abstract Optional<SourcePath> getHeaderMap()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getHeaderMap` in class `CxxHeaders`

            [Returns:]{.returnLabel}
            :   the path to the optional header map to use for this
                header pack.

        []{#getNameToPathMap()}

        -   #### getNameToPathMap

            ``` methodSignature
            @Auxiliary
            public abstract com.google.common.collect.ImmutableSortedMap<Path,​SourcePath> getNameToPathMap()
            ```

        []{#addToHeaderPathNormalizer(com.facebook.buck.cxx.HeaderPathNormalizer.Builder)}

        -   #### addToHeaderPathNormalizer

            ``` methodSignature
            public void addToHeaderPathNormalizer​(com.facebook.buck.cxx.HeaderPathNormalizer.Builder builder)
            ```

            ::: block
            [Description copied from
            class: `CxxHeaders`]{.descfrmTypeLabel}
            :::

            ::: block
            Add this header pack to the given
            `HeaderPathNormalizer.Builder`.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `addToHeaderPathNormalizer` in class `CxxHeaders`

        []{#getSymlinkTreeClass()}

        -   #### getSymlinkTreeClass

            ``` methodSignature
            public abstract String getSymlinkTreeClass()
            ```

        []{#getDeps(com.facebook.buck.core.rules.SourcePathRuleFinder)}

        -   #### getDeps

            ``` methodSignature
            public java.util.stream.Stream<BuildRule> getDeps​(SourcePathRuleFinder ruleFinder)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDeps` in interface `HasCustomDepsLogic`

            [Overrides:]{.overrideSpecifyLabel}
            :   `getDeps` in class `CxxHeaders`

            [Returns:]{.returnLabel}
            :   all deps required by this header pack.

        []{#appendToRuleKey(com.facebook.buck.rules.keys.RuleKeyAppendable.RuleKeyAppendableSink)}

        -   #### appendToRuleKey

            ``` methodSignature
            public void appendToRuleKey​(RuleKeyAppendable.RuleKeyAppendableSink sink)
            ```

            ::: block
            [Description copied from
            interface: `RuleKeyAppendable`]{.descfrmTypeLabel}
            :::

            ::: block
            Deprecated. Add additional custom things to the rulekey
            builder.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `appendToRuleKey` in interface `RuleKeyAppendable`

        []{#from(com.facebook.buck.cxx.toolchain.HeaderSymlinkTree,com.facebook.buck.cxx.CxxPreprocessables.IncludeType)}

        -   #### from

            ``` methodSignature
            public static CxxSymlinkTreeHeaders from​(HeaderSymlinkTree symlinkTree,
                                                     CxxPreprocessables.IncludeType includeType)
            ```

            [Returns:]{.returnLabel}
            :   a
                [`CxxHeaders`](CxxHeaders.html "class in com.facebook.buck.cxx")
                constructed from the given
                [`HeaderSymlinkTree`](toolchain/HeaderSymlinkTree.html "class in com.facebook.buck.cxx.toolchain").

        []{#of(com.facebook.buck.cxx.CxxPreprocessables.IncludeType,com.facebook.buck.core.sourcepath.SourcePath,com.facebook.buck.util.types.Either,java.util.Optional,com.google.common.collect.ImmutableSortedMap,java.lang.String)}

        -   #### of

            ``` methodSignature
            public static CxxSymlinkTreeHeaders of​(CxxPreprocessables.IncludeType includeType,
                                                   SourcePath root,
                                                   Either<PathSourcePath,​SourcePath> includeRoot,
                                                   Optional<? extends SourcePath> headerMap,
                                                   com.google.common.collect.ImmutableSortedMap<Path,​SourcePath> nameToPathMap,
                                                   String symlinkTreeClass)
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

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
-   Nested \| 
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

## Class CxxHeaders {#class-cxxheaders .title title="Class CxxHeaders"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.CxxHeaders

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`, `HasCustomDepsLogic`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `CxxHeadersDir`, `CxxRawHeaders`, `CxxSymlinkTreeHeaders`

    ------------------------------------------------------------------------

        public abstract class CxxHeaders
        extends Object
        implements AddsToRuleKey, HasCustomDepsLogic

    ::: block
    Encapsulates headers from a single root location.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor      Description
          ---------------- -------------
          `CxxHeaders()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `abstract void`       | `ad                   | ::: block             |
        |                       | dToHeaderPathNormaliz | Add this header pack  |
        |                       | er​(com.facebook.buck. | to the given          |
        |                       | cxx.HeaderPathNormali | `HeaderPat            |
        |                       | zer.Builder builder)` | hNormalizer.Builder`. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `getArgs​(Iterable<Cx  |                       |
        | tic Iterable<String>` | xHeaders> cxxHeaderse |                       |
        |                       | s,        SourcePathR |                       |
        |                       | esolverAdapter resolv |                       |
        |                       | er,        Optional<P |                       |
        |                       | athShortener> pathMin |                       |
        |                       | imizer,        Prepro |                       |
        |                       | cessor preprocessor)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `java.util.stre       | `getDeps​(SourcePathRu |                       |
        | am.Stream<BuildRule>` | leFinder ruleFinder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract             | `getHeaderMap()`      |                       |
        | Optional<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract CxxPreproc  | `getIncludeType()`    |                       |
        | essables.IncludeType` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Path>`      | `getResolvedInclud    |                       |
        |                       | eRoot​(SourcePathResol |                       |
        |                       | verAdapter resolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract SourcePath` | `getRoot()`           |                       |
        +-----------------------+-----------------------+-----------------------+

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

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### CxxHeaders

                public CxxHeaders()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getIncludeType()}

        -   #### getIncludeType

            ``` methodSignature
            public abstract CxxPreprocessables.IncludeType getIncludeType()
            ```

        []{#getRoot()}

        -   #### getRoot

            ``` methodSignature
            @Nullable
            public abstract SourcePath getRoot()
            ```

            [Returns:]{.returnLabel}
            :   the root of the includes.

        []{#getHeaderMap()}

        -   #### getHeaderMap

            ``` methodSignature
            public abstract Optional<SourcePath> getHeaderMap()
            ```

            [Returns:]{.returnLabel}
            :   the path to the optional header map to use for this
                header pack.

        []{#addToHeaderPathNormalizer(com.facebook.buck.cxx.HeaderPathNormalizer.Builder)}

        -   #### addToHeaderPathNormalizer

            ``` methodSignature
            public abstract void addToHeaderPathNormalizer​(com.facebook.buck.cxx.HeaderPathNormalizer.Builder builder)
            ```

            ::: block
            Add this header pack to the given
            `HeaderPathNormalizer.Builder`.
            :::

        []{#getDeps(com.facebook.buck.core.rules.SourcePathRuleFinder)}

        -   #### getDeps

            ``` methodSignature
            public java.util.stream.Stream<BuildRule> getDeps​(SourcePathRuleFinder ruleFinder)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDeps` in interface `HasCustomDepsLogic`

            [Returns:]{.returnLabel}
            :   all deps required by this header pack.

        []{#getResolvedIncludeRoot(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### getResolvedIncludeRoot

            ``` methodSignature
            public Optional<Path> getResolvedIncludeRoot​(SourcePathResolverAdapter resolver)
            ```

            [Returns:]{.returnLabel}
            :   the path to add to the preprocessor search path to find
                the includes. This defaults to the root, but can be
                overridden to use an alternate path.

        []{#getArgs(java.lang.Iterable,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,java.util.Optional,com.facebook.buck.cxx.toolchain.Preprocessor)}

        -   #### getArgs

            ``` methodSignature
            public static Iterable<String> getArgs​(Iterable<CxxHeaders> cxxHeaderses,
                                                   SourcePathResolverAdapter resolver,
                                                   Optional<PathShortener> pathMinimizer,
                                                   Preprocessor preprocessor)
            ```

            [Returns:]{.returnLabel}
            :   the arguments to add to the preprocessor command line to
                include the given header packs in preprocessor search
                path.
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
-   Nested \| 
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

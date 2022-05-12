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

## Class CxxRawHeaders {#class-cxxrawheaders .title title="Class CxxRawHeaders"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.cxx.CxxHeaders](CxxHeaders.html "class in com.facebook.buck.cxx")

    -   -   com.facebook.buck.cxx.CxxRawHeaders

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`, `HasCustomDepsLogic`

    ------------------------------------------------------------------------

        public abstract class CxxRawHeaders
        extends CxxHeaders
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor         Description
          ------------------- -------------
          `CxxRawHeaders()`    

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
        | `                     | `getHeaderMap()`      |                       |
        | Optional<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPreproc           | `getIncludeType()`    |                       |
        | essables.IncludeType` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Path>`      | `getResolvedInclud    |                       |
        |                       | eRoot​(SourcePathResol |                       |
        |                       | verAdapter resolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `getRoot()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `of​(com               |                       |
        | static CxxRawHeaders` | .google.common.collec |                       |
        |                       | t.ImmutableSortedSet< |                       |
        |                       | SourcePath> headers)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.cxx.CxxHeaders}

            ### Methods inherited from class com.facebook.buck.cxx.[CxxHeaders](CxxHeaders.html "class in com.facebook.buck.cxx")

            `getArgs, getDeps`

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

        -   #### CxxRawHeaders

                public CxxRawHeaders()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getIncludeType()}

        -   #### getIncludeType

            ``` methodSignature
            public final CxxPreprocessables.IncludeType getIncludeType()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getIncludeType` in class `CxxHeaders`

        []{#getRoot()}

        -   #### getRoot

            ``` methodSignature
            @Nullable
            public SourcePath getRoot()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRoot` in class `CxxHeaders`

            [Returns:]{.returnLabel}
            :   the root of the includes.

        []{#getHeaderMap()}

        -   #### getHeaderMap

            ``` methodSignature
            public Optional<SourcePath> getHeaderMap()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getHeaderMap` in class `CxxHeaders`

            [Returns:]{.returnLabel}
            :   the path to the optional header map to use for this
                header pack.

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

        []{#of(com.google.common.collect.ImmutableSortedSet)}

        -   #### of

            ``` methodSignature
            public static CxxRawHeaders of​(com.google.common.collect.ImmutableSortedSet<SourcePath> headers)
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

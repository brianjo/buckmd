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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.parser.buildtargetparser](package-summary.html)
:::

## Class BuildTargetMatcherParser\<T\> {#class-buildtargetmatcherparsert .title title="Class BuildTargetMatcherParser"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.parser.buildtargetparser.BuildTargetMatcherParser\<T\>

::: description
-   

    Direct Known Subclasses:
    :   `BuildTargetMatcherTargetNodeParser`

    ------------------------------------------------------------------------

        public abstract class BuildTargetMatcherParser<T>
        extends Object

    ::: block
    Context for parsing build target names. Fully-qualified target names
    are parsed the same regardless of the context.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                    Description
          ------------------------------ -------------
          `BuildTargetMatcherParser()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `                     | `createForCh          |                       |
        | protected abstract T` | ildren​(CellRelativePa |                       |
        |                       | th cellRelativePath)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `createForDesce       |                       |
        | protected abstract T` | ndants​(CellRelativePa |                       |
        |                       | th cellRelativePath)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `createForS           |                       |
        | protected abstract T` | ingleton​(Unconfigured |                       |
        |                       | BuildTargetWithOutput |                       |
        |                       | s targetWithOutputs)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Bui           | `for                  | ::: block             |
        | ldTargetMatcherParser | VisibilityArgument()` | Used when parsing     |
        | <BuildTargetMatcher>` |                       | target names in the   |
        |                       |                       | `visibility` argument |
        |                       |                       | to a build rule.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `T`                   | `parse​(Stri           | ::: block             |
        |                       | ng buildTargetPattern | Matches the given     |
        |                       | ,      CellNameResolv | `buildTargetPattern`  |
        |                       | er cellNameResolver)` | according to the      |
        |                       |                       | following rules:      |
        |                       |                       | //src/com/            |
        |                       |                       | facebook/buck/cli:cli |
        |                       |                       | will be converted to  |
        |                       |                       | a single build        |
        |                       |                       | target;               |
        |                       |                       | //src/c               |
        |                       |                       | om/facebook/buck/cli: |
        |                       |                       | will match all in the |
        |                       |                       | same directory;       |
        |                       |                       | //src/com/f           |
        |                       |                       | acebook/buck/cli/\... |
        |                       |                       | :::                   |
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

        -   #### BuildTargetMatcherParser

                public BuildTargetMatcherParser()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#parse(java.lang.String,com.facebook.buck.core.cell.nameresolver.CellNameResolver)}

        -   #### parse

            ``` methodSignature
            public final T parse​(String buildTargetPattern,
                                 CellNameResolver cellNameResolver)
            ```

            ::: block
            Matches the given `buildTargetPattern` according to the
            following rules:
            -   //src/com/facebook/buck/cli:cli will be converted to a
                single build target;
            -   //src/com/facebook/buck/cli: will match all in the same
                directory;
            -   //src/com/facebook/buck/cli/\... will match all in or
                under that directory.

            For cases 2 and 3, parseContext is expected to be
            [`forVisibilityArgument()`](#forVisibilityArgument()).
            :::

        []{#forVisibilityArgument()}

        -   #### forVisibilityArgument

            ``` methodSignature
            public static BuildTargetMatcherParser<BuildTargetMatcher> forVisibilityArgument()
            ```

            ::: block
            Used when parsing target names in the `visibility` argument
            to a build rule.
            :::

        []{#createForDescendants(com.facebook.buck.core.model.CellRelativePath)}

        -   #### createForDescendants

            ``` methodSignature
            protected abstract T createForDescendants​(CellRelativePath cellRelativePath)
            ```

            [Returns:]{.returnLabel}
            :   description of the target name and context being parsed
                when an error was encountered. Examples are \":azzetz in
                build file //first-party/orca/orcaapp/BUCK\" and
                \"//first-party/orca/orcaapp:mezzenger in context
                FULLY_QUALIFIED\"

        []{#createForChildren(com.facebook.buck.core.model.CellRelativePath)}

        -   #### createForChildren

            ``` methodSignature
            protected abstract T createForChildren​(CellRelativePath cellRelativePath)
            ```

        []{#createForSingleton(com.facebook.buck.core.model.UnconfiguredBuildTargetWithOutputs)}

        -   #### createForSingleton

            ``` methodSignature
            protected abstract T createForSingleton​(UnconfiguredBuildTargetWithOutputs targetWithOutputs)
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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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

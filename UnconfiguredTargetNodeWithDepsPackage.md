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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.model.targetgraph.raw](package-summary.html)
:::

## Class UnconfiguredTargetNodeWithDepsPackage {#class-unconfiguredtargetnodewithdepspackage .title title="Class UnconfiguredTargetNodeWithDepsPackage"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.model.targetgraph.raw.UnconfiguredTargetNodeWithDepsPackage

::: description
-   

    All Implemented Interfaces:
    :   `ComputeResult`

    ------------------------------------------------------------------------

        public abstract class UnconfiguredTargetNodeWithDepsPackage
        extends Object
        implements ComputeResult

    ::: block
    Represents all
    [`UnconfiguredTargetNodeWithDeps`](UnconfiguredTargetNodeWithDeps.html "class in com.facebook.buck.core.model.targetgraph.raw")
    that result from parsing a single build file
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                 Description
          ------------------------------------------- -------------
          `UnconfiguredTargetNodeWithDepsPackage()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `                     | `getErrors()`         | ::: block             |
        | abstract com.google.c |                       | Errors that occurred  |
        | ommon.collect.Immutab |                       | parsing this package. |
        | leList<ParsingError>` |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract com         | `getIncludes()`       | ::: block             |
        | .google.common.collec |                       | Set of extension      |
        | t.ImmutableSet<Path>` |                       | files read during     |
        |                       |                       | parsing.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Path`       | `getPackagePath()`    | ::: block             |
        |                       |                       | Package path,         |
        |                       |                       | relative to parse     |
        |                       |                       | root, usually cell    |
        |                       |                       | root                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abs                  | `getUnconfiguredT     | ::: block             |
        | tract com.google.comm | argetNodesWithDeps()` | All                   |
        | on.collect.ImmutableM |                       | [                     |
        | ap<String,​Unconfigure |                       | `UnconfiguredTargetNo |
        | dTargetNodeWithDeps>` |                       | deWithDeps`](Unconfig |
        |                       |                       | uredTargetNodeWithDep |
        |                       |                       | s.html "class in com. |
        |                       |                       | facebook.buck.core.mo |
        |                       |                       | del.targetgraph.raw") |
        |                       |                       | which comes from the  |
        |                       |                       | same build package,   |
        |                       |                       | i.e.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `of​(                  |                       |
        | tic UnconfiguredTarge | Path packagePath,   c |                       |
        | tNodeWithDepsPackage` | om.google.common.coll |                       |
        |                       | ect.ImmutableMap<Stri |                       |
        |                       | ng,​UnconfiguredTarget |                       |
        |                       | NodeWithDeps> unconfi |                       |
        |                       | guredTargetNodesWithD |                       |
        |                       | eps,   com.google.com |                       |
        |                       | mon.collect.Immutable |                       |
        |                       | List<ParsingError> er |                       |
        |                       | rors,   com.google.co |                       |
        |                       | mmon.collect.Immutabl |                       |
        |                       | eSet<Path> includes)` |                       |
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

        -   #### UnconfiguredTargetNodeWithDepsPackage

                public UnconfiguredTargetNodeWithDepsPackage()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getPackagePath()}

        -   #### getPackagePath

            ``` methodSignature
            public abstract Path getPackagePath()
            ```

            ::: block
            Package path, relative to parse root, usually cell root
            :::

        []{#getUnconfiguredTargetNodesWithDeps()}

        -   #### getUnconfiguredTargetNodesWithDeps

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableMap<String,​UnconfiguredTargetNodeWithDeps> getUnconfiguredTargetNodesWithDeps()
            ```

            ::: block
            All
            [`UnconfiguredTargetNodeWithDeps`](UnconfiguredTargetNodeWithDeps.html "class in com.facebook.buck.core.model.targetgraph.raw")
            which comes from the same build package, i.e. result from
            parsing a single build file. Key is a string representing
            short build target name (last part of the name after the
            colon) and value is corresponding target.
            :::

        []{#getErrors()}

        -   #### getErrors

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<ParsingError> getErrors()
            ```

            ::: block
            Errors that occurred parsing this package. If errors exist,
            package may be incomplete, i.e. some or all target nodes may
            be missing
            :::

        []{#getIncludes()}

        -   #### getIncludes

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSet<Path> getIncludes()
            ```

            ::: block
            Set of extension files read during parsing.
            :::

        []{#of(java.nio.file.Path,com.google.common.collect.ImmutableMap,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableSet)}

        -   #### of

            ``` methodSignature
            public static UnconfiguredTargetNodeWithDepsPackage of​(Path packagePath,
                                                                   com.google.common.collect.ImmutableMap<String,​UnconfiguredTargetNodeWithDeps> unconfiguredTargetNodesWithDeps,
                                                                   com.google.common.collect.ImmutableList<ParsingError> errors,
                                                                   com.google.common.collect.ImmutableSet<Path> includes)
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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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

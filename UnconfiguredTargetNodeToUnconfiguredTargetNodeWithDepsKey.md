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
-   [Package](package-summary.html)
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

<div>

-   Summary: 
-   Nested \| 
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.parser.targetnode](package-summary.html)
:::

## Class UnconfiguredTargetNodeToUnconfiguredTargetNodeWithDepsKey {#class-unconfiguredtargetnodetounconfiguredtargetnodewithdepskey .title title="Class UnconfiguredTargetNodeToUnconfiguredTargetNodeWithDepsKey"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.parser.targetnode.UnconfiguredTargetNodeToUnconfiguredTargetNodeWithDepsKey

::: description
-   

    All Implemented Interfaces:
    :   `ComputeKey<UnconfiguredTargetNodeWithDeps>`

    ------------------------------------------------------------------------

        public abstract class UnconfiguredTargetNodeToUnconfiguredTargetNodeWithDepsKey
        extends Object
        implements ComputeKey<UnconfiguredTargetNodeWithDeps>

    ::: block
    Transformation key containing
    [`UnconfiguredTargetNode`](../../core/model/targetgraph/raw/UnconfiguredTargetNode.html "interface in com.facebook.buck.core.model.targetgraph.raw")
    to translate it to
    [`UnconfiguredTargetNodeWithDeps`](../../core/model/targetgraph/raw/UnconfiguredTargetNodeWithDeps.html "class in com.facebook.buck.core.model.targetgraph.raw").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                                                Field          Description
          ---------------------------------------------------------------- -------------- -------------
          `static ComputationIdentifier<UnconfiguredTargetNodeWithDeps>`   `IDENTIFIER`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                     Description
          --------------------------------------------------------------- -------------
          `UnconfiguredTargetNodeToUnconfiguredTargetNodeWithDepsKey()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `protected void`      | `check()`             |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ComputationI         | `getIdentifier()`     |                       |
        | dentifier<Unconfigure |                       |                       |
        | dTargetNodeWithDeps>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Path`       | `getPackagePath()`    | ::: block             |
        |                       |                       | [`Path`](http://do    |
        |                       |                       | cs.oracle.com/javase/ |
        |                       |                       | 7/docs/api/java/nio/f |
        |                       |                       | ile/Path.html?is-exte |
        |                       |                       | rnal=true "class or i |
        |                       |                       | nterface in java.nio. |
        |                       |                       | file"){.externalLink} |
        |                       |                       | to the root of a      |
        |                       |                       | package that has this |
        |                       |                       | [`                    |
        |                       |                       | UnconfiguredTargetNod |
        |                       |                       | e`](../../core/model/ |
        |                       |                       | targetgraph/raw/Uncon |
        |                       |                       | figuredTargetNode.htm |
        |                       |                       | l "interface in com.f |
        |                       |                       | acebook.buck.core.mod |
        |                       |                       | el.targetgraph.raw"), |
        |                       |                       | relative to parse     |
        |                       |                       | root, usually cell    |
        |                       |                       | root                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Un          | `getUnco              | ::: block             |
        | configuredTargetNode` | nfiguredTargetNode()` | [                     |
        |                       |                       | `UnconfiguredTargetNo |
        |                       |                       | de`](../../core/model |
        |                       |                       | /targetgraph/raw/Unco |
        |                       |                       | nfiguredTargetNode.ht |
        |                       |                       | ml "interface in com. |
        |                       |                       | facebook.buck.core.mo |
        |                       |                       | del.targetgraph.raw") |
        |                       |                       | which should be       |
        |                       |                       | translated to         |
        |                       |                       | [`Unconfigure         |
        |                       |                       | dTargetNodeWithDeps`] |
        |                       |                       | (../../core/model/tar |
        |                       |                       | getgraph/raw/Unconfig |
        |                       |                       | uredTargetNodeWithDep |
        |                       |                       | s.html "class in com. |
        |                       |                       | facebook.buck.core.mo |
        |                       |                       | del.targetgraph.raw") |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
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
    -   []{#field.detail}

        ### Field Detail

        []{#IDENTIFIER}

        -   #### IDENTIFIER

                public static final ComputationIdentifier<UnconfiguredTargetNodeWithDeps> IDENTIFIER
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### UnconfiguredTargetNodeToUnconfiguredTargetNodeWithDepsKey

                public UnconfiguredTargetNodeToUnconfiguredTargetNodeWithDepsKey()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getUnconfiguredTargetNode()}

        -   #### getUnconfiguredTargetNode

            ``` methodSignature
            public abstract UnconfiguredTargetNode getUnconfiguredTargetNode()
            ```

            ::: block
            [`UnconfiguredTargetNode`](../../core/model/targetgraph/raw/UnconfiguredTargetNode.html "interface in com.facebook.buck.core.model.targetgraph.raw")
            which should be translated to
            [`UnconfiguredTargetNodeWithDeps`](../../core/model/targetgraph/raw/UnconfiguredTargetNodeWithDeps.html "class in com.facebook.buck.core.model.targetgraph.raw")
            :::

        []{#getPackagePath()}

        -   #### getPackagePath

            ``` methodSignature
            public abstract Path getPackagePath()
            ```

            ::: block
            [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
            to the root of a package that has this
            [`UnconfiguredTargetNode`](../../core/model/targetgraph/raw/UnconfiguredTargetNode.html "interface in com.facebook.buck.core.model.targetgraph.raw"),
            relative to parse root, usually cell root
            :::

        []{#check()}

        -   #### check

            ``` methodSignature
            @Check
            protected void check()
            ```

        []{#getIdentifier()}

        -   #### getIdentifier

            ``` methodSignature
            public ComputationIdentifier<UnconfiguredTargetNodeWithDeps> getIdentifier()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getIdentifier` in
                interface `ComputeKey<UnconfiguredTargetNodeWithDeps>`

            [Returns:]{.returnLabel}
            :   the identifier of this key. This identifier is used to
                map all keys of the same
                [`ComputationIdentifier`](../../core/graph/transformation/model/ComputationIdentifier.html "interface in com.facebook.buck.core.graph.transformation.model")
                to the same
                [`GraphComputation`](../../core/graph/transformation/GraphComputation.html "interface in com.facebook.buck.core.graph.transformation").
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

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
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

<div>

-   Summary: 
-   Nested \| 
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

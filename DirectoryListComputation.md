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
-   Field \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.core.files](package-summary.html)
:::

## Class DirectoryListComputation {#class-directorylistcomputation .title title="Class DirectoryListComputation"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.files.DirectoryListComputation

::: description
-   

    All Implemented Interfaces:
    :   `GraphComputation<DirectoryListKey,​DirectoryList>`

    ------------------------------------------------------------------------

        public class DirectoryListComputation
        extends Object
        implements GraphComputation<DirectoryListKey,​DirectoryList>

    ::: block
    Produce a list of files and directories in provided folder
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `co                   | `discoverDeps         | ::: block             |
        | m.google.common.colle | ​(DirectoryListKey key | Compute dependent     |
        | ct.ImmutableSet<? ext | ,             Computa | keys required to      |
        | ends ComputeKey<? ext | tionEnvironment env)` | compute given key,    |
        | ends ComputeResult>>` |                       | and a set of          |
        |                       |                       | dependencies as       |
        |                       |                       | listed by             |
        |                       |                       | [`Graph               |
        |                       |                       | Computation.discoverP |
        |                       |                       | reliminaryDeps(Comput |
        |                       |                       | eKey)`](../graph/tran |
        |                       |                       | sformation/GraphCompu |
        |                       |                       | tation.html#discoverP |
        |                       |                       | reliminaryDeps(Key)). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `co                   | `disc                 | ::: block             |
        | m.google.common.colle | overPreliminaryDeps​(D | Compute dependent     |
        | ct.ImmutableSet<? ext | irectoryListKey key)` | keys required to      |
        | ends ComputeKey<? ext |                       | compute given the     |
        | ends ComputeResult>>` |                       | current key.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ComputationIdent     | `getIdentifier()`     |                       |
        | ifier<DirectoryList>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Dire          | `of​(ProjectFilesystem |                       |
        | ctoryListComputation` | View fileSystemView)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `DirectoryList`       | `transf               | ::: block             |
        |                       | orm​(DirectoryListKey  | Perform a             |
        |                       | key,          Computa | transformation        |
        |                       | tionEnvironment env)` | identified by key     |
        |                       |                       | [`GraphComputation`]( |
        |                       |                       | ../graph/transformati |
        |                       |                       | on/GraphComputation.h |
        |                       |                       | tml "interface in com |
        |                       |                       | .facebook.buck.core.g |
        |                       |                       | raph.transformation") |
        |                       |                       | into a final type     |
        |                       |                       | [                     |
        |                       |                       | `GraphComputation`](. |
        |                       |                       | ./graph/transformatio |
        |                       |                       | n/GraphComputation.ht |
        |                       |                       | ml "interface in com. |
        |                       |                       | facebook.buck.core.gr |
        |                       |                       | aph.transformation"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#of(com.facebook.buck.io.filesystem.ProjectFilesystemView)}

        -   #### of

            ``` methodSignature
            public static DirectoryListComputation of​(ProjectFilesystemView fileSystemView)
            ```

        []{#getIdentifier()}

        -   #### getIdentifier

            ``` methodSignature
            public ComputationIdentifier<DirectoryList> getIdentifier()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getIdentifier` in
                interface `GraphComputation<DirectoryListKey,​DirectoryList>`

            [Returns:]{.returnLabel}
            :   the identifier of the key for this transformation. This
                should match
                [`ComputeKey.getIdentifier()`](../graph/transformation/model/ComputeKey.html#getIdentifier())

        []{#transform(com.facebook.buck.core.files.DirectoryListKey,com.facebook.buck.core.graph.transformation.ComputationEnvironment)}

        -   #### transform

            ``` methodSignature
            public DirectoryList transform​(DirectoryListKey key,
                                           ComputationEnvironment env)
                                    throws Exception
            ```

            ::: block
            [Description copied from
            interface: `GraphComputation`]{.descfrmTypeLabel}
            :::

            ::: block
            Perform a transformation identified by key
            [`GraphComputation`](../graph/transformation/GraphComputation.html "interface in com.facebook.buck.core.graph.transformation")
            into a final type
            [`GraphComputation`](../graph/transformation/GraphComputation.html "interface in com.facebook.buck.core.graph.transformation").
            This transformation should be performed synchronously.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `transform` in
                interface `GraphComputation<DirectoryListKey,​DirectoryList>`

            [Parameters:]{.paramLabel}
            :   `key` - The Key of the requested result
            :   `env` - The execution environment containing results of
                keys from
                [`GraphComputation.discoverDeps(ComputeKey, ComputationEnvironment)`](../graph/transformation/GraphComputation.html#discoverDeps(Key,com.facebook.buck.core.graph.transformation.ComputationEnvironment))
                and
                [`GraphComputation.discoverPreliminaryDeps(ComputeKey)`](../graph/transformation/GraphComputation.html#discoverPreliminaryDeps(Key))

            [Returns:]{.returnLabel}
            :   The result of the transformation

            [Throws:]{.throwsLabel}
            :   `Exception`

        []{#discoverDeps(com.facebook.buck.core.files.DirectoryListKey,com.facebook.buck.core.graph.transformation.ComputationEnvironment)}

        -   #### discoverDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<? extends ComputeKey<? extends ComputeResult>> discoverDeps​(DirectoryListKey key,
                                                                                                                      ComputationEnvironment env)
            ```

            ::: block
            [Description copied from
            interface: `GraphComputation`]{.descfrmTypeLabel}
            :::

            ::: block
            Compute dependent keys required to compute given key, and a
            set of dependencies as listed by
            [`GraphComputation.discoverPreliminaryDeps(ComputeKey)`](../graph/transformation/GraphComputation.html#discoverPreliminaryDeps(Key)).
            The results of those computations will be available in
            [`GraphComputation.transform(ComputeKey, ComputationEnvironment)`](../graph/transformation/GraphComputation.html#transform(Key,com.facebook.buck.core.graph.transformation.ComputationEnvironment))
            as a part of
            [`ComputationEnvironment`](../graph/transformation/ComputationEnvironment.html "interface in com.facebook.buck.core.graph.transformation")
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `discoverDeps` in
                interface `GraphComputation<DirectoryListKey,​DirectoryList>`

            [Parameters:]{.paramLabel}
            :   `key` - the current key to transform
            :   `env` - The execution environment containing results of
                keys from
                [`GraphComputation.discoverPreliminaryDeps(ComputeKey)`](../graph/transformation/GraphComputation.html#discoverPreliminaryDeps(Key))

            [Returns:]{.returnLabel}
            :   a set of keys that the transformation of the current key
                depends on

        []{#discoverPreliminaryDeps(com.facebook.buck.core.files.DirectoryListKey)}

        -   #### discoverPreliminaryDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<? extends ComputeKey<? extends ComputeResult>> discoverPreliminaryDeps​(DirectoryListKey key)
            ```

            ::: block
            [Description copied from
            interface: `GraphComputation`]{.descfrmTypeLabel}
            :::

            ::: block
            Compute dependent keys required to compute given the current
            key. The results of those computations will be available in
            [`GraphComputation.discoverDeps(ComputeKey, ComputationEnvironment)`](../graph/transformation/GraphComputation.html#discoverDeps(Key,com.facebook.buck.core.graph.transformation.ComputationEnvironment))
            as a part of
            [`ComputationEnvironment`](../graph/transformation/ComputationEnvironment.html "interface in com.facebook.buck.core.graph.transformation"),
            and
            [`GraphComputation.transform(ComputeKey,  ComputationEnvironment)`](../graph/transformation/GraphComputation.html#transform(Key,com.facebook.buck.core.graph.transformation.ComputationEnvironment))
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `discoverPreliminaryDeps` in
                interface `GraphComputation<DirectoryListKey,​DirectoryList>`

            [Parameters:]{.paramLabel}
            :   `key` - the current key to transform

            [Returns:]{.returnLabel}
            :   a set of keys that the
                [`GraphComputation.discoverDeps(ComputeKey, ComputationEnvironment)`](../graph/transformation/GraphComputation.html#discoverDeps(Key,com.facebook.buck.core.graph.transformation.ComputationEnvironment))
                and
                [`GraphComputation.transform(ComputeKey, ComputationEnvironment)`](../graph/transformation/GraphComputation.html#transform(Key,com.facebook.buck.core.graph.transformation.ComputationEnvironment))
                of the current key depends on
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
-   Field \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
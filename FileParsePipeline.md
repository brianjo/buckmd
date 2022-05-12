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
[Package]{.packageLabelInType} [com.facebook.buck.parser](package-summary.html)
:::

## Interface FileParsePipeline\<T extends [FileManifest](api/FileManifest.html "interface in com.facebook.buck.parser.api")\> {#interface-fileparsepipelinet-extends-filemanifest .title title="Interface FileParsePipeline"}
:::

::: contentContainer
::: description
-   

    [Type Parameters:]{.paramLabel}
    :   `T` - The type of node this pipeline will produce (raw nodes,
        target nodes, etc)

    ```{=html}
    <!-- -->
    ```

    All Superinterfaces:
    :   `AutoCloseable`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `BuildFileRawNodeParsePipeline`, `GenericFileParsePipeline`,
        `PackageFileParsePipeline`

    ------------------------------------------------------------------------

        public interface FileParsePipeline<T extends FileManifest>
        extends AutoCloseable

    ::: block
    Abstract node parsing pipeline. Allows implementors to define their
    own logic for creating nodes of type T.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `default T`           | `get                  | ::: block             |
        |                       | File​(Cell cell,       | Obtain all            |
        |                       |   AbsPath buildFile)` | [`TargetN             |
        |                       |                       | ode`](../core/model/t |
        |                       |                       | argetgraph/TargetNode |
        |                       |                       | .html "interface in c |
        |                       |                       | om.facebook.buck.core |
        |                       |                       | .model.targetgraph")s |
        |                       |                       | from a build file.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.c         | `getFileJo            | ::: block             |
        | ommon.util.concurrent | b​(Cell cell,          | Asynchronously obtain |
        | .ListenableFuture<T>` |   AbsPath buildFile)` | all                   |
        |                       |                       | [`TargetN             |
        |                       |                       | ode`](../core/model/t |
        |                       |                       | argetgraph/TargetNode |
        |                       |                       | .html "interface in c |
        |                       |                       | om.facebook.buck.core |
        |                       |                       | .model.targetgraph")s |
        |                       |                       | from a build file.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Default
        Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.AutoCloseable}

            ### Methods inherited from interface java.lang.[AutoCloseable](http://docs.oracle.com/javase/7/docs/api/java/lang/AutoCloseable.html?is-external=true "class or interface in java.lang"){.externalLink}

            `close`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getFile(com.facebook.buck.core.cell.Cell,com.facebook.buck.core.filesystems.AbsPath)}

        -   #### getFile

            ``` methodSignature
            default T getFile​(Cell cell,
                              AbsPath buildFile)
                       throws BuildFileParseException
            ```

            ::: block
            Obtain all
            [`TargetNode`](../core/model/targetgraph/TargetNode.html "interface in com.facebook.buck.core.model.targetgraph")s
            from a build file. This may block if the file is not cached.
            :::

            [Parameters:]{.paramLabel}
            :   `cell` - the
                [`Cell`](../core/cell/Cell.html "interface in com.facebook.buck.core.cell")
                that the build file belongs to.
            :   `buildFile` - absolute path to the file to process.

            [Returns:]{.returnLabel}
            :   all targets from the file

            [Throws:]{.throwsLabel}
            :   `BuildFileParseException` - for syntax errors.

        []{#getFileJob(com.facebook.buck.core.cell.Cell,com.facebook.buck.core.filesystems.AbsPath)}

        -   #### getFileJob

            ``` methodSignature
            com.google.common.util.concurrent.ListenableFuture<T> getFileJob​(Cell cell,
                                                                             AbsPath buildFile)
                                                                      throws BuildTargetException
            ```

            ::: block
            Asynchronously obtain all
            [`TargetNode`](../core/model/targetgraph/TargetNode.html "interface in com.facebook.buck.core.model.targetgraph")s
            from a build file. This will leverage previously cached raw
            contents of the file (if present) but will always loop over
            the contents, so repeated calls (with the same args) are not
            free.
            returned future may throw
            [`BuildFileParseException`](exceptions/BuildFileParseException.html "class in com.facebook.buck.parser.exceptions")
            and
            [`HumanReadableException`](../core/exceptions/HumanReadableException.html "class in com.facebook.buck.core.exceptions").
            :::

            [Parameters:]{.paramLabel}
            :   `cell` - the
                [`Cell`](../core/cell/Cell.html "interface in com.facebook.buck.core.cell")
                that the build file belongs to.
            :   `buildFile` - absolute path to the file to process.

            [Returns:]{.returnLabel}
            :   future.

            [Throws:]{.throwsLabel}
            :   `BuildTargetException`
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

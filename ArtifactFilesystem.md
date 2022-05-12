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
[Package]{.packageLabelInType} [com.facebook.buck.core.artifact](package-summary.html)
:::

## Class ArtifactFilesystem {#class-artifactfilesystem .title title="Class ArtifactFilesystem"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.artifact.ArtifactFilesystem

::: description
-   

    ------------------------------------------------------------------------

        public class ArtifactFilesystem
        extends Object

    ::: block
    A Filesystem for operating on
    [`Artifact`](Artifact.html "interface in com.facebook.buck.core.artifact")s
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                          Description
          ---------------------------------------------------- -------------
          `ArtifactFilesystem​(ProjectFilesystem filesystem)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `cop                  | ::: block             |
        |                       | y​(Artifact toCopy,    | Makes a copy of the   |
        |                       |   Artifact dest,      | given                 |
        |                       | CopySourceMode mode)` | [`Artifact`           |
        |                       |                       | ](Artifact.html "inte |
        |                       |                       | rface in com.facebook |
        |                       |                       | .buck.core.artifact") |
        |                       |                       | to the given          |
        |                       |                       | destination           |
        |                       |                       | [`Artifact`]          |
        |                       |                       | (Artifact.html "inter |
        |                       |                       | face in com.facebook. |
        |                       |                       | buck.core.artifact"), |
        |                       |                       | with copy behaviour   |
        |                       |                       | as specified by the   |
        |                       |                       | [`CopySourceMode`]    |
        |                       |                       | (../../io/filesystem/ |
        |                       |                       | CopySourceMode.html " |
        |                       |                       | enum in com.facebook. |
        |                       |                       | buck.io.filesystem"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `createPackagePaths​(c | ::: block             |
        |                       | om.google.common.coll | Create the package    |
        |                       | ect.ImmutableSet<Outp | paths that actions    |
        |                       | utArtifact> outputs)` | will write into if it |
        |                       |                       | does not exist        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `InputStream`         | `getInputStrea        |                       |
        |                       | m​(Artifact artifact)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `OutputStream`        | `getOutputStrea       |                       |
        |                       | m​(Artifact artifact,  |                       |
        |                       |                FileAt |                       |
        |                       | tribute<?>... attrs)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `makeExecutabl        | ::: block             |
        |                       | e​(Artifact artifact)` | Make an               |
        |                       |                       | [`Artifact`           |
        |                       |                       | ](Artifact.html "inte |
        |                       |                       | rface in com.facebook |
        |                       |                       | .buck.core.artifact") |
        |                       |                       | executable            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `r                    | ::: block             |
        |                       | emoveBuildArtifacts​(c | Remove build          |
        |                       | om.google.common.coll | artifacts (only) that |
        |                       | ect.ImmutableSet<Outp | exist on the          |
        |                       | utArtifact> outputs)` | underlying            |
        |                       |                       | filesystem.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `stringif             | ::: block             |
        |                       | y​(Artifact artifact)` | Expand an artifact    |
        |                       |                       | into a command line   |
        |                       |                       | argument.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `stringifyAbsolut     | ::: block             |
        |                       | e​(Artifact artifact)` | Expand an artifact    |
        |                       |                       | into a command line   |
        |                       |                       | argument.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `writeContent         | ::: block             |
        |                       | sToPath​(String conten | Write a string to a   |
        |                       | ts,                   | given                 |
        |                       |   Artifact artifact)` | [`Artifact`]          |
        |                       |                       | (Artifact.html "inter |
        |                       |                       | face in com.facebook. |
        |                       |                       | buck.core.artifact"), |
        |                       |                       | creating parent       |
        |                       |                       | directories as        |
        |                       |                       | necessary             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### ArtifactFilesystem

                public ArtifactFilesystem​(ProjectFilesystem filesystem)

            [Parameters:]{.paramLabel}
            :   `filesystem` - that the
                [`Artifact`](Artifact.html "interface in com.facebook.buck.core.artifact")s
                are relative to.
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getInputStream(com.facebook.buck.core.artifact.Artifact)}

        -   #### getInputStream

            ``` methodSignature
            public InputStream getInputStream​(Artifact artifact)
                                       throws IOException
            ```

            [Parameters:]{.paramLabel}
            :   `artifact` - the artifact to read. It should be bound.

            [Returns:]{.returnLabel}
            :   an
                [`InputStream`](http://docs.oracle.com/javase/7/docs/api/java/io/InputStream.html?is-external=true "class or interface in java.io"){.externalLink}
                of the given artifact.

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getOutputStream(com.facebook.buck.core.artifact.Artifact,java.nio.file.attribute.FileAttribute...)}

        -   #### getOutputStream

            ``` methodSignature
            public OutputStream getOutputStream​(Artifact artifact,
                                                FileAttribute<?>... attrs)
                                         throws IOException
            ```

            [Parameters:]{.paramLabel}
            :   `artifact` - the artifact to write. It should be bound.

            [Returns:]{.returnLabel}
            :   an
                [`OutputStream`](http://docs.oracle.com/javase/7/docs/api/java/io/OutputStream.html?is-external=true "class or interface in java.io"){.externalLink}
                of the given artifact.

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#writeContentsToPath(java.lang.String,com.facebook.buck.core.artifact.Artifact)}

        -   #### writeContentsToPath

            ``` methodSignature
            public void writeContentsToPath​(String contents,
                                            Artifact artifact)
                                     throws IOException
            ```

            ::: block
            Write a string to a given
            [`Artifact`](Artifact.html "interface in com.facebook.buck.core.artifact"),
            creating parent directories as necessary
            :::

            [Parameters:]{.paramLabel}
            :   `contents` - the desired contents
            :   `artifact` - the artifact to write. It must be bound.

            [Throws:]{.throwsLabel}
            :   `IOException` - The file could not be written

        []{#makeExecutable(com.facebook.buck.core.artifact.Artifact)}

        -   #### makeExecutable

            ``` methodSignature
            public void makeExecutable​(Artifact artifact)
                                throws IOException
            ```

            ::: block
            Make an
            [`Artifact`](Artifact.html "interface in com.facebook.buck.core.artifact")
            executable
            :::

            [Parameters:]{.paramLabel}
            :   `artifact` - the artifact to write. It must be bound.

            [Throws:]{.throwsLabel}
            :   `IOException` - Making the file executable failed

        []{#copy(com.facebook.buck.core.artifact.Artifact,com.facebook.buck.core.artifact.Artifact,com.facebook.buck.io.filesystem.CopySourceMode)}

        -   #### copy

            ``` methodSignature
            public void copy​(Artifact toCopy,
                             Artifact dest,
                             CopySourceMode mode)
                      throws IOException
            ```

            ::: block
            Makes a copy of the given
            [`Artifact`](Artifact.html "interface in com.facebook.buck.core.artifact")
            to the given destination
            [`Artifact`](Artifact.html "interface in com.facebook.buck.core.artifact"),
            with copy behaviour as specified by the
            [`CopySourceMode`](../../io/filesystem/CopySourceMode.html "enum in com.facebook.buck.io.filesystem").
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#stringify(com.facebook.buck.core.artifact.Artifact)}

        -   #### stringify

            ``` methodSignature
            public String stringify​(Artifact artifact)
            ```

            ::: block
            Expand an artifact into a command line argument.
            NOTE: This should not be used just to get a string version
            of a path. This API may become more restrictive in the
            future if necessary.
            :::

            [Parameters:]{.paramLabel}
            :   `artifact` - a bound artifact whose path is requested

            [Returns:]{.returnLabel}
            :   The path to an artifact as a string

        []{#stringifyAbsolute(com.facebook.buck.core.artifact.Artifact)}

        -   #### stringifyAbsolute

            ``` methodSignature
            public String stringifyAbsolute​(Artifact artifact)
            ```

            ::: block
            Expand an artifact into a command line argument.
            NOTE: This should not be used just to get a string version
            of a path. This API may become more restrictive in the
            future if necessary. When possible, then non-absolute
            version of this function
            ([`stringify(Artifact)`](#stringify(com.facebook.buck.core.artifact.Artifact))
            should be used.
            :::

            [Parameters:]{.paramLabel}
            :   `artifact` - a bound artifact whose path is requested

            [Returns:]{.returnLabel}
            :   The path to an artifact as a string

        []{#createPackagePaths(com.google.common.collect.ImmutableSet)}

        -   #### createPackagePaths

            ``` methodSignature
            public void createPackagePaths​(com.google.common.collect.ImmutableSet<OutputArtifact> outputs)
                                    throws IOException
            ```

            ::: block
            Create the package paths that actions will write into if it
            does not exist
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#removeBuildArtifacts(com.google.common.collect.ImmutableSet)}

        -   #### removeBuildArtifacts

            ``` methodSignature
            public void removeBuildArtifacts​(com.google.common.collect.ImmutableSet<OutputArtifact> outputs)
                                      throws IOException
            ```

            ::: block
            Remove build artifacts (only) that exist on the underlying
            filesystem.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`
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

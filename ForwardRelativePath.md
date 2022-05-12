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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.core.path](package-summary.html)
:::

## Class ForwardRelativePath {#class-forwardrelativepath .title title="Class ForwardRelativePath"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.path.ForwardRelativePath

::: description
-   

    All Implemented Interfaces:
    :   `Comparable<ForwardRelativePath>`

    ------------------------------------------------------------------------

        public class ForwardRelativePath
        extends Object
        implements Comparable<ForwardRelativePath>

    ::: block
    A normalized relative path object which:
    -   Does not contain dot or dot-dot
    -   Does not start and does not end with slash
    -   Does not contain slash-slash
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type              Field     Description
          ------------------------------ --------- -------------
          `static ForwardRelativePath`   `EMPTY`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `int`                 | `compareTo​(Forwa      |                       |
        |                       | rdRelativePath that)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `endsWith​(Forwa       | ::: block             |
        |                       | rdRelativePath path)` | This path ends with   |
        |                       |                       | given path.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `equals​(Object o)`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isEmpty()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<            | `nameAsPath()`        | ::: block             |
        | ForwardRelativePath>` |                       | Last segment of path  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `of​(String path)`     | ::: block             |
        |  ForwardRelativePath` |                       | Parse a string into   |
        |                       |                       | path.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `ofPath​(Path path)`   | ::: block             |
        |  ForwardRelativePath` |                       | Construct from given  |
        |                       |                       | relative              |
        |                       |                       | [`Path`](http://doc   |
        |                       |                       | s.oracle.com/javase/7 |
        |                       |                       | /docs/api/java/nio/fi |
        |                       |                       | le/Path.html?is-exter |
        |                       |                       | nal=true "class or in |
        |                       |                       | terface in java.nio.f |
        |                       |                       | ile"){.externalLink}. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `ofSubs               | ::: block             |
        |  ForwardRelativePath` | tring​(String path,    | Parse a string into   |
        |                       |          int offset)` | path removing .       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<            | `parent()`            | ::: block             |
        | ForwardRelativePath>` |                       | Path without last     |
        |                       |                       | segment               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `relativize​(Forwar    | ::: block             |
        |                       | dRelativePath other)` | Constructs a relative |
        |                       |                       | path between this     |
        |                       |                       | path and a given      |
        |                       |                       | path.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ForwardRelativePath` | `resolve​(Forwar       | ::: block             |
        |                       | dRelativePath other)` | Append given path to  |
        |                       |                       | the current path      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ForwardRelativePath` | `r                    |                       |
        |                       | esolve​(String other)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `segments()`          |                       |
        | ogle.common.collect.I |                       |                       |
        | mmutableList<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `startsWith​(Forwa     | ::: block             |
        |                       | rdRelativePath path)` | This path starts with |
        |                       |                       | given path.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `toPath​(Fi            | ::: block             |
        |                       | leSystem fileSystem)` | Convert file path to  |
        |                       |                       | a relative path in    |
        |                       |                       | given filesystem.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `toPat                | ::: block             |
        |                       | hDefaultFileSystem()` | Convert this path to  |
        |                       |                       | the                   |
        |                       |                       | [`Path`](http://do    |
        |                       |                       | cs.oracle.com/javase/ |
        |                       |                       | 7/docs/api/java/nio/f |
        |                       |                       | ile/Path.html?is-exte |
        |                       |                       | rnal=true "class or i |
        |                       |                       | nterface in java.nio. |
        |                       |                       | file"){.externalLink} |
        |                       |                       | of                    |
        |                       |                       | [`FileSystems.get     |
        |                       |                       | Default()`](http://do |
        |                       |                       | cs.oracle.com/javase/ |
        |                       |                       | 7/docs/api/java/nio/f |
        |                       |                       | ile/FileSystems.html? |
        |                       |                       | is-external=true#getD |
        |                       |                       | efault() "class or in |
        |                       |                       | terface in java.nio.f |
        |                       |                       | ile"){.externalLink}. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toPathPrefix()`      | ::: block             |
        |                       |                       | A string to be        |
        |                       |                       | prepended to another  |
        |                       |                       | path to make a        |
        |                       |                       | relative path         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RelPath`             | `toRelPath​(Fi         |                       |
        |                       | leSystem fileSystem)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#EMPTY}

        -   #### EMPTY

                public static final ForwardRelativePath EMPTY
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#of(java.lang.String)}

        -   #### of

            ``` methodSignature
            public static ForwardRelativePath of​(String path)
            ```

            ::: block
            Parse a string into path.
            This function throws if path is not normalized (e. g.
            contains two consecutive slashes).
            :::

        []{#ofSubstring(java.lang.String,int)}

        -   #### ofSubstring

            ``` methodSignature
            public static ForwardRelativePath ofSubstring​(String path,
                                                          int offset)
            ```

            ::: block
            Parse a string into path removing .
            This function throws if path is not normalized (e. g.
            contains two consecutive slashes).
            :::

            [Parameters:]{.paramLabel}
            :   `offset` - is the number of characters to be removed
                from the path before parsing (useful in certain cases to
                avoid extra string allocation).

        []{#ofPath(java.nio.file.Path)}

        -   #### ofPath

            ``` methodSignature
            public static ForwardRelativePath ofPath​(Path path)
            ```

            ::: block
            Construct from given relative
            [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}.
            This functions calls
            [`Path.normalize()`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true#normalize() "class or interface in java.nio.file"){.externalLink}.
            Throw if path is not relative.
            :::

        []{#resolve(com.facebook.buck.core.path.ForwardRelativePath)}

        -   #### resolve

            ``` methodSignature
            public ForwardRelativePath resolve​(ForwardRelativePath other)
            ```

            ::: block
            Append given path to the current path
            :::

        []{#resolve(java.lang.String)}

        -   #### resolve

            ``` methodSignature
            public ForwardRelativePath resolve​(String other)
            ```

        []{#isEmpty()}

        -   #### isEmpty

            ``` methodSignature
            public boolean isEmpty()
            ```

        []{#toPath(java.nio.file.FileSystem)}

        -   #### toPath

            ``` methodSignature
            public Path toPath​(FileSystem fileSystem)
            ```

            ::: block
            Convert file path to a relative path in given filesystem.
            Note this function is optimized for
            [`BuckFileSystem`](../filesystems/BuckFileSystem.html "class in com.facebook.buck.core.filesystems")
            (avoids re-parsing and re-interning).
            :::

        []{#toPathDefaultFileSystem()}

        -   #### toPathDefaultFileSystem

            ``` methodSignature
            public Path toPathDefaultFileSystem()
            ```

            ::: block
            Convert this path to the
            [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
            of
            [`FileSystems.getDefault()`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/FileSystems.html?is-external=true#getDefault() "class or interface in java.nio.file"){.externalLink}.
            :::

        []{#toRelPath(java.nio.file.FileSystem)}

        -   #### toRelPath

            ``` methodSignature
            public RelPath toRelPath​(FileSystem fileSystem)
            ```

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

        []{#nameAsPath()}

        -   #### nameAsPath

            ``` methodSignature
            public Optional<ForwardRelativePath> nameAsPath()
            ```

            ::: block
            Last segment of path
            :::

        []{#parent()}

        -   #### parent

            ``` methodSignature
            public Optional<ForwardRelativePath> parent()
            ```

            ::: block
            Path without last segment
            :::

        []{#toPathPrefix()}

        -   #### toPathPrefix

            ``` methodSignature
            public String toPathPrefix()
            ```

            ::: block
            A string to be prepended to another path to make a relative
            path
            :::

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(Object o)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `Object`

        []{#startsWith(com.facebook.buck.core.path.ForwardRelativePath)}

        -   #### startsWith

            ``` methodSignature
            public boolean startsWith​(ForwardRelativePath path)
            ```

            ::: block
            This path starts with given path.
            `ab/cd` starts with `ab/cd`, `ab`, but not `ab/c`.
            :::

        []{#endsWith(com.facebook.buck.core.path.ForwardRelativePath)}

        -   #### endsWith

            ``` methodSignature
            public boolean endsWith​(ForwardRelativePath path)
            ```

            ::: block
            This path ends with given path.
            `ab/cd` ends with `ab/cd`, `cd`, but not `b/cd`.
            :::

        []{#segments()}

        -   #### segments

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> segments()
            ```

        []{#relativize(com.facebook.buck.core.path.ForwardRelativePath)}

        -   #### relativize

            ``` methodSignature
            public String relativize​(ForwardRelativePath other)
            ```

            ::: block
            Constructs a relative path between this path and a given
            path.
            Returns empty string when paths are equal.
            :::

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `Object`

        []{#compareTo(com.facebook.buck.core.path.ForwardRelativePath)}

        -   #### compareTo

            ``` methodSignature
            public int compareTo​(ForwardRelativePath that)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `compareTo` in
                interface `Comparable<ForwardRelativePath>`
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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

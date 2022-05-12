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
[Package]{.packageLabelInType} [com.facebook.buck.file](package-summary.html)
:::

## Class FileHash {#class-filehash .title title="Class FileHash"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.file.FileHash

::: description
-   

    ------------------------------------------------------------------------

        public class FileHash
        extends Object

    ::: block
    A small class that encapsulates a file hash that is either sha1, or
    sha256
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `boolean`             | `equals​(Object o)`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `getHashCode()`       | ::: block             |
        | common.hash.HashCode` |                       | Get the original hash |
        |                       |                       | code object used to   |
        |                       |                       | create this           |
        |                       |                       | [`FileHash`](FileHa   |
        |                       |                       | sh.html "class in com |
        |                       |                       | .facebook.buck.file") |
        |                       |                       | object                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.comm      | `getHashFunction()`   | ::: block             |
        | on.hash.HashFunction` |                       | Get the hash function |
        |                       |                       | for this type of hash |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static FileHash`     | `ofS                  | ::: block             |
        |                       | ha1​(com.google.common | Create a              |
        |                       | .hash.HashCode sha1)` | [`FileHash`](FileHa   |
        |                       |                       | sh.html "class in com |
        |                       |                       | .facebook.buck.file") |
        |                       |                       | object with a sha1    |
        |                       |                       | hash                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static FileHash`     | `ofSha25              | ::: block             |
        |                       | 6​(com.google.common.h | Create a              |
        |                       | ash.HashCode sha256)` | [`FileHash`](FileHa   |
        |                       |                       | sh.html "class in com |
        |                       |                       | .facebook.buck.file") |
        |                       |                       | object with a sha1    |
        |                       |                       | hash                  |
        |                       |                       | :::                   |
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
    -   []{#method.detail}

        ### Method Detail

        []{#ofSha1(com.google.common.hash.HashCode)}

        -   #### ofSha1

            ``` methodSignature
            public static FileHash ofSha1​(com.google.common.hash.HashCode sha1)
            ```

            ::: block
            Create a
            [`FileHash`](FileHash.html "class in com.facebook.buck.file")
            object with a sha1 hash
            :::

        []{#ofSha256(com.google.common.hash.HashCode)}

        -   #### ofSha256

            ``` methodSignature
            public static FileHash ofSha256​(com.google.common.hash.HashCode sha256)
            ```

            ::: block
            Create a
            [`FileHash`](FileHash.html "class in com.facebook.buck.file")
            object with a sha1 hash
            :::

        []{#getHashFunction()}

        -   #### getHashFunction

            ``` methodSignature
            public com.google.common.hash.HashFunction getHashFunction()
            ```

            ::: block
            Get the hash function for this type of hash
            :::

        []{#getHashCode()}

        -   #### getHashCode

            ``` methodSignature
            public com.google.common.hash.HashCode getHashCode()
            ```

            ::: block
            Get the original hash code object used to create this
            [`FileHash`](FileHash.html "class in com.facebook.buck.file")
            object
            :::

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(Object o)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `Object`

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `Object`
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

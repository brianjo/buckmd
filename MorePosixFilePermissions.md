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
[Package]{.packageLabelInType} [com.facebook.buck.io.file](package-summary.html)
:::

## Class MorePosixFilePermissions {#class-moreposixfilepermissions .title title="Class MorePosixFilePermissions"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.io.file.MorePosixFilePermissions

::: description
-   

    ------------------------------------------------------------------------

        public class MorePosixFilePermissions
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type           Field                        Description
          --------------------------- ---------------------------- -------------
          `static FileAttribute<?>`   `READ_ONLY_FILE_ATTRIBUTE`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `stat                 | `addExec              | ::: block             |
        | ic com.google.common. | utePermissionsIfReada | Return a new set of   |
        | collect.ImmutableSet< | ble​(Set<PosixFilePerm | permissions which     |
        | PosixFilePermission>` | ission> permissions)` | include execute       |
        |                       |                       | permission for each   |
        |                       |                       | of the roles that     |
        |                       |                       | already have read     |
        |                       |                       | permissions (e.g.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `stat                 | `fromMode​(long mode)` | ::: block             |
        | ic com.google.common. |                       | Convert a unix bit    |
        | collect.ImmutableSet< |                       | representation (e.g.  |
        | PosixFilePermission>` |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static long`         | `toM                  | ::: block             |
        |                       | ode​(Set<PosixFilePerm | Convert a set of      |
        |                       | ission> permissions)` | posix file            |
        |                       |                       | permissions the unix  |
        |                       |                       | bit representation    |
        |                       |                       | (e.g.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
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

        []{#READ_ONLY_FILE_ATTRIBUTE}

        -   #### READ_ONLY_FILE_ATTRIBUTE

                public static final FileAttribute<?> READ_ONLY_FILE_ATTRIBUTE
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#toMode(java.util.Set)}

        -   #### toMode

            ``` methodSignature
            public static long toMode​(Set<PosixFilePermission> permissions)
            ```

            ::: block
            Convert a set of posix file permissions the unix bit
            representation (e.g. 0644).
            :::

        []{#fromMode(long)}

        -   #### fromMode

            ``` methodSignature
            public static com.google.common.collect.ImmutableSet<PosixFilePermission> fromMode​(long mode)
            ```

            ::: block
            Convert a unix bit representation (e.g. 0644) into a set of
            posix file permissions.
            :::

        []{#addExecutePermissionsIfReadable(java.util.Set)}

        -   #### addExecutePermissionsIfReadable

            ``` methodSignature
            public static com.google.common.collect.ImmutableSet<PosixFilePermission> addExecutePermissionsIfReadable​(Set<PosixFilePermission> permissions)
            ```

            ::: block
            Return a new set of permissions which include execute
            permission for each of the roles that already have read
            permissions (e.g. 0606 =\> 0707).
            :::
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

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
[Package]{.packageLabelInType} [com.facebook.buck.skylark.io.impl](package-summary.html)
:::

## Class NativeGlobber {#class-nativeglobber .title title="Class NativeGlobber"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.skylark.io.impl.NativeGlobber

::: description
-   

    All Implemented Interfaces:
    :   `Globber`

    ------------------------------------------------------------------------

        public class NativeGlobber
        extends Object
        implements Globber

    ::: block
    A Java native glob function implementation that allows resolving
    file paths based on include patterns (file patterns that should be
    returned) minus exclude patterns (file patterns that should be
    excluded from the resulting set).
    Since this is a simple implementation it does not support caching
    and other smarts.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `                     | `create​(com.goo       | ::: block             |
        | static NativeGlobber` | gle.devtools.build.li | Factory method for    |
        |                       | b.vfs.Path basePath)` | creating              |
        |                       |                       | [`NativeGlobber`](N   |
        |                       |                       | ativeGlobber.html "cl |
        |                       |                       | ass in com.facebook.b |
        |                       |                       | uck.skylark.io.impl") |
        |                       |                       | instances.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Set<String>`         | `run​(Collec           |                       |
        |                       | tion<String> include, |                       |
        |                       |     Collection<String |                       |
        |                       | > exclude,    boolean |                       |
        |                       |  excludeDirectories)` |                       |
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

        []{#run(java.util.Collection,java.util.Collection,boolean)}

        -   #### run

            ``` methodSignature
            public Set<String> run​(Collection<String> include,
                                   Collection<String> exclude,
                                   boolean excludeDirectories)
                            throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `run` in interface `Globber`

            [Parameters:]{.paramLabel}
            :   `include` - File patterns that should be included in the
                resulting set.
            :   `exclude` - File patterns that should be excluded from
                the resulting set.
            :   `excludeDirectories` - Whether directories should be
                excluded from the resulting set.

            [Returns:]{.returnLabel}
            :   The set of paths resolved using include patterns minus
                paths excluded by exclude patterns.

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#create(com.google.devtools.build.lib.vfs.Path)}

        -   #### create

            ``` methodSignature
            public static NativeGlobber create​(com.google.devtools.build.lib.vfs.Path basePath)
            ```

            ::: block
            Factory method for creating
            [`NativeGlobber`](NativeGlobber.html "class in com.facebook.buck.skylark.io.impl")
            instances.
            :::

            [Parameters:]{.paramLabel}
            :   `basePath` - The base path relative to which paths
                matching glob patterns will be resolved.
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

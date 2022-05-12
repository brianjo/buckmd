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
[Package]{.packageLabelInType} [com.facebook.buck.cxx](package-summary.html)
:::

## Class OmnibusRoots.Builder {#class-omnibusroots.builder .title title="Class OmnibusRoots.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.OmnibusRoots.Builder

::: description
-   

    Enclosing class:
    :   [OmnibusRoots](OmnibusRoots.html "class in com.facebook.buck.cxx")

    ------------------------------------------------------------------------

        public static class OmnibusRoots.Builder
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `addExcludedRoot​(     | ::: block             |
        |                       | NativeLinkable root)` | Add a root which is   |
        |                       |                       | excluded from omnibus |
        |                       |                       | linking.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `addIncludedRoot​(Na   | ::: block             |
        |                       | tiveLinkTarget root)` | Add a root which is   |
        |                       |                       | included in omnibus   |
        |                       |                       | linking.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `addPo                | ::: block             |
        |                       | tentialRoot​(NativeLin | Add a node which may  |
        |                       | kable node,           | qualify as either an  |
        |                       |        boolean includ | included root, and    |
        |                       | ePrivateLinkerFlags)` | excluded root, or     |
        |                       |                       | neither.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OmnibusRoots`        | `build()`             |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isEmpty()`           |                       |
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
    -   []{#method.detail}

        ### Method Detail

        []{#addIncludedRoot(com.facebook.buck.cxx.toolchain.nativelink.NativeLinkTarget)}

        -   #### addIncludedRoot

            ``` methodSignature
            public void addIncludedRoot​(NativeLinkTarget root)
            ```

            ::: block
            Add a root which is included in omnibus linking.
            :::

        []{#addExcludedRoot(com.facebook.buck.cxx.toolchain.nativelink.NativeLinkable)}

        -   #### addExcludedRoot

            ``` methodSignature
            public void addExcludedRoot​(NativeLinkable root)
            ```

            ::: block
            Add a root which is excluded from omnibus linking.
            :::

        []{#addPotentialRoot(com.facebook.buck.cxx.toolchain.nativelink.NativeLinkable,boolean)}

        -   #### addPotentialRoot

            ``` methodSignature
            public void addPotentialRoot​(NativeLinkable node,
                                         boolean includePrivateLinkerFlags)
            ```

            ::: block
            Add a node which may qualify as either an included root, and
            excluded root, or neither.
            :::

        []{#isEmpty()}

        -   #### isEmpty

            ``` methodSignature
            public boolean isEmpty()
            ```

        []{#build()}

        -   #### build

            ``` methodSignature
            public OmnibusRoots build()
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

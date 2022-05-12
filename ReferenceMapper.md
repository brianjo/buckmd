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
[Package]{.packageLabelInType} [com.facebook.buck.android.resources](package-summary.html)
:::

## Interface ReferenceMapper {#interface-referencemapper .title title="Interface ReferenceMapper"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `BringToFrontMapper`

    ------------------------------------------------------------------------

        public interface ReferenceMapper

    ::: block
    A ReferenceMapper is used to reassign ids in Android\'s .arsc/.xml
    files.
    Android .arsc/.xml files include many resource references. These are
    ints of the form 0xPPTTIIII encoding three things: package, type,
    index. The index part is an index into an array of integers (or
    rather, into multiple arrays of integers).

    A ReferenceMapper implements a method to update references and to
    rewrite those arrays that they refer to.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `int`                 | `map​(int id)`         | ::: block             |
        |                       |                       | Converts an id to its |
        |                       |                       | new value under this  |
        |                       |                       | mapping.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `rewrite​(int type,    | ::: block             |
        |                       |       IntBuffer buf)` | Given an IntBuffer    |
        |                       |                       | with an entry for     |
        |                       |                       | every value of the    |
        |                       |                       | given type,           |
        |                       |                       | rearranges the        |
        |                       |                       | entries in the buffer |
        |                       |                       | to match the id       |
        |                       |                       | reassignment.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#map(int)}

        -   #### map

            ``` methodSignature
            int map​(int id)
            ```

            ::: block
            Converts an id to its new value under this mapping.
            :::

        []{#rewrite(int,java.nio.IntBuffer)}

        -   #### rewrite

            ``` methodSignature
            void rewrite​(int type,
                         IntBuffer buf)
            ```

            ::: block
            Given an IntBuffer with an entry for every value of the
            given type, rearranges the entries in the buffer to match
            the id reassignment.
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

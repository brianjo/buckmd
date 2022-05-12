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
[Package]{.packageLabelInType} [com.facebook.buck.android.resources](package-summary.html)
:::

## Class BringToFrontMapper {#class-bringtofrontmapper .title title="Class BringToFrontMapper"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.resources.BringToFrontMapper

::: description
-   

    All Implemented Interfaces:
    :   `ReferenceMapper`

    ------------------------------------------------------------------------

        public class BringToFrontMapper
        extends Object
        implements ReferenceMapper

    ::: block
    BringToFrontMapper supports \"bring-to-front\" reassignment of
    reference ids. Given a set of ids, it will construct an assignment
    that ensures that those ids are the first ones for each type.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                   Description
          ------------------------------------------------------------------------------------------------------------- -------------
          `BringToFrontMapper​(int packageId,                   int[][] mapping,                   int[][] rewriters)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `stati                | `construct​(int        | ::: block             |
        | c BringToFrontMapper` | packageId,          M | Constructs a          |
        |                       | ap<Integer,​SortedSet< | ReferenceMapper that  |
        |                       | Integer>> idsByType)` | will reassign ids and |
        |                       |                       | adjust offsets such   |
        |                       |                       | that for each key in  |
        |                       |                       | idsByType, the ids in |
        |                       |                       | idsByType will be     |
        |                       |                       | reassigned to the     |
        |                       |                       | first n ids of that   |
        |                       |                       | type.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(int,int[][],int[][])}

        -   #### BringToFrontMapper

                public BringToFrontMapper​(int packageId,
                                          int[][] mapping,
                                          int[][] rewriters)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#construct(int,java.util.Map)}

        -   #### construct

            ``` methodSignature
            public static BringToFrontMapper construct​(int packageId,
                                                       Map<Integer,​SortedSet<Integer>> idsByType)
            ```

            ::: block
            Constructs a ReferenceMapper that will reassign ids and
            adjust offsets such that for each key in idsByType, the ids
            in idsByType will be reassigned to the first n ids of that
            type. The ids provided should not include package or type
            ids.
            :::

        []{#map(int)}

        -   #### map

            ``` methodSignature
            public int map​(int id)
            ```

            ::: block
            [Description copied from
            interface: `ReferenceMapper`]{.descfrmTypeLabel}
            :::

            ::: block
            Converts an id to its new value under this mapping.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `map` in interface `ReferenceMapper`

        []{#rewrite(int,java.nio.IntBuffer)}

        -   #### rewrite

            ``` methodSignature
            public void rewrite​(int type,
                                IntBuffer buf)
            ```

            ::: block
            [Description copied from
            interface: `ReferenceMapper`]{.descfrmTypeLabel}
            :::

            ::: block
            Given an IntBuffer with an entry for every value of the
            given type, rearranges the entries in the buffer to match
            the id reassignment.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `rewrite` in interface `ReferenceMapper`
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

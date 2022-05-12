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
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   Method

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
[Package]{.packageLabelInType} [com.facebook.buck.android.dalvik](package-summary.html)
:::

## Class DalvikStatsTool.Stats {#class-dalvikstatstool.stats .title title="Class DalvikStatsTool.Stats"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.dalvik.DalvikStatsTool.Stats

::: description
-   

    Enclosing class:
    :   [DalvikStatsTool](DalvikStatsTool.html "class in com.facebook.buck.android.dalvik")

    ------------------------------------------------------------------------

        public static class DalvikStatsTool.Stats
        extends Object

    ::: block
    Stats about a java class.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Field                 | Description           |
        +=======================+=======================+=======================+
        | `int`                 | `esti                 | ::: block             |
        |                       | matedLinearAllocSize` | Estimated bytes the   |
        |                       |                       | class will contribute |
        |                       |                       | to Dalvik linear      |
        |                       |                       | alloc.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `fieldReferences`     | ::: block             |
        | common.collect.Immuta |                       | Fields referenced by  |
        | bleSet<com.facebook.b |                       | the class.            |
        | uck.android.dalvik.Da |                       | :::                   |
        | lvikMemberReference>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `methodReferences`    | ::: block             |
        | common.collect.Immuta |                       | Methods referenced by |
        | bleSet<com.facebook.b |                       | the class.            |
        | uck.android.dalvik.Da |                       | :::                   |
        | lvikMemberReference>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static D             | `ZERO`                |                       |
        | alvikStatsTool.Stats` |                       |                       |
        +-----------------------+-----------------------+-----------------------+

        : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                  Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `Stats​(int estimatedLinearAllocSize,      Set<com.facebook.buck.android.dalvik.DalvikMemberReference> methodReferences,      Set<com.facebook.buck.android.dalvik.DalvikMemberReference> fieldReferences)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#ZERO}

        -   #### ZERO

                public static final DalvikStatsTool.Stats ZERO

        []{#estimatedLinearAllocSize}

        -   #### estimatedLinearAllocSize

                public final int estimatedLinearAllocSize

            ::: block
            Estimated bytes the class will contribute to Dalvik linear
            alloc.
            :::

        []{#methodReferences}

        -   #### methodReferences

                public final com.google.common.collect.ImmutableSet<com.facebook.buck.android.dalvik.DalvikMemberReference> methodReferences

            ::: block
            Methods referenced by the class.
            :::

        []{#fieldReferences}

        -   #### fieldReferences

                public final com.google.common.collect.ImmutableSet<com.facebook.buck.android.dalvik.DalvikMemberReference> fieldReferences

            ::: block
            Fields referenced by the class.
            :::
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(int,java.util.Set,java.util.Set)}

        -   #### Stats

                public Stats​(int estimatedLinearAllocSize,
                             Set<com.facebook.buck.android.dalvik.DalvikMemberReference> methodReferences,
                             Set<com.facebook.buck.android.dalvik.DalvikMemberReference> fieldReferences)
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
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   Method

</div>

[]{#skip.navbar.bottom}
:::

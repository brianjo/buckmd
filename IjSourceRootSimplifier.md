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
[Package]{.packageLabelInType} [com.facebook.buck.features.project.intellij](package-summary.html)
:::

## Class IjSourceRootSimplifier {#class-ijsourcerootsimplifier .title title="Class IjSourceRootSimplifier"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.project.intellij.IjSourceRootSimplifier

::: description
-   

    ------------------------------------------------------------------------

        public class IjSourceRootSimplifier
        extends Object

    ::: block
    Groups
    [`IjFolder`](model/folders/IjFolder.html "class in com.facebook.buck.features.project.intellij.model.folders")s
    into sets which are of the same type and belong to the same package
    structure.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                     Description
          --------------------------------------------------------------- -------------
          `IjSourceRootSimplifier​(JavaPackageFinder javaPackageFinder)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `                     | `simplify             | ::: block             |
        | com.google.common.col | ​(int simplificationLi | Merges                |
        | lect.ImmutableListMul | mit,         Iterable | [`IjFo                |
        | timap<Path,​IjFolder>` | <IjFolder> folders,   | lder`](model/folders/ |
        |                       |        Path moduleLoc | IjFolder.html "class  |
        |                       | ation,         com.go | in com.facebook.buck. |
        |                       | ogle.common.collect.I | features.project.inte |
        |                       | mmutableSet<Path> tra | llij.model.folders")s |
        |                       | versalBoundaryPaths)` | of the same type and  |
        |                       |                       | package prefix.       |
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

        []{#<init>(com.facebook.buck.jvm.core.JavaPackageFinder)}

        -   #### IjSourceRootSimplifier

                public IjSourceRootSimplifier​(JavaPackageFinder javaPackageFinder)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#simplify(int,java.lang.Iterable,java.nio.file.Path,com.google.common.collect.ImmutableSet)}

        -   #### simplify

            ``` methodSignature
            public com.google.common.collect.ImmutableListMultimap<Path,​IjFolder> simplify​(int simplificationLimit,
                                                                                                 Iterable<IjFolder> folders,
                                                                                                 Path moduleLocation,
                                                                                                 com.google.common.collect.ImmutableSet<Path> traversalBoundaryPaths)
            ```

            ::: block
            Merges
            [`IjFolder`](model/folders/IjFolder.html "class in com.facebook.buck.features.project.intellij.model.folders")s
            of the same type and package prefix.
            :::

            [Parameters:]{.paramLabel}
            :   `simplificationLimit` - if a path has this many segments
                it will not be simplified further.
            :   `folders` - set of
                [`IjFolder`](model/folders/IjFolder.html "class in com.facebook.buck.features.project.intellij.model.folders")s
                to simplify.
            :   `moduleLocation` - location of the current module
            :   `traversalBoundaryPaths` - contains a list of locations
                of modules in the current project

            [Returns:]{.returnLabel}
            :   simplified map of Path,
                [`IjFolder`](model/folders/IjFolder.html "class in com.facebook.buck.features.project.intellij.model.folders")s.
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

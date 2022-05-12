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

## Class IjProject {#class-ijproject .title title="Class IjProject"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.project.intellij.IjProject

::: description
-   

    ------------------------------------------------------------------------

        public class IjProject
        extends Object

    ::: block
    Top-level class for IntelliJ project generation.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                  Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `IjProject​(TargetGraph targetGraph,          JavaPackageFinder javaPackageFinder,          JavaFileParser javaFileParser,          ProjectFilesystem projectFilesystem,          IjProjectConfig projectConfig,          ProjectFilesystem outFilesystem)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.google           | `update()`            | ::: block             |
        | .common.collect.Immut |                       | Write a subset of the |
        | ableSet<BuildTarget>` |                       | project to disk,      |
        |                       |                       | specified by the      |
        |                       |                       | targets passed on the |
        |                       |                       | command line.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `write()`             | ::: block             |
        | .common.collect.Immut |                       | Write the project to  |
        | ableSet<BuildTarget>` |                       | disk.                 |
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

        []{#<init>(com.facebook.buck.core.model.targetgraph.TargetGraph,com.facebook.buck.jvm.core.JavaPackageFinder,com.facebook.buck.jvm.java.JavaFileParser,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.features.project.intellij.model.IjProjectConfig,com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### IjProject

                public IjProject​(TargetGraph targetGraph,
                                 JavaPackageFinder javaPackageFinder,
                                 JavaFileParser javaFileParser,
                                 ProjectFilesystem projectFilesystem,
                                 IjProjectConfig projectConfig,
                                 ProjectFilesystem outFilesystem)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#write()}

        -   #### write

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<BuildTarget> write()
                                                                      throws IOException
            ```

            ::: block
            Write the project to disk.
            :::

            [Returns:]{.returnLabel}
            :   set of
                [`BuildTarget`](../../../core/model/BuildTarget.html "class in com.facebook.buck.core.model")s
                which should be built in order for the project to index
                correctly.

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#update()}

        -   #### update

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<BuildTarget> update()
                                                                       throws IOException
            ```

            ::: block
            Write a subset of the project to disk, specified by the
            targets passed on the command line. Does not perform a clean
            of the project space after updating.
            :::

            [Returns:]{.returnLabel}
            :   set of
                [`BuildTarget`](../../../core/model/BuildTarget.html "class in com.facebook.buck.core.model")s
                which should be built in to allow indexing

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

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

## Class DefaultIjModuleFactory {#class-defaultijmodulefactory .title title="Class DefaultIjModuleFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.project.intellij.DefaultIjModuleFactory

::: description
-   

    All Implemented Interfaces:
    :   `IjModuleFactory`

    ------------------------------------------------------------------------

        public class DefaultIjModuleFactory
        extends Object
        implements IjModuleFactory
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                          Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `DefaultIjModuleFactory​(ProjectFilesystem projectFilesystem,                       IjProjectConfig projectConfig,                       SupportedTargetTypeRegistry typeRegistry)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `IjModule`            | `createModule​(Pat     | ::: block             |
        |                       | h moduleBasePath,     | Create an             |
        |                       |          com.google.c | [`IjModule            |
        |                       | ommon.collect.Immutab | `](model/IjModule.htm |
        |                       | leSet<TargetNode> tar | l "class in com.faceb |
        |                       | getNodes,             | ook.buck.features.pro |
        |                       |  Set<Path> excludes)` | ject.intellij.model") |
        |                       |                       | form the supplied     |
        |                       |                       | parameters.           |
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

        []{#<init>(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.features.project.intellij.model.IjProjectConfig,com.facebook.buck.features.project.intellij.SupportedTargetTypeRegistry)}

        -   #### DefaultIjModuleFactory

                public DefaultIjModuleFactory​(ProjectFilesystem projectFilesystem,
                                              IjProjectConfig projectConfig,
                                              SupportedTargetTypeRegistry typeRegistry)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#createModule(java.nio.file.Path,com.google.common.collect.ImmutableSet,java.util.Set)}

        -   #### createModule

            ``` methodSignature
            public IjModule createModule​(Path moduleBasePath,
                                         com.google.common.collect.ImmutableSet<TargetNode> targetNodes,
                                         Set<Path> excludes)
            ```

            ::: block
            [Description copied from
            interface: `IjModuleFactory`]{.descfrmTypeLabel}
            :::

            ::: block
            Create an
            [`IjModule`](model/IjModule.html "class in com.facebook.buck.features.project.intellij.model")
            form the supplied parameters.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `createModule` in interface `IjModuleFactory`

            [Parameters:]{.paramLabel}
            :   `moduleBasePath` - the top-most directory the module is
                responsible for.
            :   `targetNodes` - set of nodes the module is to be created
                from.

            [Returns:]{.returnLabel}
            :   nice shiny new module.
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

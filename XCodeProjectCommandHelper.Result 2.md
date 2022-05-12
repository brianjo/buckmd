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
[Package]{.packageLabelInType} [com.facebook.buck.features.apple.projectV2](package-summary.html)
:::

## Class XCodeProjectCommandHelper.Result {#class-xcodeprojectcommandhelper.result .title title="Class XCodeProjectCommandHelper.Result"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.apple.projectV2.XCodeProjectCommandHelper.Result

::: description
-   

    Enclosing class:
    :   [XCodeProjectCommandHelper](XCodeProjectCommandHelper.html "class in com.facebook.buck.features.apple.projectV2")

    ------------------------------------------------------------------------

        public static class XCodeProjectCommandHelper.Result
        extends Object

    ::: block
    A result with metadata about the subcommand helper\'s output.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                          Description
          -------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `Result​(BuildTarget inputTarget,       Path outputRelativePath,       PBXProject project,       com.google.common.collect.ImmutableSet<BuildTarget> buildTargets)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                       Method                      Description
          ------------------------------------------------------- --------------------------- -------------
          `com.google.common.collect.ImmutableSet<BuildTarget>`   `getBuildTargets()`          
          `BuildTarget`                                           `getInputTarget()`           
          `Path`                                                  `getOutputRelativePath()`    
          `PBXProject`                                            `getProject()`               

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

        []{#<init>(com.facebook.buck.core.model.BuildTarget,java.nio.file.Path,com.facebook.buck.apple.xcode.xcodeproj.PBXProject,com.google.common.collect.ImmutableSet)}

        -   #### Result

                public Result​(BuildTarget inputTarget,
                              Path outputRelativePath,
                              PBXProject project,
                              com.google.common.collect.ImmutableSet<BuildTarget> buildTargets)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getInputTarget()}

        -   #### getInputTarget

            ``` methodSignature
            public BuildTarget getInputTarget()
            ```

        []{#getOutputRelativePath()}

        -   #### getOutputRelativePath

            ``` methodSignature
            public Path getOutputRelativePath()
            ```

        []{#getProject()}

        -   #### getProject

            ``` methodSignature
            public PBXProject getProject()
            ```

        []{#getBuildTargets()}

        -   #### getBuildTargets

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<BuildTarget> getBuildTargets()
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

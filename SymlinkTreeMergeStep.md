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
[Package]{.packageLabelInType} [com.facebook.buck.step.fs](package-summary.html)
:::

## Class SymlinkTreeMergeStep {#class-symlinktreemergestep .title title="Class SymlinkTreeMergeStep"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.step.fs.SymlinkTreeMergeStep

::: description
-   

    All Implemented Interfaces:
    :   `Step`

    ------------------------------------------------------------------------

        public class SymlinkTreeMergeStep
        extends Object
        implements Step

    ::: block
    A step to merge the contents of provided directories into a symlink
    tree
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `Symlin                           | ::: block                         |
        | kTreeMergeStep​(String category,   | Creates an instance of            |
        |                    ProjectFilesys | [`SymlinkTreeMergeStep            |
        | tem filesystem,                   | `](SymlinkTreeMergeStep.html "cla |
        |    Path root,                     | ss in com.facebook.buck.step.fs") |
        |  SymlinkPaths links,              | :::                               |
        |         java.util.function.BiFunc |                                   |
        | tion<ProjectFilesystem,​Path,​Boole |                                   |
        | an> deleteExistingLinkPredicate)` |                                   |
        +-----------------------------------+-----------------------------------+

        : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type       Method                                       Description
          ----------------------- -------------------------------------------- -------------
          `boolean`               `equals​(Object obj)`                          
          `StepExecutionResult`   `execute​(ExecutionContext context)`           
          `String`                `getDescription​(ExecutionContext context)`    
          `String`                `getShortName()`                              
          `int`                   `hashCode()`                                  

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.lang.String,com.facebook.buck.io.filesystem.ProjectFilesystem,java.nio.file.Path,com.facebook.buck.step.fs.SymlinkPaths,java.util.function.BiFunction)}

        -   #### SymlinkTreeMergeStep

                public SymlinkTreeMergeStep​(String category,
                                            ProjectFilesystem filesystem,
                                            Path root,
                                            SymlinkPaths links,
                                            java.util.function.BiFunction<ProjectFilesystem,​Path,​Boolean> deleteExistingLinkPredicate)

            ::: block
            Creates an instance of
            [`SymlinkTreeMergeStep`](SymlinkTreeMergeStep.html "class in com.facebook.buck.step.fs")
            :::

            [Parameters:]{.paramLabel}
            :   `category` - The type of link tree that will be used.
                This is used in the name
            :   `filesystem` - The filesystem that the root resides on
            :   `root` - The root of the link tree
            :   `links` - A map of relative paths within the link tree
                into which files from the value will be recursively
                linked. e.g. if a file at /tmp/foo/bar should be linked
                as /tmp/symlink-root/subdir/bar, the map should contain
                {Paths.get(\"subdir\"),
            :   `deleteExistingLinkPredicate` - A predicate that, given
                an existing filesystem and target of an existing
                symlink, can return \'true\' if the original link should
                be deleted. This is used in the case that there are
                conflicting files when merging `links` into `root`. A
                common example is dummy \_\_init\_\_.py files placed by
                [`PythonInPlaceBinary`](../../features/python/PythonInPlaceBinary.html "class in com.facebook.buck.features.python")
                which may be deleted safely in the destination directory
                if one of the other directories being merged has a file
                with some substance.
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getDescription(com.facebook.buck.core.build.execution.context.ExecutionContext)}

        -   #### getDescription

            ``` methodSignature
            public String getDescription​(ExecutionContext context)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDescription` in interface `Step`

        []{#getShortName()}

        -   #### getShortName

            ``` methodSignature
            public String getShortName()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getShortName` in interface `Step`

            [Returns:]{.returnLabel}
            :   a short name/description for the command, such as
                \"javac\". Should fit on one line.

        []{#execute(com.facebook.buck.core.build.execution.context.ExecutionContext)}

        -   #### execute

            ``` methodSignature
            public StepExecutionResult execute​(ExecutionContext context)
                                        throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `execute` in interface `Step`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(Object obj)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `Object`

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `Object`
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

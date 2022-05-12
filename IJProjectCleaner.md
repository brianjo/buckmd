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

## Class IJProjectCleaner {#class-ijprojectcleaner .title title="Class IJProjectCleaner"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.project.intellij.IJProjectCleaner

::: description
-   

    ------------------------------------------------------------------------

        public class IJProjectCleaner
        extends Object

    ::: block
    Cleans out any unwanted IntelliJ IDEA project files.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                               Description
          --------------------------------------------------------- -------------
          `IJProjectCleaner​(ProjectFilesystem projectFilesystem)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                                                                                        Description
          ------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `void`              `clean​(BuckConfig buckConfig,      Path ideaConfigDir,      Path librariesXmlBase,      boolean runPostGenerationCleaner,      boolean removeOldLibraries)`    
          `void`              `doNotDelete​(Path path)`                                                                                                                                       
          `void`              `writeFilesToKeepToFile​(String filename)`                                                                                                                      

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

        []{#<init>(com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### IJProjectCleaner

                public IJProjectCleaner​(ProjectFilesystem projectFilesystem)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#doNotDelete(java.nio.file.Path)}

        -   #### doNotDelete

            ``` methodSignature
            public void doNotDelete​(Path path)
            ```

            [Parameters:]{.paramLabel}
            :   `path` - The path to not include in the cleaning
                operation.

        []{#writeFilesToKeepToFile(java.lang.String)}

        -   #### writeFilesToKeepToFile

            ``` methodSignature
            public void writeFilesToKeepToFile​(String filename)
                                        throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#clean(com.facebook.buck.core.config.BuckConfig,java.nio.file.Path,java.nio.file.Path,boolean,boolean)}

        -   #### clean

            ``` methodSignature
            public void clean​(BuckConfig buckConfig,
                              Path ideaConfigDir,
                              Path librariesXmlBase,
                              boolean runPostGenerationCleaner,
                              boolean removeOldLibraries)
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

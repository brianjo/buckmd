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
[Package]{.packageLabelInType} [com.facebook.buck.core.sourcepath](package-summary.html)
:::

## Class PathSourcePath {#class-pathsourcepath .title title="Class PathSourcePath"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.sourcepath.PathSourcePath

::: description
-   

    All Implemented Interfaces:
    :   `SourcePath`, `Comparable<SourcePath>`

    ------------------------------------------------------------------------

        public abstract class PathSourcePath
        extends Object
        implements SourcePath
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor          Description
          -------------------- -------------
          `PathSourcePath()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                   Method                                                                   Description
          ----------------------------------- ------------------------------------------------------------------------ -------------
          `int`                               `compareTo​(SourcePath other)`                                             
          `boolean`                           `equals​(Object other)`                                                    
          `static Optional<PathSourcePath>`   `from​(SourcePath sourcePath)`                                             
          `abstract ProjectFilesystem`        `getFilesystem()`                                                         
          `abstract Path`                     `getRelativePath()`                                                       
          `int`                               `hashCode()`                                                              
          `static PathSourcePath`             `of​(ProjectFilesystem filesystem,   RelPath relativePath)`                
          `static PathSourcePath`             `of​(ProjectFilesystem filesystem,   ForwardRelativePath relativePath)`    
          `static PathSourcePath`             `of​(ProjectFilesystem filesystem,   Path relativePath)`                   
          `String`                            `toString()`                                                              

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.sourcepath.SourcePath}

            ### Methods inherited from interface com.facebook.buck.core.sourcepath.[SourcePath](SourcePath.html "interface in com.facebook.buck.core.sourcepath")

            `compareClasses`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### PathSourcePath

                public PathSourcePath()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getFilesystem()}

        -   #### getFilesystem

            ``` methodSignature
            public abstract ProjectFilesystem getFilesystem()
            ```

        []{#getRelativePath()}

        -   #### getRelativePath

            ``` methodSignature
            public abstract Path getRelativePath()
            ```

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `Object`

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(Object other)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `Object`

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

        []{#compareTo(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### compareTo

            ``` methodSignature
            public int compareTo​(SourcePath other)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `compareTo` in interface `Comparable<SourcePath>`

        []{#of(com.facebook.buck.io.filesystem.ProjectFilesystem,java.nio.file.Path)}

        -   #### of

            ``` methodSignature
            public static PathSourcePath of​(ProjectFilesystem filesystem,
                                            Path relativePath)
            ```

        []{#of(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.path.ForwardRelativePath)}

        -   #### of

            ``` methodSignature
            public static PathSourcePath of​(ProjectFilesystem filesystem,
                                            ForwardRelativePath relativePath)
            ```

        []{#of(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.filesystems.RelPath)}

        -   #### of

            ``` methodSignature
            public static PathSourcePath of​(ProjectFilesystem filesystem,
                                            RelPath relativePath)
            ```

        []{#from(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### from

            ``` methodSignature
            public static Optional<PathSourcePath> from​(SourcePath sourcePath)
            ```

            [Returns:]{.returnLabel}
            :   the
                [`PathSourcePath`](PathSourcePath.html "class in com.facebook.buck.core.sourcepath")
                backing the given
                [`SourcePath`](SourcePath.html "interface in com.facebook.buck.core.sourcepath"),
                if any.
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

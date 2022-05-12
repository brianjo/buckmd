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
[Package]{.packageLabelInType} [com.facebook.buck.apple.xcode.xcodeproj](package-summary.html)
:::

## Class SourceTreePath {#class-sourcetreepath .title title="Class SourceTreePath"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.xcode.xcodeproj.SourceTreePath

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`, `Comparable<SourceTreePath>`

    ------------------------------------------------------------------------

        public class SourceTreePath
        extends Object
        implements Comparable<SourceTreePath>, AddsToRuleKey

    ::: block
    Utility class representing a tuple of (SourceTree, Path) used for
    uniquely describing a file reference in a group.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                 Description
          --------------------------------------------------------------------------------------------------------------------------- -------------
          `SourceTreePath​(PBXReference.SourceTree sourceTree,               Path path,               Optional<String> defaultType)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type           Method                                                                                          Description
          --------------------------- ----------------------------------------------------------------------------------------------- -------------
          `int`                       `compareTo​(SourceTreePath o)`                                                                    
          `PBXFileReference`          `createFileReference​(AbstractPBXObjectFactory objectFactory)`                                    
          `PBXFileReference`          `createFileReference​(String name,                    AbstractPBXObjectFactory objectFactory)`    
          `XCVersionGroup`            `createVersionGroup​(AbstractPBXObjectFactory objectFactory)`                                     
          `boolean`                   `equals​(Object other)`                                                                           
          `Path`                      `getPath()`                                                                                      
          `PBXReference.SourceTree`   `getSourceTree()`                                                                                
          `int`                       `hashCode()`                                                                                     
          `String`                    `toString()`                                                                                     

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.apple.xcode.xcodeproj.PBXReference.SourceTree,java.nio.file.Path,java.util.Optional)}

        -   #### SourceTreePath

                public SourceTreePath​(PBXReference.SourceTree sourceTree,
                                      Path path,
                                      Optional<String> defaultType)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getSourceTree()}

        -   #### getSourceTree

            ``` methodSignature
            public PBXReference.SourceTree getSourceTree()
            ```

        []{#getPath()}

        -   #### getPath

            ``` methodSignature
            public Path getPath()
            ```

        []{#createFileReference(java.lang.String,com.facebook.buck.apple.xcode.AbstractPBXObjectFactory)}

        -   #### createFileReference

            ``` methodSignature
            public PBXFileReference createFileReference​(String name,
                                                        AbstractPBXObjectFactory objectFactory)
            ```

        []{#createFileReference(com.facebook.buck.apple.xcode.AbstractPBXObjectFactory)}

        -   #### createFileReference

            ``` methodSignature
            public PBXFileReference createFileReference​(AbstractPBXObjectFactory objectFactory)
            ```

        []{#createVersionGroup(com.facebook.buck.apple.xcode.AbstractPBXObjectFactory)}

        -   #### createVersionGroup

            ``` methodSignature
            public XCVersionGroup createVersionGroup​(AbstractPBXObjectFactory objectFactory)
            ```

        []{#compareTo(com.facebook.buck.apple.xcode.xcodeproj.SourceTreePath)}

        -   #### compareTo

            ``` methodSignature
            public int compareTo​(SourceTreePath o)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `compareTo` in interface `Comparable<SourceTreePath>`

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
            public boolean equals​(@Nullable
                                  Object other)
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

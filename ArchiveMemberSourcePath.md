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

## Class ArchiveMemberSourcePath {#class-archivemembersourcepath .title title="Class ArchiveMemberSourcePath"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.sourcepath.ArchiveMemberSourcePath

::: description
-   

    All Implemented Interfaces:
    :   `SourcePath`, `Comparable<SourcePath>`

    ------------------------------------------------------------------------

        public abstract class ArchiveMemberSourcePath
        extends Object
        implements SourcePath

    ::: block
    A
    [`SourcePath`](SourcePath.html "interface in com.facebook.buck.core.sourcepath")
    that can reference a member within an archive.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                   Description
          ----------------------------- -------------
          `ArchiveMemberSourcePath()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                  Method                                                  Description
          ---------------------------------- ------------------------------------------------------- -------------
          `void`                             `check()`                                                
          `int`                              `compareTo​(SourcePath other)`                            
          `abstract SourcePath`              `getArchiveSourcePath()`                                 
          `abstract Path`                    `getMemberPath()`                                        
          `static ArchiveMemberSourcePath`   `of​(SourcePath archiveSourcePath,   Path memberPath)`    

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

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

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

        -   #### ArchiveMemberSourcePath

                public ArchiveMemberSourcePath()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#of(com.facebook.buck.core.sourcepath.SourcePath,java.nio.file.Path)}

        -   #### of

            ``` methodSignature
            public static ArchiveMemberSourcePath of​(SourcePath archiveSourcePath,
                                                     Path memberPath)
            ```

        []{#getArchiveSourcePath()}

        -   #### getArchiveSourcePath

            ``` methodSignature
            public abstract SourcePath getArchiveSourcePath()
            ```

        []{#getMemberPath()}

        -   #### getMemberPath

            ``` methodSignature
            public abstract Path getMemberPath()
            ```

        []{#check()}

        -   #### check

            ``` methodSignature
            @Check
            public void check()
            ```

        []{#compareTo(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### compareTo

            ``` methodSignature
            public int compareTo​(SourcePath other)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `compareTo` in interface `Comparable<SourcePath>`
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

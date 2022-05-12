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
[Package]{.packageLabelInType} [com.facebook.buck.util.hashing](package-summary.html)
:::

## Class FilePathHashLoader {#class-filepathhashloader .title title="Class FilePathHashLoader"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.hashing.FilePathHashLoader

::: description
-   

    All Implemented Interfaces:
    :   `FileHashLoader`

    ------------------------------------------------------------------------

        public class FilePathHashLoader
        extends Object
        implements FileHashLoader

    ::: block
    A
    [`FileHashLoader`](FileHashLoader.html "interface in com.facebook.buck.util.hashing")
    that only hashes the files\' paths without reading their contents.
    If file\'s hash needs to be changed, for example to reflect changes
    to the file\'s contents, the file\'s path can be specified in a set
    of modified files. Files specified in this set will get new unique
    hashes based on their paths distinct from the hashes they would get
    if they were omitted from the set.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                               Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `FilePathHashLoader​(Path defaultCellRoot,                   com.google.common.collect.ImmutableSet<Path> assumeModifiedFiles,                   boolean allowSymlinks)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                   Method                                                                                Description
          ----------------------------------- ------------------------------------------------------------------------------------- -------------
          `com.google.common.hash.HashCode`   `get​(Path root)`                                                                       
          `com.google.common.hash.HashCode`   `getForArchiveMember​(Path relativeArchivePath,                    Path memberPath)`    
          `long`                              `getSize​(Path path)`                                                                   

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.util.hashing.FileHashLoader}

            ### Methods inherited from interface com.facebook.buck.util.hashing.[FileHashLoader](FileHashLoader.html "interface in com.facebook.buck.util.hashing")

            `get, getForArchiveMember, getSize`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.nio.file.Path,com.google.common.collect.ImmutableSet,boolean)}

        -   #### FilePathHashLoader

                public FilePathHashLoader​(Path defaultCellRoot,
                                          com.google.common.collect.ImmutableSet<Path> assumeModifiedFiles,
                                          boolean allowSymlinks)
                                   throws IOException

            [Throws:]{.throwsLabel}
            :   `IOException`
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#get(java.nio.file.Path)}

        -   #### get

            ``` methodSignature
            public com.google.common.hash.HashCode get​(Path root)
                                                throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `get` in interface `FileHashLoader`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getSize(java.nio.file.Path)}

        -   #### getSize

            ``` methodSignature
            public long getSize​(Path path)
                         throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSize` in interface `FileHashLoader`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getForArchiveMember(java.nio.file.Path,java.nio.file.Path)}

        -   #### getForArchiveMember

            ``` methodSignature
            public com.google.common.hash.HashCode getForArchiveMember​(Path relativeArchivePath,
                                                                       Path memberPath)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getForArchiveMember` in interface `FileHashLoader`
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

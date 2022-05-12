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

-   [Overview](../../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../../index-all.html)
-   [Help](../../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../../allclasses.html)

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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.features.project.intellij.model.folders](package-summary.html)
:::

## Class IjFolder {#class-ijfolder .title title="Class IjFolder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.project.intellij.model.folders.IjFolder

::: description
-   

    All Implemented Interfaces:
    :   `Comparable<IjFolder>`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `ExcludeFolder`, `InclusiveFolder`

    ------------------------------------------------------------------------

        public abstract class IjFolder
        extends Object
        implements Comparable<IjFolder>

    ::: block
    A path which contains a set of sources we wish to present to
    IntelliJ.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `boolean`             | `canMerge             |                       |
        |                       | With​(IjFolder other)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static com.googl     | `combineInputs​(IjFo   |                       |
        | e.common.collect.Immu | lder first,           |                       |
        | tableSortedSet<Path>` |     IjFolder second)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `compa                |                       |
        |                       | reTo​(IjFolder other)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `IjFolder`            | `creat                | ::: block             |
        |                       | eCopyWith​(Path path)` | Create a copy of this |
        |                       |                       | folder using the      |
        |                       |                       | specified path.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `                     |                       |
        |                       | equals​(Object other)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected abst       | `getFactory()`        |                       |
        | ract IJFolderFactory` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract String`     | `getIjName()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `getInputs()`         |                       |
        | e.common.collect.Immu |                       |                       |
        | tableSortedSet<Path>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getPath()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `get                  | ::: block             |
        |                       | WantsPackagePrefix()` | Used to make IntelliJ |
        |                       |                       | ignore the package    |
        |                       |                       | name-\>folder         |
        |                       |                       | structure convention  |
        |                       |                       | and assume the given  |
        |                       |                       | package prefix.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isResourceFolder()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `IjFolder`            | `merge​(I              |                       |
        |                       | jFolder otherFolder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          |                       |
        +-----------------------+-----------------------+-----------------------+

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
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getIjName()}

        -   #### getIjName

            ``` methodSignature
            public abstract String getIjName()
            ```

            [Returns:]{.returnLabel}
            :   name IntelliJ would use to refer to this type of folder.

        []{#getPath()}

        -   #### getPath

            ``` methodSignature
            public Path getPath()
            ```

            [Returns:]{.returnLabel}
            :   path that this folder represents relative to the project
                root.

        []{#getInputs()}

        -   #### getInputs

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<Path> getInputs()
            ```

            [Returns:]{.returnLabel}
            :   set of input files corresponding to this folder.

        []{#getFactory()}

        -   #### getFactory

            ``` methodSignature
            protected abstract IJFolderFactory getFactory()
            ```

            [Returns:]{.returnLabel}
            :   a IJFolderFactory to create new instances of the folder
                class.

        []{#createCopyWith(java.nio.file.Path)}

        -   #### createCopyWith

            ``` methodSignature
            public IjFolder createCopyWith​(Path path)
            ```

            ::: block
            Create a copy of this folder using the specified path.
            :::

            [Returns:]{.returnLabel}
            :   a copy of this object with the new path

        []{#isResourceFolder()}

        -   #### isResourceFolder

            ``` methodSignature
            public boolean isResourceFolder()
            ```

            [Returns:]{.returnLabel}
            :   true if it should be marked as a java-resource or
                java-test-resource folder, false otherwise.

        []{#getWantsPackagePrefix()}

        -   #### getWantsPackagePrefix

            ``` methodSignature
            public boolean getWantsPackagePrefix()
            ```

            ::: block
            Used to make IntelliJ ignore the package name-\>folder
            structure convention and assume the given package prefix. An
            example of a scenario this makes possible to achieve is
            having java/src/Foo.java declare the package \"org.bar\"
            (instead of having the path to the file be
            java/org/bar/Foo.java). The main effect of this is the
            elimination of IntelliJ warnings about incorrect package
            prefixes and having it use the correct package when creating
            new files.
            :::

            [Returns:]{.returnLabel}
            :   whether to generate package prefix for this folder.

        []{#canMergeWith(com.facebook.buck.features.project.intellij.model.folders.IjFolder)}

        -   #### canMergeWith

            ``` methodSignature
            public boolean canMergeWith​(IjFolder other)
            ```

        []{#merge(com.facebook.buck.features.project.intellij.model.folders.IjFolder)}

        -   #### merge

            ``` methodSignature
            public IjFolder merge​(IjFolder otherFolder)
            ```

        []{#compareTo(com.facebook.buck.features.project.intellij.model.folders.IjFolder)}

        -   #### compareTo

            ``` methodSignature
            public int compareTo​(IjFolder other)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `compareTo` in interface `Comparable<IjFolder>`

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(Object other)
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

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

        []{#combineInputs(com.facebook.buck.features.project.intellij.model.folders.IjFolder,com.facebook.buck.features.project.intellij.model.folders.IjFolder)}

        -   #### combineInputs

            ``` methodSignature
            public static com.google.common.collect.ImmutableSortedSet<Path> combineInputs​(IjFolder first,
                                                                                           IjFolder second)
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

-   [Overview](../../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../../index-all.html)
-   [Help](../../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

<div>

-   Summary: 
-   Nested \| 
-   Field \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

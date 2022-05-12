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
[Package]{.packageLabelInType} [com.facebook.buck.features.project.intellij.model.folders](package-summary.html)
:::

## Class IjSourceFolder {#class-ijsourcefolder .title title="Class IjSourceFolder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.project.intellij.model.folders.IjSourceFolder

::: description
-   

    All Implemented Interfaces:
    :   `Comparable<IjSourceFolder>`

    ------------------------------------------------------------------------

        public abstract class IjSourceFolder
        extends Object
        implements Comparable<IjSourceFolder>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor          Description
          -------------------- -------------
          `IjSourceFolder()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                                            Method                                                                                                                                                                                             Description
          -------------------------------------------------------------------------------------------- -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `int`                                                                                        `compareTo​(IjSourceFolder o)`                                                                                                                                                                       
          `abstract IjResourceFolderType`                                                              `getIjResourceFolderType()`                                                                                                                                                                         
          `abstract boolean`                                                                           `getIsResourceFolder()`                                                                                                                                                                             
          `abstract boolean`                                                                           `getIsTestSource()`                                                                                                                                                                                 
          `abstract String`                                                                            `getPackagePrefix()`                                                                                                                                                                                
          `abstract Path`                                                                              `getPath()`                                                                                                                                                                                         
          `abstract Path`                                                                              `getRelativeOutputPath()`                                                                                                                                                                           
          `abstract String`                                                                            `getType()`                                                                                                                                                                                         
          `abstract String`                                                                            `getUrl()`                                                                                                                                                                                          
          `static com.facebook.buck.features.project.intellij.model.folders.ImmutableIjSourceFolder`   `of​(String type,   String url,   Path path,   boolean isTestSource,   boolean isResourceFolder,   IjResourceFolderType ijResourceFolderType,   Path relativeOutputPath,   String packagePrefix)`    

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
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### IjSourceFolder

                public IjSourceFolder()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getType()}

        -   #### getType

            ``` methodSignature
            public abstract String getType()
            ```

        []{#getUrl()}

        -   #### getUrl

            ``` methodSignature
            public abstract String getUrl()
            ```

        []{#getPath()}

        -   #### getPath

            ``` methodSignature
            public abstract Path getPath()
            ```

        []{#getIsTestSource()}

        -   #### getIsTestSource

            ``` methodSignature
            public abstract boolean getIsTestSource()
            ```

        []{#getIsResourceFolder()}

        -   #### getIsResourceFolder

            ``` methodSignature
            public abstract boolean getIsResourceFolder()
            ```

        []{#getIjResourceFolderType()}

        -   #### getIjResourceFolderType

            ``` methodSignature
            public abstract IjResourceFolderType getIjResourceFolderType()
            ```

        []{#getRelativeOutputPath()}

        -   #### getRelativeOutputPath

            ``` methodSignature
            @Nullable
            public abstract Path getRelativeOutputPath()
            ```

        []{#getPackagePrefix()}

        -   #### getPackagePrefix

            ``` methodSignature
            @Nullable
            public abstract String getPackagePrefix()
            ```

        []{#compareTo(com.facebook.buck.features.project.intellij.model.folders.IjSourceFolder)}

        -   #### compareTo

            ``` methodSignature
            public int compareTo​(IjSourceFolder o)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `compareTo` in interface `Comparable<IjSourceFolder>`

        []{#of(java.lang.String,java.lang.String,java.nio.file.Path,boolean,boolean,com.facebook.buck.features.project.intellij.model.folders.IjResourceFolderType,java.nio.file.Path,java.lang.String)}

        -   #### of

            ``` methodSignature
            public static com.facebook.buck.features.project.intellij.model.folders.ImmutableIjSourceFolder of​(String type,
                                                                                                               String url,
                                                                                                               Path path,
                                                                                                               boolean isTestSource,
                                                                                                               boolean isResourceFolder,
                                                                                                               IjResourceFolderType ijResourceFolderType,
                                                                                                               @Nullable
                                                                                                               Path relativeOutputPath,
                                                                                                               @Nullable
                                                                                                               String packagePrefix)
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

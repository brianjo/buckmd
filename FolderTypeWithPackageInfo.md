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
-   [Enum Constants](#enum.constant.summary) \| 
-   Field \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Enum Constants](#enum.constant.detail) \| 
-   Field \| 
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

## Enum FolderTypeWithPackageInfo {#enum-foldertypewithpackageinfo .title title="Enum FolderTypeWithPackageInfo"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<[FolderTypeWithPackageInfo](FolderTypeWithPackageInfo.html "enum in com.facebook.buck.features.project.intellij")\>

    -   -   com.facebook.buck.features.project.intellij.FolderTypeWithPackageInfo

::: description
-   

    All Implemented Interfaces:
    :   `Serializable`, `Comparable<FolderTypeWithPackageInfo>`

    ------------------------------------------------------------------------

        public enum FolderTypeWithPackageInfo
        extends Enum<FolderTypeWithPackageInfo>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#enum.constant.summary}

        ### Enum Constant Summary

          Enum Constant                          Description
          -------------------------------------- -------------
          `JAVA_RESOURCE_FOLDER`                  
          `JAVA_TEST_RESOURCE_FOLDER`             
          `SOURCE_FOLDER_WITH_PACKAGE_INFO`       
          `SOURCE_FOLDER_WITHOUT_PACKAGE_INFO`    
          `TEST_FOLDER_WITH_PACKAGE_INFO`         
          `TEST_FOLDER_WITHOUT_PACKAGE_INFO`      

          : Enum Constants[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static Folde         | `fromFol              |                       |
        | rTypeWithPackageInfo` | der​(IjFolder folder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `IJFolderFactory`     | `getFolderFactory()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Class                | `                     |                       |
        | <? extends IjFolder>` | getFolderTypeClass()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getIj                |                       |
        | IjResourceFolderType` | ResourceFolderType()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `R                    | `getRes               |                       |
        | esourceFolderFactory` | ourceFolderFactory()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isResourceFolder()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Folde         | `                     | ::: block             |
        | rTypeWithPackageInfo` | valueOf​(String name)` | Returns the enum      |
        |                       |                       | constant of this type |
        |                       |                       | with the specified    |
        |                       |                       | name.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static FolderT       | `values()`            | ::: block             |
        | ypeWithPackageInfo[]` |                       | Returns an array      |
        |                       |                       | containing the        |
        |                       |                       | constants of this     |
        |                       |                       | enum type, in the     |
        |                       |                       | order they are        |
        |                       |                       | declared.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `                     |                       |
        |                       | wantsPackagePrefix()` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Enum}

            ### Methods inherited from class java.lang.[Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, compareTo, equals, finalize, getDeclaringClass, hashCode, name, ordinal, toString, valueOf`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `getClass, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#enum.constant.detail}

        ### Enum Constant Detail

        []{#SOURCE_FOLDER_WITH_PACKAGE_INFO}

        -   #### SOURCE_FOLDER_WITH_PACKAGE_INFO

                public static final FolderTypeWithPackageInfo SOURCE_FOLDER_WITH_PACKAGE_INFO

        []{#SOURCE_FOLDER_WITHOUT_PACKAGE_INFO}

        -   #### SOURCE_FOLDER_WITHOUT_PACKAGE_INFO

                public static final FolderTypeWithPackageInfo SOURCE_FOLDER_WITHOUT_PACKAGE_INFO

        []{#TEST_FOLDER_WITH_PACKAGE_INFO}

        -   #### TEST_FOLDER_WITH_PACKAGE_INFO

                public static final FolderTypeWithPackageInfo TEST_FOLDER_WITH_PACKAGE_INFO

        []{#TEST_FOLDER_WITHOUT_PACKAGE_INFO}

        -   #### TEST_FOLDER_WITHOUT_PACKAGE_INFO

                public static final FolderTypeWithPackageInfo TEST_FOLDER_WITHOUT_PACKAGE_INFO

        []{#JAVA_RESOURCE_FOLDER}

        -   #### JAVA_RESOURCE_FOLDER

                public static final FolderTypeWithPackageInfo JAVA_RESOURCE_FOLDER

        []{#JAVA_TEST_RESOURCE_FOLDER}

        -   #### JAVA_TEST_RESOURCE_FOLDER

                public static final FolderTypeWithPackageInfo JAVA_TEST_RESOURCE_FOLDER
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#values()}

        -   #### values

            ``` methodSignature
            public static FolderTypeWithPackageInfo[] values()
            ```

            ::: block
            Returns an array containing the constants of this enum type,
            in the order they are declared. This method may be used to
            iterate over the constants as follows:
                for (FolderTypeWithPackageInfo c : FolderTypeWithPackageInfo.values())
                    System.out.println(c);
            :::

            [Returns:]{.returnLabel}
            :   an array containing the constants of this enum type, in
                the order they are declared

        []{#valueOf(java.lang.String)}

        -   #### valueOf

            ``` methodSignature
            public static FolderTypeWithPackageInfo valueOf​(String name)
            ```

            ::: block
            Returns the enum constant of this type with the specified
            name. The string must match *exactly* an identifier used to
            declare an enum constant in this type. (Extraneous
            whitespace characters are not permitted.)
            :::

            [Parameters:]{.paramLabel}
            :   `name` - the name of the enum constant to be returned.

            [Returns:]{.returnLabel}
            :   the enum constant with the specified name

            [Throws:]{.throwsLabel}
            :   `IllegalArgumentException` - if this enum type has no
                constant with the specified name
            :   `NullPointerException` - if the argument is null

        []{#fromFolder(com.facebook.buck.features.project.intellij.model.folders.IjFolder)}

        -   #### fromFolder

            ``` methodSignature
            public static FolderTypeWithPackageInfo fromFolder​(IjFolder folder)
            ```

        []{#getFolderFactory()}

        -   #### getFolderFactory

            ``` methodSignature
            public IJFolderFactory getFolderFactory()
            ```

        []{#getFolderTypeClass()}

        -   #### getFolderTypeClass

            ``` methodSignature
            public Class<? extends IjFolder> getFolderTypeClass()
            ```

        []{#wantsPackagePrefix()}

        -   #### wantsPackagePrefix

            ``` methodSignature
            public boolean wantsPackagePrefix()
            ```

        []{#getResourceFolderFactory()}

        -   #### getResourceFolderFactory

            ``` methodSignature
            public ResourceFolderFactory getResourceFolderFactory()
            ```

        []{#isResourceFolder()}

        -   #### isResourceFolder

            ``` methodSignature
            public boolean isResourceFolder()
            ```

        []{#getIjResourceFolderType()}

        -   #### getIjResourceFolderType

            ``` methodSignature
            public IjResourceFolderType getIjResourceFolderType()
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
-   [Enum Constants](#enum.constant.summary) \| 
-   Field \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Enum Constants](#enum.constant.detail) \| 
-   Field \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

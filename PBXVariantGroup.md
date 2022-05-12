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
-   [Nested](#nested.class.summary) \| 
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

## Class PBXVariantGroup {#class-pbxvariantgroup .title title="Class PBXVariantGroup"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.apple.xcode.xcodeproj.PBXObject](PBXObject.html "class in com.facebook.buck.apple.xcode.xcodeproj")

    -   -   [com.facebook.buck.apple.xcode.xcodeproj.PBXContainerItem](PBXContainerItem.html "class in com.facebook.buck.apple.xcode.xcodeproj")

        -   -   [com.facebook.buck.apple.xcode.xcodeproj.PBXReference](PBXReference.html "class in com.facebook.buck.apple.xcode.xcodeproj")

            -   -   [com.facebook.buck.apple.xcode.xcodeproj.PBXGroup](PBXGroup.html "class in com.facebook.buck.apple.xcode.xcodeproj")

                -   -   com.facebook.buck.apple.xcode.xcodeproj.PBXVariantGroup

::: description
-   

    ------------------------------------------------------------------------

        public final class PBXVariantGroup
        extends PBXGroup

    ::: block
    Group for referencing localized resources.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.apple.xcode.xcodeproj.PBXGroup}

            ### Nested classes/interfaces inherited from class com.facebook.buck.apple.xcode.xcodeproj.[PBXGroup](PBXGroup.html "class in com.facebook.buck.apple.xcode.xcodeproj")

            `PBXGroup.SortPolicy`

        ```{=html}
        <!-- -->
        ```
        -   []{#nested.classes.inherited.from.class.com.facebook.buck.apple.xcode.xcodeproj.PBXReference}

            ### Nested classes/interfaces inherited from class com.facebook.buck.apple.xcode.xcodeproj.[PBXReference](PBXReference.html "class in com.facebook.buck.apple.xcode.xcodeproj")

            `PBXReference.SourceTree`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                            Description
          ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `PBXVariantGroup​(String name,                String path,                PBXReference.SourceTree sourceTree,                AbstractPBXObjectFactory objectFactory)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type    Method                                                                                                                                                              Description
          -------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `PBXFileReference`   `getOrCreateVariantFileReferenceByNameAndSourceTreePath​(String virtualName,                                                       SourceTreePath sourceTreePath)`    
          `String`             `isa()`                                                                                                                                                              

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.apple.xcode.xcodeproj.PBXGroup}

            ### Methods inherited from class com.facebook.buck.apple.xcode.xcodeproj.[PBXGroup](PBXGroup.html "class in com.facebook.buck.apple.xcode.xcodeproj")

            `getChildren, getOrCreateChildGroupByName, getOrCreateChildVariantGroupByName, getOrCreateChildVersionGroupsBySourceTreePath, getOrCreateDescendantGroupByPath, getOrCreateFileReferenceBySourceTreePath, serializeInto, setSortPolicy`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.apple.xcode.xcodeproj.PBXReference}

            ### Methods inherited from class com.facebook.buck.apple.xcode.xcodeproj.[PBXReference](PBXReference.html "class in com.facebook.buck.apple.xcode.xcodeproj")

            `getName, getPath, getSourceTree, setPath, setSourceTree, stableHash, toString`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.apple.xcode.xcodeproj.PBXObject}

            ### Methods inherited from class com.facebook.buck.apple.xcode.xcodeproj.[PBXObject](PBXObject.html "class in com.facebook.buck.apple.xcode.xcodeproj")

            `generateGid, getGlobalID, setGlobalID`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.lang.String,java.lang.String,com.facebook.buck.apple.xcode.xcodeproj.PBXReference.SourceTree,com.facebook.buck.apple.xcode.AbstractPBXObjectFactory)}

        -   #### PBXVariantGroup

                public PBXVariantGroup​(String name,
                                       @Nullable
                                       String path,
                                       PBXReference.SourceTree sourceTree,
                                       AbstractPBXObjectFactory objectFactory)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getOrCreateVariantFileReferenceByNameAndSourceTreePath(java.lang.String,com.facebook.buck.apple.xcode.xcodeproj.SourceTreePath)}

        -   #### getOrCreateVariantFileReferenceByNameAndSourceTreePath

            ``` methodSignature
            public PBXFileReference getOrCreateVariantFileReferenceByNameAndSourceTreePath​(String virtualName,
                                                                                           SourceTreePath sourceTreePath)
            ```

        []{#isa()}

        -   #### isa

            ``` methodSignature
            public String isa()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `isa` in class `PBXGroup`

            [Returns:]{.returnLabel}
            :   Type name of the serialized object.
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
-   [Nested](#nested.class.summary) \| 
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

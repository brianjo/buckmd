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

## Class PBXGroup {#class-pbxgroup .title title="Class PBXGroup"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.apple.xcode.xcodeproj.PBXObject](PBXObject.html "class in com.facebook.buck.apple.xcode.xcodeproj")

    -   -   [com.facebook.buck.apple.xcode.xcodeproj.PBXContainerItem](PBXContainerItem.html "class in com.facebook.buck.apple.xcode.xcodeproj")

        -   -   [com.facebook.buck.apple.xcode.xcodeproj.PBXReference](PBXReference.html "class in com.facebook.buck.apple.xcode.xcodeproj")

            -   -   com.facebook.buck.apple.xcode.xcodeproj.PBXGroup

::: description
-   

    Direct Known Subclasses:
    :   `PBXVariantGroup`

    ------------------------------------------------------------------------

        public class PBXGroup
        extends PBXReference

    ::: block
    A collection of files in Xcode\'s virtual filesystem hierarchy.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `PBXGroup.SortPolicy` | ::: block             |
        |                       |                       | Method by which group |
        |                       |                       | contents will be      |
        |                       |                       | sorted.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.apple.xcode.xcodeproj.PBXReference}

            ### Nested classes/interfaces inherited from class com.facebook.buck.apple.xcode.xcodeproj.[PBXReference](PBXReference.html "class in com.facebook.buck.apple.xcode.xcodeproj")

            `PBXReference.SourceTree`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                Description
          ------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `PBXGroup​(String name,         String path,         PBXReference.SourceTree sourceTree,         AbstractPBXObjectFactory objectFactory)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `List<PBXReference>`  | `getChildren()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `PBXGroup`            | `getOrCreateChildGrou |                       |
        |                       | pByName​(String name)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `PBXVariantGroup`     | `getOrC               |                       |
        |                       | reateChildVariantGrou |                       |
        |                       | pByName​(String name)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `XCVersionGroup`      | `getOrCreateChi       |                       |
        |                       | ldVersionGroupsBySour |                       |
        |                       | ceTreePath​(SourceTree |                       |
        |                       | Path sourceTreePath)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `PBXGroup`            | `get                  |                       |
        |                       | OrCreateDescendantGro |                       |
        |                       | upByPath​(com.google.c |                       |
        |                       | ommon.collect.Immutab |                       |
        |                       | leList<String> path)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `PBXFileReference`    | `getOrCrea            |                       |
        |                       | teFileReferenceBySour |                       |
        |                       | ceTreePath​(SourceTree |                       |
        |                       | Path sourceTreePath)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `isa()`               |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `serializeInto​(Xc     | ::: block             |
        |                       | odeprojSerializer s)` | Populates the         |
        |                       |                       | serializer with the   |
        |                       |                       | fields of this        |
        |                       |                       | object.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `setS                 |                       |
        |                       | ortPolicy​(PBXGroup.So |                       |
        |                       | rtPolicy sortPolicy)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

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

        -   #### PBXGroup

                public PBXGroup​(String name,
                                @Nullable
                                String path,
                                PBXReference.SourceTree sourceTree,
                                AbstractPBXObjectFactory objectFactory)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getOrCreateChildGroupByName(java.lang.String)}

        -   #### getOrCreateChildGroupByName

            ``` methodSignature
            public PBXGroup getOrCreateChildGroupByName​(String name)
            ```

        []{#getOrCreateDescendantGroupByPath(com.google.common.collect.ImmutableList)}

        -   #### getOrCreateDescendantGroupByPath

            ``` methodSignature
            public PBXGroup getOrCreateDescendantGroupByPath​(com.google.common.collect.ImmutableList<String> path)
            ```

        []{#getOrCreateChildVariantGroupByName(java.lang.String)}

        -   #### getOrCreateChildVariantGroupByName

            ``` methodSignature
            public PBXVariantGroup getOrCreateChildVariantGroupByName​(String name)
            ```

        []{#getOrCreateFileReferenceBySourceTreePath(com.facebook.buck.apple.xcode.xcodeproj.SourceTreePath)}

        -   #### getOrCreateFileReferenceBySourceTreePath

            ``` methodSignature
            public PBXFileReference getOrCreateFileReferenceBySourceTreePath​(SourceTreePath sourceTreePath)
            ```

        []{#getOrCreateChildVersionGroupsBySourceTreePath(com.facebook.buck.apple.xcode.xcodeproj.SourceTreePath)}

        -   #### getOrCreateChildVersionGroupsBySourceTreePath

            ``` methodSignature
            public XCVersionGroup getOrCreateChildVersionGroupsBySourceTreePath​(SourceTreePath sourceTreePath)
            ```

        []{#getChildren()}

        -   #### getChildren

            ``` methodSignature
            public List<PBXReference> getChildren()
            ```

        []{#setSortPolicy(com.facebook.buck.apple.xcode.xcodeproj.PBXGroup.SortPolicy)}

        -   #### setSortPolicy

            ``` methodSignature
            public void setSortPolicy​(PBXGroup.SortPolicy sortPolicy)
            ```

        []{#isa()}

        -   #### isa

            ``` methodSignature
            public String isa()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `isa` in class `PBXReference`

            [Returns:]{.returnLabel}
            :   Type name of the serialized object.

        []{#serializeInto(com.facebook.buck.apple.xcode.XcodeprojSerializer)}

        -   #### serializeInto

            ``` methodSignature
            public void serializeInto​(XcodeprojSerializer s)
            ```

            ::: block
            [Description copied from
            class: `PBXObject`]{.descfrmTypeLabel}
            :::

            ::: block
            Populates the serializer with the fields of this object.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `serializeInto` in class `PBXReference`
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

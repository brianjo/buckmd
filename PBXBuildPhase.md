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

## Class PBXBuildPhase {#class-pbxbuildphase .title title="Class PBXBuildPhase"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.apple.xcode.xcodeproj.PBXObject](PBXObject.html "class in com.facebook.buck.apple.xcode.xcodeproj")

    -   -   [com.facebook.buck.apple.xcode.xcodeproj.PBXContainerItem](PBXContainerItem.html "class in com.facebook.buck.apple.xcode.xcodeproj")

        -   -   [com.facebook.buck.apple.xcode.xcodeproj.PBXProjectItem](PBXProjectItem.html "class in com.facebook.buck.apple.xcode.xcodeproj")

            -   -   com.facebook.buck.apple.xcode.xcodeproj.PBXBuildPhase

::: description
-   

    Direct Known Subclasses:
    :   `PBXCopyFilesBuildPhase`, `PBXFrameworksBuildPhase`,
        `PBXHeadersBuildPhase`, `PBXResourcesBuildPhase`,
        `PBXShellScriptBuildPhase`, `PBXSourcesBuildPhase`

    ------------------------------------------------------------------------

        public abstract class PBXBuildPhase
        extends PBXProjectItem

    ::: block
    Superclass of build phases. Each build phase represents one step in
    building a target.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor         Description
          ------------------- -------------
          `PBXBuildPhase()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `List<PBXBuildFile>`  | `getFiles()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getName()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `serializeInto​(Xc     | ::: block             |
        |                       | odeprojSerializer s)` | Populates the         |
        |                       |                       | serializer with the   |
        |                       |                       | fields of this        |
        |                       |                       | object.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `setName​(Op           |                       |
        |                       | tional<String> name)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `setRunOnlyForDe      |                       |
        |                       | ploymentPostprocessin |                       |
        |                       | g​(Optional<Boolean> r |                       |
        |                       | unOnlyForDeployment)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.apple.xcode.xcodeproj.PBXProjectItem}

            ### Methods inherited from class com.facebook.buck.apple.xcode.xcodeproj.[PBXProjectItem](PBXProjectItem.html "class in com.facebook.buck.apple.xcode.xcodeproj")

            `isa`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.apple.xcode.xcodeproj.PBXObject}

            ### Methods inherited from class com.facebook.buck.apple.xcode.xcodeproj.[PBXObject](PBXObject.html "class in com.facebook.buck.apple.xcode.xcodeproj")

            `generateGid, getGlobalID, setGlobalID, stableHash, toString`

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

        []{#<init>()}

        -   #### PBXBuildPhase

                public PBXBuildPhase()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getFiles()}

        -   #### getFiles

            ``` methodSignature
            public List<PBXBuildFile> getFiles()
            ```

        []{#setRunOnlyForDeploymentPostprocessing(java.util.Optional)}

        -   #### setRunOnlyForDeploymentPostprocessing

            ``` methodSignature
            public void setRunOnlyForDeploymentPostprocessing​(Optional<Boolean> runOnlyForDeployment)
            ```

        []{#setName(java.util.Optional)}

        -   #### setName

            ``` methodSignature
            public void setName​(Optional<String> name)
            ```

        []{#getName()}

        -   #### getName

            ``` methodSignature
            public Optional<String> getName()
            ```

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
            :   `serializeInto` in class `PBXContainerItem`
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

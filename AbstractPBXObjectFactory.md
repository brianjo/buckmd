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
[Package]{.packageLabelInType} [com.facebook.buck.apple.xcode](package-summary.html)
:::

## Class AbstractPBXObjectFactory {#class-abstractpbxobjectfactory .title title="Class AbstractPBXObjectFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.xcode.AbstractPBXObjectFactory

::: description
-   

    Direct Known Subclasses:
    :   `PBXObjectGIDFactory`

    ------------------------------------------------------------------------

        public abstract class AbstractPBXObjectFactory
        extends Object

    ::: block
    A factory object for generating new PBX object types.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                    Description
          ------------------------------ -------------
          `AbstractPBXObjectFactory()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `abstract             | `createBuildConfig    |                       |
        | XCBuildConfiguration` | uration​(String name)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `a                    | `createBuildFi        |                       |
        | bstract PBXBuildFile` | le​(PBXReference ref)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract             | `creat                |                       |
        |  XCConfigurationList` | eConfigurationList()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract P           | `crea                 |                       |
        | BXContainerItemProxy` | teContainerItemProxy​( |                       |
        |                       | PBXObject containerPo |                       |
        |                       | rtal,                 |                       |
        |                       |          String remot |                       |
        |                       | eGlobalIDString,      |                       |
        |                       |                     P |                       |
        |                       | BXContainerItemProxy. |                       |
        |                       | ProxyType proxyType)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstr                | `c                    |                       |
        | act PBXFileReference` | reateFileReference​(St |                       |
        |                       | ring name,            |                       |
        |                       |          String path, |                       |
        |                       |                     P |                       |
        |                       | BXReference.SourceTre |                       |
        |                       | e sourceTree,         |                       |
        |                       |             Optional< |                       |
        |                       | String> defaultType)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract PBX         | `createFr             |                       |
        | FrameworksBuildPhase` | ameworksBuildPhase()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract             | `creat                |                       |
        | PBXHeadersBuildPhase` | eHeadersBuildPhase()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abst                 | `createNativ          |                       |
        | ract PBXNativeTarget` | eTarget​(String name)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract PBXGroup`   | `                     |                       |
        |                       | createPBXGroup​(String |                       |
        |                       |  name,                |                       |
        |                       | String path,          |                       |
        |                       |       PBXReference.So |                       |
        |                       | urceTree sourceTree)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract PBXProject` | `create               |                       |
        |                       | Project​(String name)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract PBXS        | `createShe            |                       |
        | hellScriptBuildPhase` | llScriptBuildPhase()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract             | `creat                |                       |
        | PBXSourcesBuildPhase` | eSourcesBuildPhase()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract             | `cr                   |                       |
        |  PBXTargetDependency` | eateTargetDependency​( |                       |
        |                       | PBXContainerItemProxy |                       |
        |                       |  containerItemProxy)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abst                 | `createVarian         |                       |
        | ract PBXVariantGroup` | tGroup​(String name,   |                       |
        |                       |                  Stri |                       |
        |                       | ng path,              |                       |
        |                       |       PBXReference.So |                       |
        |                       | urceTree sourceTree)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abs                  | `createVersio         |                       |
        | tract XCVersionGroup` | nGroup​(String name,   |                       |
        |                       |                  Stri |                       |
        |                       | ng path,              |                       |
        |                       |       PBXReference.So |                       |
        |                       | urceTree sourceTree)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Abst          | `DefaultFactory()`    | ::: block             |
        | ractPBXObjectFactory` |                       | The default factory.  |
        |                       |                       | :::                   |
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

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### AbstractPBXObjectFactory

                public AbstractPBXObjectFactory()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#DefaultFactory()}

        -   #### DefaultFactory

            ``` methodSignature
            public static AbstractPBXObjectFactory DefaultFactory()
            ```

            ::: block
            The default factory.
            :::

            [Returns:]{.returnLabel}
            :   The default factory just forwards all calls to new
                PBX\*(\...);

        []{#createProject(java.lang.String)}

        -   #### createProject

            ``` methodSignature
            public abstract PBXProject createProject​(String name)
            ```

        []{#createBuildFile(com.facebook.buck.apple.xcode.xcodeproj.PBXReference)}

        -   #### createBuildFile

            ``` methodSignature
            public abstract PBXBuildFile createBuildFile​(PBXReference ref)
            ```

        []{#createContainerItemProxy(com.facebook.buck.apple.xcode.xcodeproj.PBXObject,java.lang.String,com.facebook.buck.apple.xcode.xcodeproj.PBXContainerItemProxy.ProxyType)}

        -   #### createContainerItemProxy

            ``` methodSignature
            public abstract PBXContainerItemProxy createContainerItemProxy​(PBXObject containerPortal,
                                                                           String remoteGlobalIDString,
                                                                           PBXContainerItemProxy.ProxyType proxyType)
            ```

        []{#createFileReference(java.lang.String,java.lang.String,com.facebook.buck.apple.xcode.xcodeproj.PBXReference.SourceTree,java.util.Optional)}

        -   #### createFileReference

            ``` methodSignature
            public abstract PBXFileReference createFileReference​(String name,
                                                                 @Nullable
                                                                 String path,
                                                                 PBXReference.SourceTree sourceTree,
                                                                 Optional<String> defaultType)
            ```

        []{#createFrameworksBuildPhase()}

        -   #### createFrameworksBuildPhase

            ``` methodSignature
            public abstract PBXFrameworksBuildPhase createFrameworksBuildPhase()
            ```

        []{#createPBXGroup(java.lang.String,java.lang.String,com.facebook.buck.apple.xcode.xcodeproj.PBXReference.SourceTree)}

        -   #### createPBXGroup

            ``` methodSignature
            public abstract PBXGroup createPBXGroup​(String name,
                                                    @Nullable
                                                    String path,
                                                    PBXReference.SourceTree sourceTree)
            ```

        []{#createHeadersBuildPhase()}

        -   #### createHeadersBuildPhase

            ``` methodSignature
            public abstract PBXHeadersBuildPhase createHeadersBuildPhase()
            ```

        []{#createNativeTarget(java.lang.String)}

        -   #### createNativeTarget

            ``` methodSignature
            public abstract PBXNativeTarget createNativeTarget​(String name)
            ```

        []{#createShellScriptBuildPhase()}

        -   #### createShellScriptBuildPhase

            ``` methodSignature
            public abstract PBXShellScriptBuildPhase createShellScriptBuildPhase()
            ```

        []{#createSourcesBuildPhase()}

        -   #### createSourcesBuildPhase

            ``` methodSignature
            public abstract PBXSourcesBuildPhase createSourcesBuildPhase()
            ```

        []{#createTargetDependency(com.facebook.buck.apple.xcode.xcodeproj.PBXContainerItemProxy)}

        -   #### createTargetDependency

            ``` methodSignature
            public abstract PBXTargetDependency createTargetDependency​(PBXContainerItemProxy containerItemProxy)
            ```

        []{#createVariantGroup(java.lang.String,java.lang.String,com.facebook.buck.apple.xcode.xcodeproj.PBXReference.SourceTree)}

        -   #### createVariantGroup

            ``` methodSignature
            public abstract PBXVariantGroup createVariantGroup​(String name,
                                                               @Nullable
                                                               String path,
                                                               PBXReference.SourceTree sourceTree)
            ```

        []{#createConfigurationList()}

        -   #### createConfigurationList

            ``` methodSignature
            public abstract XCConfigurationList createConfigurationList()
            ```

        []{#createBuildConfiguration(java.lang.String)}

        -   #### createBuildConfiguration

            ``` methodSignature
            public abstract XCBuildConfiguration createBuildConfiguration​(String name)
            ```

        []{#createVersionGroup(java.lang.String,java.lang.String,com.facebook.buck.apple.xcode.xcodeproj.PBXReference.SourceTree)}

        -   #### createVersionGroup

            ``` methodSignature
            public abstract XCVersionGroup createVersionGroup​(String name,
                                                              @Nullable
                                                              String path,
                                                              PBXReference.SourceTree sourceTree)
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

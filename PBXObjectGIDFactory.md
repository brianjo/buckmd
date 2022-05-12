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

## Class PBXObjectGIDFactory {#class-pbxobjectgidfactory .title title="Class PBXObjectGIDFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.apple.xcode.AbstractPBXObjectFactory](AbstractPBXObjectFactory.html "class in com.facebook.buck.apple.xcode")

    -   -   com.facebook.buck.apple.xcode.PBXObjectGIDFactory

::: description
-   

    ------------------------------------------------------------------------

        public final class PBXObjectGIDFactory
        extends AbstractPBXObjectFactory

    ::: block
    A factory for creating PBXObjects that assigns a Global ID on
    initialization.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor               Description
          ------------------------- -------------
          `PBXObjectGIDFactory()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type            Method                                                                                                                                                                          Description
          ---------------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `XCBuildConfiguration`       `createBuildConfiguration​(String name)`                                                                                                                                          
          `PBXBuildFile`               `createBuildFile​(PBXReference ref)`                                                                                                                                              
          `XCConfigurationList`        `createConfigurationList()`                                                                                                                                                      
          `PBXContainerItemProxy`      `createContainerItemProxy​(PBXObject containerPortal,                         String remoteGlobalIDString,                         PBXContainerItemProxy.ProxyType proxyType)`    
          `PBXFileReference`           `createFileReference​(String name,                    String path,                    PBXReference.SourceTree sourceTree,                    Optional<String> defaultType)`       
          `PBXFrameworksBuildPhase`    `createFrameworksBuildPhase()`                                                                                                                                                   
          `PBXHeadersBuildPhase`       `createHeadersBuildPhase()`                                                                                                                                                      
          `PBXNativeTarget`            `createNativeTarget​(String name)`                                                                                                                                                
          `PBXGroup`                   `createPBXGroup​(String name,               String path,               PBXReference.SourceTree sourceTree)`                                                                       
          `PBXProject`                 `createProject​(String name)`                                                                                                                                                     
          `PBXShellScriptBuildPhase`   `createShellScriptBuildPhase()`                                                                                                                                                  
          `PBXSourcesBuildPhase`       `createSourcesBuildPhase()`                                                                                                                                                      
          `PBXTargetDependency`        `createTargetDependency​(PBXContainerItemProxy containerItemProxy)`                                                                                                               
          `PBXVariantGroup`            `createVariantGroup​(String name,                   String path,                   PBXReference.SourceTree sourceTree)`                                                           
          `XCVersionGroup`             `createVersionGroup​(String name,                   String path,                   PBXReference.SourceTree sourceTree)`                                                           

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.apple.xcode.AbstractPBXObjectFactory}

            ### Methods inherited from class com.facebook.buck.apple.xcode.[AbstractPBXObjectFactory](AbstractPBXObjectFactory.html "class in com.facebook.buck.apple.xcode")

            `DefaultFactory`

        ```{=html}
        <!-- -->
        ```
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

        -   #### PBXObjectGIDFactory

                public PBXObjectGIDFactory()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#createProject(java.lang.String)}

        -   #### createProject

            ``` methodSignature
            public PBXProject createProject​(String name)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `createProject` in class `AbstractPBXObjectFactory`

        []{#createBuildFile(com.facebook.buck.apple.xcode.xcodeproj.PBXReference)}

        -   #### createBuildFile

            ``` methodSignature
            public PBXBuildFile createBuildFile​(PBXReference ref)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `createBuildFile` in class `AbstractPBXObjectFactory`

        []{#createContainerItemProxy(com.facebook.buck.apple.xcode.xcodeproj.PBXObject,java.lang.String,com.facebook.buck.apple.xcode.xcodeproj.PBXContainerItemProxy.ProxyType)}

        -   #### createContainerItemProxy

            ``` methodSignature
            public PBXContainerItemProxy createContainerItemProxy​(PBXObject containerPortal,
                                                                  String remoteGlobalIDString,
                                                                  PBXContainerItemProxy.ProxyType proxyType)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `createContainerItemProxy` in
                class `AbstractPBXObjectFactory`

        []{#createFileReference(java.lang.String,java.lang.String,com.facebook.buck.apple.xcode.xcodeproj.PBXReference.SourceTree,java.util.Optional)}

        -   #### createFileReference

            ``` methodSignature
            public PBXFileReference createFileReference​(String name,
                                                        @Nullable
                                                        String path,
                                                        PBXReference.SourceTree sourceTree,
                                                        Optional<String> defaultType)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `createFileReference` in
                class `AbstractPBXObjectFactory`

        []{#createFrameworksBuildPhase()}

        -   #### createFrameworksBuildPhase

            ``` methodSignature
            public PBXFrameworksBuildPhase createFrameworksBuildPhase()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `createFrameworksBuildPhase` in
                class `AbstractPBXObjectFactory`

        []{#createPBXGroup(java.lang.String,java.lang.String,com.facebook.buck.apple.xcode.xcodeproj.PBXReference.SourceTree)}

        -   #### createPBXGroup

            ``` methodSignature
            public PBXGroup createPBXGroup​(String name,
                                           @Nullable
                                           String path,
                                           PBXReference.SourceTree sourceTree)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `createPBXGroup` in class `AbstractPBXObjectFactory`

        []{#createHeadersBuildPhase()}

        -   #### createHeadersBuildPhase

            ``` methodSignature
            public PBXHeadersBuildPhase createHeadersBuildPhase()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `createHeadersBuildPhase` in
                class `AbstractPBXObjectFactory`

        []{#createNativeTarget(java.lang.String)}

        -   #### createNativeTarget

            ``` methodSignature
            public PBXNativeTarget createNativeTarget​(String name)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `createNativeTarget` in class `AbstractPBXObjectFactory`

        []{#createShellScriptBuildPhase()}

        -   #### createShellScriptBuildPhase

            ``` methodSignature
            public PBXShellScriptBuildPhase createShellScriptBuildPhase()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `createShellScriptBuildPhase` in
                class `AbstractPBXObjectFactory`

        []{#createSourcesBuildPhase()}

        -   #### createSourcesBuildPhase

            ``` methodSignature
            public PBXSourcesBuildPhase createSourcesBuildPhase()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `createSourcesBuildPhase` in
                class `AbstractPBXObjectFactory`

        []{#createTargetDependency(com.facebook.buck.apple.xcode.xcodeproj.PBXContainerItemProxy)}

        -   #### createTargetDependency

            ``` methodSignature
            public PBXTargetDependency createTargetDependency​(PBXContainerItemProxy containerItemProxy)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `createTargetDependency` in
                class `AbstractPBXObjectFactory`

        []{#createVariantGroup(java.lang.String,java.lang.String,com.facebook.buck.apple.xcode.xcodeproj.PBXReference.SourceTree)}

        -   #### createVariantGroup

            ``` methodSignature
            public PBXVariantGroup createVariantGroup​(String name,
                                                      @Nullable
                                                      String path,
                                                      PBXReference.SourceTree sourceTree)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `createVariantGroup` in class `AbstractPBXObjectFactory`

        []{#createConfigurationList()}

        -   #### createConfigurationList

            ``` methodSignature
            public XCConfigurationList createConfigurationList()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `createConfigurationList` in
                class `AbstractPBXObjectFactory`

        []{#createBuildConfiguration(java.lang.String)}

        -   #### createBuildConfiguration

            ``` methodSignature
            public XCBuildConfiguration createBuildConfiguration​(String name)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `createBuildConfiguration` in
                class `AbstractPBXObjectFactory`

        []{#createVersionGroup(java.lang.String,java.lang.String,com.facebook.buck.apple.xcode.xcodeproj.PBXReference.SourceTree)}

        -   #### createVersionGroup

            ``` methodSignature
            public XCVersionGroup createVersionGroup​(String name,
                                                     @Nullable
                                                     String path,
                                                     PBXReference.SourceTree sourceTree)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `createVersionGroup` in class `AbstractPBXObjectFactory`
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

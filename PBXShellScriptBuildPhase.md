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

## Class PBXShellScriptBuildPhase {#class-pbxshellscriptbuildphase .title title="Class PBXShellScriptBuildPhase"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.apple.xcode.xcodeproj.PBXObject](PBXObject.html "class in com.facebook.buck.apple.xcode.xcodeproj")

    -   -   [com.facebook.buck.apple.xcode.xcodeproj.PBXContainerItem](PBXContainerItem.html "class in com.facebook.buck.apple.xcode.xcodeproj")

        -   -   [com.facebook.buck.apple.xcode.xcodeproj.PBXProjectItem](PBXProjectItem.html "class in com.facebook.buck.apple.xcode.xcodeproj")

            -   -   [com.facebook.buck.apple.xcode.xcodeproj.PBXBuildPhase](PBXBuildPhase.html "class in com.facebook.buck.apple.xcode.xcodeproj")

                -   -   com.facebook.buck.apple.xcode.xcodeproj.PBXShellScriptBuildPhase

::: description
-   

    ------------------------------------------------------------------------

        public class PBXShellScriptBuildPhase
        extends PBXBuildPhase

    ::: block
    Build phase which represents running a shell script.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                    Description
          ------------------------------ -------------
          `PBXShellScriptBuildPhase()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `List<String>`        | `get                  | ::: block             |
        |                       | InputFileListPaths()` | Returns the list      |
        |                       |                       | (possibly empty) of   |
        |                       |                       | .xcfilelist files     |
        |                       |                       | that contain inputs   |
        |                       |                       | for the script        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `List<String>`        | `getInputPaths()`     | ::: block             |
        |                       |                       | Returns the list      |
        |                       |                       | (possibly empty) of   |
        |                       |                       | files passed as input |
        |                       |                       | to the shell script.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `List<String>`        | `getO                 | ::: block             |
        |                       | utputFileListPaths()` | Returns the list      |
        |                       |                       | (possibly empty) of   |
        |                       |                       | .xcfilelist files     |
        |                       |                       | that contain inputs   |
        |                       |                       | for the script        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `List<String>`        | `getOutputPaths()`    | ::: block             |
        |                       |                       | Returns the list      |
        |                       |                       | (possibly empty) of   |
        |                       |                       | files created as      |
        |                       |                       | output of the shell   |
        |                       |                       | script.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getShellPath()`      | ::: block             |
        |                       |                       | Returns the path to   |
        |                       |                       | the shell under which |
        |                       |                       | the script is to be   |
        |                       |                       | executed.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getShellScript()`    | ::: block             |
        |                       |                       | Gets the contents of  |
        |                       |                       | the shell script to   |
        |                       |                       | execute under the     |
        |                       |                       | shell returned by     |
        |                       |                       | [`getShellPath(       |
        |                       |                       | )`](#getShellPath()). |
        |                       |                       | :::                   |
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
        | `protected            | `serializeStringLis   | ::: block             |
        | com.dd.plist.NSArray` | t​(List<String> list)` | Converts List of      |
        |                       |                       | Strings into NSArray  |
        |                       |                       | of NSStrings          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `setShellPa           | ::: block             |
        |                       | th​(String shellPath)` | Sets the path to the  |
        |                       |                       | shell under which the |
        |                       |                       | script is to be       |
        |                       |                       | executed.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `setShellScript       | ::: block             |
        |                       | ​(String shellScript)` | Sets the contents of  |
        |                       |                       | the script to         |
        |                       |                       | execute.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.apple.xcode.xcodeproj.PBXBuildPhase}

            ### Methods inherited from class com.facebook.buck.apple.xcode.xcodeproj.[PBXBuildPhase](PBXBuildPhase.html "class in com.facebook.buck.apple.xcode.xcodeproj")

            `getFiles, getName, setName, setRunOnlyForDeploymentPostprocessing`

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

        -   #### PBXShellScriptBuildPhase

                public PBXShellScriptBuildPhase()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#isa()}

        -   #### isa

            ``` methodSignature
            public String isa()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `isa` in class `PBXProjectItem`

            [Returns:]{.returnLabel}
            :   Type name of the serialized object.

        []{#getInputPaths()}

        -   #### getInputPaths

            ``` methodSignature
            public List<String> getInputPaths()
            ```

            ::: block
            Returns the list (possibly empty) of files passed as input
            to the shell script. May not be actual paths, because they
            can have variable interpolations.
            :::

        []{#getInputFileListPaths()}

        -   #### getInputFileListPaths

            ``` methodSignature
            public List<String> getInputFileListPaths()
            ```

            ::: block
            Returns the list (possibly empty) of .xcfilelist files that
            contain inputs for the script
            :::

        []{#getOutputPaths()}

        -   #### getOutputPaths

            ``` methodSignature
            public List<String> getOutputPaths()
            ```

            ::: block
            Returns the list (possibly empty) of files created as output
            of the shell script. May not be actual paths, because they
            can have variable interpolations.
            :::

        []{#getOutputFileListPaths()}

        -   #### getOutputFileListPaths

            ``` methodSignature
            public List<String> getOutputFileListPaths()
            ```

            ::: block
            Returns the list (possibly empty) of .xcfilelist files that
            contain inputs for the script
            :::

        []{#getShellPath()}

        -   #### getShellPath

            ``` methodSignature
            @Nullable
            public String getShellPath()
            ```

            ::: block
            Returns the path to the shell under which the script is to
            be executed. Defaults to \"/bin/sh\".
            :::

        []{#setShellPath(java.lang.String)}

        -   #### setShellPath

            ``` methodSignature
            public void setShellPath​(String shellPath)
            ```

            ::: block
            Sets the path to the shell under which the script is to be
            executed.
            :::

        []{#getShellScript()}

        -   #### getShellScript

            ``` methodSignature
            @Nullable
            public String getShellScript()
            ```

            ::: block
            Gets the contents of the shell script to execute under the
            shell returned by [`getShellPath()`](#getShellPath()).
            :::

        []{#setShellScript(java.lang.String)}

        -   #### setShellScript

            ``` methodSignature
            public void setShellScript​(String shellScript)
            ```

            ::: block
            Sets the contents of the script to execute.
            :::

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
            :   `serializeInto` in class `PBXBuildPhase`

        []{#serializeStringList(java.util.List)}

        -   #### serializeStringList

            ``` methodSignature
            protected com.dd.plist.NSArray serializeStringList​(List<String> list)
            ```

            ::: block
            Converts List of Strings into NSArray of NSStrings
            :::
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

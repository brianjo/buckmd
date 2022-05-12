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

## Class PBXContainerItemProxy {#class-pbxcontaineritemproxy .title title="Class PBXContainerItemProxy"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.apple.xcode.xcodeproj.PBXObject](PBXObject.html "class in com.facebook.buck.apple.xcode.xcodeproj")

    -   -   [com.facebook.buck.apple.xcode.xcodeproj.PBXContainerItem](PBXContainerItem.html "class in com.facebook.buck.apple.xcode.xcodeproj")

        -   -   com.facebook.buck.apple.xcode.xcodeproj.PBXContainerItemProxy

::: description
-   

    ------------------------------------------------------------------------

        public class PBXContainerItemProxy
        extends PBXContainerItem

    ::: block
    Reference to another object used by
    [`PBXTargetDependency`](PBXTargetDependency.html "class in com.facebook.buck.apple.xcode.xcodeproj").
    Can reference a remote file by specifying the
    [`PBXFileReference`](PBXFileReference.html "class in com.facebook.buck.apple.xcode.xcodeproj")
    to the remote project file, and the GID of the object within that
    file.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                               Description
          ------------------- ----------------------------------- -------------
          `static class `     `PBXContainerItemProxy.ProxyType`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                            Description
          ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `PBXContainerItemProxy​(PBXObject containerPortal,                      String remoteGlobalIDString,                      PBXContainerItemProxy.ProxyType proxyType)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `PBXObject`           | `                     |                       |
        |                       | getContainerPortal()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `PBXContaine          | `getProxyType()`      |                       |
        | rItemProxy.ProxyType` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getRe                |                       |
        |                       | moteGlobalIDString()` |                       |
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
        | `int`                 | `stableHash()`        | ::: block             |
        |                       |                       | This method is used   |
        |                       |                       | to generate stable    |
        |                       |                       | GIDs and must be      |
        |                       |                       | stable for identical  |
        |                       |                       | contents.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.apple.xcode.xcodeproj.PBXObject}

            ### Methods inherited from class com.facebook.buck.apple.xcode.xcodeproj.[PBXObject](PBXObject.html "class in com.facebook.buck.apple.xcode.xcodeproj")

            `generateGid, getGlobalID, setGlobalID, toString`

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

        []{#<init>(com.facebook.buck.apple.xcode.xcodeproj.PBXObject,java.lang.String,com.facebook.buck.apple.xcode.xcodeproj.PBXContainerItemProxy.ProxyType)}

        -   #### PBXContainerItemProxy

                public PBXContainerItemProxy​(PBXObject containerPortal,
                                             String remoteGlobalIDString,
                                             PBXContainerItemProxy.ProxyType proxyType)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getContainerPortal()}

        -   #### getContainerPortal

            ``` methodSignature
            public PBXObject getContainerPortal()
            ```

        []{#getRemoteGlobalIDString()}

        -   #### getRemoteGlobalIDString

            ``` methodSignature
            public String getRemoteGlobalIDString()
            ```

        []{#getProxyType()}

        -   #### getProxyType

            ``` methodSignature
            public PBXContainerItemProxy.ProxyType getProxyType()
            ```

        []{#isa()}

        -   #### isa

            ``` methodSignature
            public String isa()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `isa` in class `PBXContainerItem`

            [Returns:]{.returnLabel}
            :   Type name of the serialized object.

        []{#stableHash()}

        -   #### stableHash

            ``` methodSignature
            public int stableHash()
            ```

            ::: block
            [Description copied from
            class: `PBXObject`]{.descfrmTypeLabel}
            :::

            ::: block
            This method is used to generate stable GIDs and must be
            stable for identical contents. Returning a constant value is
            ok but will make the generated project order-dependent.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `stableHash` in class `PBXObject`

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

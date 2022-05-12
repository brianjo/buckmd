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

## Class PBXProject {#class-pbxproject .title title="Class PBXProject"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.apple.xcode.xcodeproj.PBXObject](PBXObject.html "class in com.facebook.buck.apple.xcode.xcodeproj")

    -   -   [com.facebook.buck.apple.xcode.xcodeproj.PBXContainer](PBXContainer.html "class in com.facebook.buck.apple.xcode.xcodeproj")

        -   -   com.facebook.buck.apple.xcode.xcodeproj.PBXProject

::: description
-   

    ------------------------------------------------------------------------

        public final class PBXProject
        extends PBXContainer

    ::: block
    The root object representing the project itself.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                   Description
          ----------------------------------------------------------------------------- -------------
          `PBXProject​(String name,           AbstractPBXObjectFactory objectFactory)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `XCConfigurationList` | `getBuil              |                       |
        |                       | dConfigurationList()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getCo                |                       |
        |                       | mpatibilityVersion()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `PBXGroup`            | `getMainGroup()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getName()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `List<PBXTarget>`     | `getTargets()`        |                       |
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
        | `void`                | `setName​(String v)`   |                       |
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

        []{#<init>(java.lang.String,com.facebook.buck.apple.xcode.AbstractPBXObjectFactory)}

        -   #### PBXProject

                public PBXProject​(String name,
                                  AbstractPBXObjectFactory objectFactory)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getName()}

        -   #### getName

            ``` methodSignature
            public String getName()
            ```

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public void setName​(String v)
            ```

        []{#getMainGroup()}

        -   #### getMainGroup

            ``` methodSignature
            public PBXGroup getMainGroup()
            ```

        []{#getTargets()}

        -   #### getTargets

            ``` methodSignature
            public List<PBXTarget> getTargets()
            ```

        []{#getBuildConfigurationList()}

        -   #### getBuildConfigurationList

            ``` methodSignature
            public XCConfigurationList getBuildConfigurationList()
            ```

        []{#getCompatibilityVersion()}

        -   #### getCompatibilityVersion

            ``` methodSignature
            public String getCompatibilityVersion()
            ```

        []{#isa()}

        -   #### isa

            ``` methodSignature
            public String isa()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `isa` in class `PBXContainer`

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
            :   `serializeInto` in class `PBXObject`
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

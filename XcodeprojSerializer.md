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

## Class XcodeprojSerializer {#class-xcodeprojserializer .title title="Class XcodeprojSerializer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.xcode.XcodeprojSerializer

::: description
-   

    ------------------------------------------------------------------------

        @NotThreadSafe
        public class XcodeprojSerializer
        extends Object

    ::: block
    Serializer that handles conversion of an in-memory object graph
    representation of an xcode project (instances of
    [`PBXObject`](xcodeproj/PBXObject.html "class in com.facebook.buck.apple.xcode.xcodeproj"))
    into an Apple property list.
    Serialization proceeds from the root object, a \${link PBXProject}
    instance, to all of its referenced objects. Each object being
    visited calls back into this class
    ([`addField(java.lang.String, com.facebook.buck.apple.xcode.xcodeproj.PBXObject)`](#addField(java.lang.String,com.facebook.buck.apple.xcode.xcodeproj.PBXObject)))
    to populate the plist representation with its fields.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                               Description
          ----------------------------------------------------------------------------------------- -------------
          `XcodeprojSerializer​(GidGenerator gidGenerator,                    PBXProject project)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `a                    |                       |
        |                       | ddField​(String name,  |                       |
        |                       |         boolean val)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `addField​(String na   |                       |
        |                       | me,         int val)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `addField​(Stri        |                       |
        |                       | ng name,         com. |                       |
        |                       | dd.plist.NSObject v)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `add                  |                       |
        |                       | Field​(String name,    |                       |
        |                       |       PBXObject obj)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `                     |                       |
        |                       | addField​(String name, |                       |
        |                       |          String val)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `addFi                |                       |
        |                       | eld​(String name,      |                       |
        |                       |     List<? extends PB |                       |
        |                       | XObject> objectList)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.d                | `toPlist()`           | ::: block             |
        | d.plist.NSDictionary` |                       | Generate a plist      |
        |                       |                       | serialization of      |
        |                       |                       | project bound to this |
        |                       |                       | serializer.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
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

        []{#<init>(com.facebook.buck.apple.xcode.GidGenerator,com.facebook.buck.apple.xcode.xcodeproj.PBXProject)}

        -   #### XcodeprojSerializer

                public XcodeprojSerializer​(GidGenerator gidGenerator,
                                           PBXProject project)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#toPlist()}

        -   #### toPlist

            ``` methodSignature
            public com.dd.plist.NSDictionary toPlist()
            ```

            ::: block
            Generate a plist serialization of project bound to this
            serializer.
            :::

        []{#addField(java.lang.String,com.facebook.buck.apple.xcode.xcodeproj.PBXObject)}

        -   #### addField

            ``` methodSignature
            public void addField​(String name,
                                 PBXObject obj)
            ```

        []{#addField(java.lang.String,int)}

        -   #### addField

            ``` methodSignature
            public void addField​(String name,
                                 int val)
            ```

        []{#addField(java.lang.String,java.lang.String)}

        -   #### addField

            ``` methodSignature
            public void addField​(String name,
                                 String val)
            ```

        []{#addField(java.lang.String,boolean)}

        -   #### addField

            ``` methodSignature
            public void addField​(String name,
                                 boolean val)
            ```

        []{#addField(java.lang.String,java.util.List)}

        -   #### addField

            ``` methodSignature
            public void addField​(String name,
                                 List<? extends PBXObject> objectList)
            ```

        []{#addField(java.lang.String,com.dd.plist.NSObject)}

        -   #### addField

            ``` methodSignature
            public void addField​(String name,
                                 com.dd.plist.NSObject v)
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

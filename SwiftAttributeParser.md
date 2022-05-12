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
[Package]{.packageLabelInType} [com.facebook.buck.features.apple.projectV2](package-summary.html)
:::

## Class SwiftAttributeParser {#class-swiftattributeparser .title title="Class SwiftAttributeParser"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.apple.projectV2.SwiftAttributeParser

::: description
-   

    ------------------------------------------------------------------------

        public class SwiftAttributeParser
        extends Object

    ::: block
    Parser that derives Swift specific attributes from a Target and
    returns `SwiftAttributes`.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `SwiftAttributeParser​(Sw          | ::: block                         |
        | iftBuckConfig swiftBuckConfig,    | Attribute parser for Swift        |
        |                   ProjectGenerati | specific attributes of a Target.. |
        | onStateCache projectGenerationSta | :::                               |
        | teCache,                     Proj |                                   |
        | ectFilesystem projectFilesystem)` |                                   |
        +-----------------------------------+-----------------------------------+

        : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static String`       | `getSwiftOb           | ::: block             |
        |                       | jCGeneratedHeaderName | Get the generated     |
        |                       | ​(TargetNode<?> node,  | header name with the  |
        |                       |                       | provided              |
        |                       |           Optional<St | `optModuleName` or    |
        |                       | ring> optModuleName)` | getting the module    |
        |                       |                       | name from the `node`. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.facebook.buck    | `par                  | ::: block             |
        | .features.apple.proje | seSwiftAttributes​(Tar | Parse Swift specific  |
        | ctV2.SwiftAttributes` | getNode<? extends Cxx | attributes for the    |
        |                       | LibraryDescription.Co | `targetNode`.         |
        |                       | mmonArg> targetNode)` | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
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

        []{#<init>(com.facebook.buck.swift.SwiftBuckConfig,com.facebook.buck.features.apple.projectV2.ProjectGenerationStateCache,com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### SwiftAttributeParser

                public SwiftAttributeParser​(SwiftBuckConfig swiftBuckConfig,
                                            ProjectGenerationStateCache projectGenerationStateCache,
                                            ProjectFilesystem projectFilesystem)

            ::: block
            Attribute parser for Swift specific attributes of a Target..
            :::

            [Parameters:]{.paramLabel}
            :   `swiftBuckConfig` -
            :   `projectGenerationStateCache` -
            :   `projectFilesystem` -
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#parseSwiftAttributes(com.facebook.buck.core.model.targetgraph.TargetNode)}

        -   #### parseSwiftAttributes

            ``` methodSignature
            public com.facebook.buck.features.apple.projectV2.SwiftAttributes parseSwiftAttributes​(TargetNode<? extends CxxLibraryDescription.CommonArg> targetNode)
            ```

            ::: block
            Parse Swift specific attributes for the `targetNode`.
            :::

        []{#getSwiftObjCGeneratedHeaderName(com.facebook.buck.core.model.targetgraph.TargetNode,java.util.Optional)}

        -   #### getSwiftObjCGeneratedHeaderName

            ``` methodSignature
            public static String getSwiftObjCGeneratedHeaderName​(TargetNode<?> node,
                                                                 Optional<String> optModuleName)
            ```

            ::: block
            Get the generated header name with the provided
            `optModuleName` or getting the module name from the `node`.
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

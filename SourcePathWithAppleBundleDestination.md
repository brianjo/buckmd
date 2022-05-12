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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.apple](package-summary.html)
:::

## Class SourcePathWithAppleBundleDestination {#class-sourcepathwithapplebundledestination .title title="Class SourcePathWithAppleBundleDestination"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.SourcePathWithAppleBundleDestination

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`,
        `Comparable<SourcePathWithAppleBundleDestination>`

    ------------------------------------------------------------------------

        public abstract class SourcePathWithAppleBundleDestination
        extends Object
        implements AddsToRuleKey, Comparable<SourcePathWithAppleBundleDestination>

    ::: block
    Simple type representing a
    [`SourcePath`](../core/sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")
    and a destination
    [`AppleBundleDestination`](AppleBundleDestination.html "enum in com.facebook.buck.apple")
    in a resulting bundle where a file or a directory with this path
    should be copied.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                Description
          ------------------------------------------ -------------
          `SourcePathWithAppleBundleDestination()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `int`                 | `compareT             |                       |
        |                       | o​(SourcePathWithApple |                       |
        |                       | BundleDestination o)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract boolean`    | `getCodesignOnCopy()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Ap          | `getDestination()`    |                       |
        | pleBundleDestination` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract SourcePath` | `getSourcePath()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `of​(So                | ::: block             |
        | atic SourcePathWithAp | urcePath sourcePath)` | Construct a new       |
        | pleBundleDestination` |                       | immutable             |
        |                       |                       | `SourcePathWithAp     |
        |                       |                       | pleBundleDestination` |
        |                       |                       | instance with default |
        |                       |                       | value of apple bundle |
        |                       |                       | destination.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `o                    |                       |
        | atic SourcePathWithAp | f​(SourcePath sourcePa |                       |
        | pleBundleDestination` | th,   AppleBundleDest |                       |
        |                       | ination destination)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `of​(Sou               |                       |
        | atic SourcePathWithAp | rcePath sourcePath,   |                       |
        | pleBundleDestination` |  AppleBundleDestinati |                       |
        |                       | on destination,   boo |                       |
        |                       | lean codesignOnCopy)` |                       |
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

        -   #### SourcePathWithAppleBundleDestination

                public SourcePathWithAppleBundleDestination()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getSourcePath()}

        -   #### getSourcePath

            ``` methodSignature
            public abstract SourcePath getSourcePath()
            ```

        []{#getDestination()}

        -   #### getDestination

            ``` methodSignature
            public abstract AppleBundleDestination getDestination()
            ```

        []{#getCodesignOnCopy()}

        -   #### getCodesignOnCopy

            ``` methodSignature
            public abstract boolean getCodesignOnCopy()
            ```

        []{#of(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### of

            ``` methodSignature
            public static SourcePathWithAppleBundleDestination of​(SourcePath sourcePath)
            ```

            ::: block
            Construct a new immutable
            `SourcePathWithAppleBundleDestination` instance with default
            value of apple bundle destination.
            :::

            [Parameters:]{.paramLabel}
            :   `sourcePath` - The value for the `sourcePath` attribute

            [Returns:]{.returnLabel}
            :   An immutable SourcePathWithAppleBundleDestination
                instance

        []{#of(com.facebook.buck.core.sourcepath.SourcePath,com.facebook.buck.apple.AppleBundleDestination)}

        -   #### of

            ``` methodSignature
            public static SourcePathWithAppleBundleDestination of​(SourcePath sourcePath,
                                                                  AppleBundleDestination destination)
            ```

        []{#of(com.facebook.buck.core.sourcepath.SourcePath,com.facebook.buck.apple.AppleBundleDestination,boolean)}

        -   #### of

            ``` methodSignature
            public static SourcePathWithAppleBundleDestination of​(SourcePath sourcePath,
                                                                  AppleBundleDestination destination,
                                                                  boolean codesignOnCopy)
            ```

        []{#compareTo(com.facebook.buck.apple.SourcePathWithAppleBundleDestination)}

        -   #### compareTo

            ``` methodSignature
            public int compareTo​(SourcePathWithAppleBundleDestination o)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `compareTo` in
                interface `Comparable<SourcePathWithAppleBundleDestination>`
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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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

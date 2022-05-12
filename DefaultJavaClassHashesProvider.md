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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java](package-summary.html)
:::

## Class DefaultJavaClassHashesProvider {#class-defaultjavaclasshashesprovider .title title="Class DefaultJavaClassHashesProvider"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.DefaultJavaClassHashesProvider

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`, `JavaClassHashesProvider`

    ------------------------------------------------------------------------

        public class DefaultJavaClassHashesProvider
        extends Object
        implements JavaClassHashesProvider

    ::: block
    Default implementation of
    [`JavaClassHashesProvider`](../core/JavaClassHashesProvider.html "interface in com.facebook.buck.jvm.core")
    interface
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                 Description
          --------------------------------------------------------------------------- -------------
          `DefaultJavaClassHashesProvider​(SourcePath classNamesToHashesSourcePath)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `c                    | `                     |                       |
        | om.google.common.coll | getClassNamesToHashes |                       |
        | ect.ImmutableSortedMa | ​(ProjectFilesystem fi |                       |
        | p<String,​com.google.c | lesystem,             |                       |
        | ommon.hash.HashCode>` |           SourcePathR |                       |
        |                       | esolverAdapter source |                       |
        |                       | PathResolverAdapter)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `invalidate()`        | ::: block             |
        |                       |                       | Invalidates a state   |
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

        []{#<init>(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### DefaultJavaClassHashesProvider

                public DefaultJavaClassHashesProvider​(SourcePath classNamesToHashesSourcePath)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getClassNamesToHashes(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### getClassNamesToHashes

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedMap<String,​com.google.common.hash.HashCode> getClassNamesToHashes​(ProjectFilesystem filesystem,
                                                                                                                                    SourcePathResolverAdapter sourcePathResolverAdapter)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getClassNamesToHashes` in
                interface `JavaClassHashesProvider`

        []{#invalidate()}

        -   #### invalidate

            ``` methodSignature
            public void invalidate()
            ```

            ::: block
            [Description copied from
            interface: `JavaClassHashesProvider`]{.descfrmTypeLabel}
            :::

            ::: block
            Invalidates a state
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `invalidate` in interface `JavaClassHashesProvider`
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

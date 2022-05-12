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

## Class ResolvedJavacPluginProperties {#class-resolvedjavacpluginproperties .title title="Class ResolvedJavacPluginProperties"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.ResolvedJavacPluginProperties

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`

    ------------------------------------------------------------------------

        public class ResolvedJavacPluginProperties
        extends Object
        implements AddsToRuleKey
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                               Description
          ----------------------------------------------------------------------------------------- -------------
          `ResolvedJavacPluginProperties​(com.facebook.buck.jvm.java.JavacPluginProperties inner)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `boolean`             | `getC                 |                       |
        |                       | anReuseClassLoader()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `URL[]`               | `getClas              | ::: block             |
        |                       | spath​(SourcePathResol | Get the classpath for |
        |                       | verAdapter resolver,  | the plugin.           |
        |                       |             ProjectFi | :::                   |
        |                       | lesystem filesystem)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `g                    |                       |
        |                       | etDoesNotAffectAbi()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.comm      | `getInputs()`         |                       |
        | on.collect.ImmutableS |                       |                       |
        | ortedSet<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Jav                  | `getJavacPlugin       | ::: block             |
        | acPluginJsr199Fields` | Jsr199Fields​(SourcePa | Get the javac plugin  |
        |                       | thResolverAdapter res | fields.               |
        |                       | olver,                | :::                   |
        |                       |             ProjectFi |                       |
        |                       | lesystem filesystem)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `ge                   |                       |
        |                       | tJoinedClasspath​(Sour |                       |
        |                       | cePathResolverAdapter |                       |
        |                       |  resolver,            |                       |
        |                       |         ProjectFilesy |                       |
        |                       | stem filesystem,      |                       |
        |                       |               com.goo |                       |
        |                       | gle.common.collect.Im |                       |
        |                       | mutableList<ResolvedJ |                       |
        |                       | avacPluginProperties> |                       |
        |                       |  resolvedProperties)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `getProcessorNames()` |                       |
        | common.collect.Immuta |                       |                       |
        | bleSortedSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getSupportAbiGe      |                       |
        |                       | nerationFromSource()` |                       |
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

        []{#<init>(com.facebook.buck.jvm.java.JavacPluginProperties)}

        -   #### ResolvedJavacPluginProperties

                public ResolvedJavacPluginProperties​(com.facebook.buck.jvm.java.JavacPluginProperties inner)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getCanReuseClassLoader()}

        -   #### getCanReuseClassLoader

            ``` methodSignature
            public boolean getCanReuseClassLoader()
            ```

        []{#getDoesNotAffectAbi()}

        -   #### getDoesNotAffectAbi

            ``` methodSignature
            public boolean getDoesNotAffectAbi()
            ```

        []{#getSupportAbiGenerationFromSource()}

        -   #### getSupportAbiGenerationFromSource

            ``` methodSignature
            public boolean getSupportAbiGenerationFromSource()
            ```

        []{#getProcessorNames()}

        -   #### getProcessorNames

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<String> getProcessorNames()
            ```

        []{#getClasspath(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### getClasspath

            ``` methodSignature
            public URL[] getClasspath​(SourcePathResolverAdapter resolver,
                                      ProjectFilesystem filesystem)
            ```

            ::: block
            Get the classpath for the plugin.
            :::

        []{#getInputs()}

        -   #### getInputs

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<SourcePath> getInputs()
            ```

        []{#getJavacPluginJsr199Fields(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### getJavacPluginJsr199Fields

            ``` methodSignature
            public JavacPluginJsr199Fields getJavacPluginJsr199Fields​(SourcePathResolverAdapter resolver,
                                                                      ProjectFilesystem filesystem)
            ```

            ::: block
            Get the javac plugin fields.
            :::

        []{#getJoinedClasspath(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,com.facebook.buck.io.filesystem.ProjectFilesystem,com.google.common.collect.ImmutableList)}

        -   #### getJoinedClasspath

            ``` methodSignature
            public static String getJoinedClasspath​(SourcePathResolverAdapter resolver,
                                                    ProjectFilesystem filesystem,
                                                    com.google.common.collect.ImmutableList<ResolvedJavacPluginProperties> resolvedProperties)
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

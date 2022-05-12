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
-   [Nested](#nested.class.summary) \| 
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.cxx](package-summary.html)
:::

## Class Omnibus {#class-omnibus .title title="Class Omnibus"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.Omnibus

::: description
-   

    ------------------------------------------------------------------------

        public class Omnibus
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type     Class                        Description
          --------------------- ---------------------------- -------------
          `static class `       `Omnibus.OmnibusLibraries`    
          `static interface `   `Omnibus.OmnibusLibrary`      
          `static interface `   `Omnibus.OmnibusRoot`         

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field              Description
          ------------------- ------------------ -------------
          `static Flavor`     `OMNIBUS_FLAVOR`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static Omni          | `getShar              | ::: block             |
        | bus.OmnibusLibraries` | edLibraries​(BuildTarg | An alternate link     |
        |                       | et buildTarget,       | strategy for          |
        |                       |              ProjectF | languages which need  |
        |                       | ilesystem projectFile | to package native     |
        |                       | system,               | deps up as shared     |
        |                       |      BuildRuleParams  | libraries, which only |
        |                       | params,               | links native nodes    |
        |                       |      CellPathResolver | which have an         |
        |                       |  cellPathResolver,    | explicit edge from    |
        |                       |                 Actio | non-native code as    |
        |                       | nGraphBuilder graphBu | separate, and         |
        |                       | ilder,                | statically linking    |
        |                       |     CxxBuckConfig cxx | all other native      |
        |                       | BuckConfig,           | nodes into a single   |
        |                       |          CxxPlatform  | giant shared library. |
        |                       | cxxPlatform,          | :::                   |
        |                       |           com.google. |                       |
        |                       | common.collect.Immuta |                       |
        |                       | bleList<? extends Arg |                       |
        |                       | > extraLdflags,       |                       |
        |                       |              Iterable |                       |
        |                       | <? extends NativeLink |                       |
        |                       | Target> nativeLinkTar |                       |
        |                       | getRoots,             |                       |
        |                       |        Iterable<? ext |                       |
        |                       | ends NativeLinkable>  |                       |
        |                       | nativeLinkableRoots)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#OMNIBUS_FLAVOR}

        -   #### OMNIBUS_FLAVOR

                public static final Flavor OMNIBUS_FLAVOR
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getSharedLibraries(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.core.cell.CellPathResolver,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.cxx.config.CxxBuckConfig,com.facebook.buck.cxx.toolchain.CxxPlatform,com.google.common.collect.ImmutableList,java.lang.Iterable,java.lang.Iterable)}

        -   #### getSharedLibraries

            ``` methodSignature
            public static Omnibus.OmnibusLibraries getSharedLibraries​(BuildTarget buildTarget,
                                                                      ProjectFilesystem projectFilesystem,
                                                                      BuildRuleParams params,
                                                                      CellPathResolver cellPathResolver,
                                                                      ActionGraphBuilder graphBuilder,
                                                                      CxxBuckConfig cxxBuckConfig,
                                                                      CxxPlatform cxxPlatform,
                                                                      com.google.common.collect.ImmutableList<? extends Arg> extraLdflags,
                                                                      Iterable<? extends NativeLinkTarget> nativeLinkTargetRoots,
                                                                      Iterable<? extends NativeLinkable> nativeLinkableRoots)
            ```

            ::: block
            An alternate link strategy for languages which need to
            package native deps up as shared libraries, which only links
            native nodes which have an explicit edge from non-native
            code as separate, and statically linking all other native
            nodes into a single giant shared library. This reduces the
            number of shared libraries considerably and also allows the
            linker to throw away a lot of unused object files.
            :::

            [Parameters:]{.paramLabel}
            :   `cellPathResolver` -
            :   `nativeLinkTargetRoots` - root nodes which will be
                included in the omnibus link.
            :   `nativeLinkableRoots` - root nodes which are to be
                excluded from the omnibus link.

            [Returns:]{.returnLabel}
            :   a map of shared library names to their containing
                [`SourcePath`](../core/sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")s.
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
-   [Nested](#nested.class.summary) \| 
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

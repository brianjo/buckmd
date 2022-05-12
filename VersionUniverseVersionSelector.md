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
[Package]{.packageLabelInType} [com.facebook.buck.versions](package-summary.html)
:::

## Class VersionUniverseVersionSelector {#class-versionuniverseversionselector .title title="Class VersionUniverseVersionSelector"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.versions.VersionUniverseVersionSelector

::: description
-   

    All Implemented Interfaces:
    :   `VersionSelector`

    ------------------------------------------------------------------------

        public class VersionUniverseVersionSelector
        extends Object
        implements VersionSelector

    ::: block
    A fast constraint resolver which selects versions using pre-defined
    version universes.
    TODO(agallagher): Validate version constraints.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                         Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `VersionUniverseVersionSelector​(TargetGraph targetGraph,                               com.google.common.collect.ImmutableMap<String,​VersionUniverse> universes)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                               Method                                                                                                                                           Description
          --------------------------------------------------------------- ------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `protected Optional<Map.Entry<String,​VersionUniverse>>`         `getVersionUniverse​(TargetNode<?> root)`                                                                                                          
          `com.google.common.collect.ImmutableMap<BuildTarget,​Version>`   `resolve​(BuildTarget root,        com.google.common.collect.ImmutableMap<BuildTarget,​com.google.common.collect.ImmutableSet<Version>> domain)`    

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

        []{#<init>(com.facebook.buck.core.model.targetgraph.TargetGraph,com.google.common.collect.ImmutableMap)}

        -   #### VersionUniverseVersionSelector

                public VersionUniverseVersionSelector​(TargetGraph targetGraph,
                                                      com.google.common.collect.ImmutableMap<String,​VersionUniverse> universes)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getVersionUniverse(com.facebook.buck.core.model.targetgraph.TargetNode)}

        -   #### getVersionUniverse

            ``` methodSignature
            protected Optional<Map.Entry<String,​VersionUniverse>> getVersionUniverse​(TargetNode<?> root)
            ```

        []{#resolve(com.facebook.buck.core.model.BuildTarget,com.google.common.collect.ImmutableMap)}

        -   #### resolve

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<BuildTarget,​Version> resolve​(BuildTarget root,
                                                                                             com.google.common.collect.ImmutableMap<BuildTarget,​com.google.common.collect.ImmutableSet<Version>> domain)
                                                                                      throws VersionException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `resolve` in interface `VersionSelector`

            [Parameters:]{.paramLabel}
            :   `root` - the root of the versioned sub-graph.
            :   `domain` - the versioned nodes and their version domain.

            [Returns:]{.returnLabel}
            :   the map of versioned nodes to their selected versions.

            [Throws:]{.throwsLabel}
            :   `VersionException`
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

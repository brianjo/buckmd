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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.core.artifact.converter](package-summary.html)
:::

## Class SourceArtifactConverter {#class-sourceartifactconverter .title title="Class SourceArtifactConverter"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.artifact.converter.SourceArtifactConverter

::: description
-   

    ------------------------------------------------------------------------

        public class SourceArtifactConverter
        extends Object

    ::: block
    Utility class to resolve specified
    [`SourcePath`](../../sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")
    into
    [`Artifact`](../Artifact.html "interface in com.facebook.buck.core.artifact")s.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                 Method                                                                                                                                                   Description
          ----------------------------------------------------------------- -------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `static Artifact`                                                 `getArtifactsFromSrc​(SourcePath src,                    com.google.common.collect.ImmutableMap<BuildTarget,​ProviderInfoCollection> deps)`                 
          `static com.google.common.collect.ImmutableSortedSet<Artifact>`   `getArtifactsFromSrcs​(Iterable<SourcePath> srcs,                     com.google.common.collect.ImmutableMap<BuildTarget,​ProviderInfoCollection> deps)`    

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
    -   []{#method.detail}

        ### Method Detail

        []{#getArtifactsFromSrc(com.facebook.buck.core.sourcepath.SourcePath,com.google.common.collect.ImmutableMap)}

        -   #### getArtifactsFromSrc

            ``` methodSignature
            public static Artifact getArtifactsFromSrc​(SourcePath src,
                                                       com.google.common.collect.ImmutableMap<BuildTarget,​ProviderInfoCollection> deps)
            ```

            [Parameters:]{.paramLabel}
            :   `src` - the object representing the sources of a rule
                attribute
            :   `deps` - the
                [`ProviderInfoCollection`](../../rules/providers/collect/ProviderInfoCollection.html "interface in com.facebook.buck.core.rules.providers.collect")
                from the dependencies of a rule

            [Returns:]{.returnLabel}
            :   the
                [`Artifact`](../Artifact.html "interface in com.facebook.buck.core.artifact")s
                representing the sources.

        []{#getArtifactsFromSrcs(java.lang.Iterable,com.google.common.collect.ImmutableMap)}

        -   #### getArtifactsFromSrcs

            ``` methodSignature
            public static com.google.common.collect.ImmutableSortedSet<Artifact> getArtifactsFromSrcs​(Iterable<SourcePath> srcs,
                                                                                                      com.google.common.collect.ImmutableMap<BuildTarget,​ProviderInfoCollection> deps)
            ```

            [Parameters:]{.paramLabel}
            :   `srcs` - the set of the sources of a rule attribute
            :   `deps` - the
                [`ProviderInfoCollection`](../../rules/providers/collect/ProviderInfoCollection.html "interface in com.facebook.buck.core.rules.providers.collect")
                from the dependencies of a rule

            [Returns:]{.returnLabel}
            :   the
                [`Artifact`](../Artifact.html "interface in com.facebook.buck.core.artifact")s
                representing the sources.
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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

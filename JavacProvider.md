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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java](package-summary.html)
:::

## Interface JavacProvider {#interface-javacprovider .title title="Interface JavacProvider"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `ConstantJavacProvider`, `ExternalJavacProvider`,
        `JarBackedJavacProvider`

    ------------------------------------------------------------------------

        public interface JavacProvider
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                     Method                                                                                                Description
          ----------------------------------------------------- ----------------------------------------------------------------------------------------------------- -------------
          `void`                                                `addParseTimeDeps​(com.google.common.collect.ImmutableCollection.Builder<BuildTarget> depsConsumer)`    
          `com.google.common.collect.ImmutableSet<BuildRule>`   `getBuildDeps​(SourcePathRuleFinder ruleFinder)`                                                        
          `Javac`                                               `resolve​(SourcePathRuleFinder ruleFinder)`                                                             

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#resolve(com.facebook.buck.core.rules.SourcePathRuleFinder)}

        -   #### resolve

            ``` methodSignature
            Javac resolve​(SourcePathRuleFinder ruleFinder)
            ```

        []{#addParseTimeDeps(com.google.common.collect.ImmutableCollection.Builder)}

        -   #### addParseTimeDeps

            ``` methodSignature
            void addParseTimeDeps​(com.google.common.collect.ImmutableCollection.Builder<BuildTarget> depsConsumer)
            ```

        []{#getBuildDeps(com.facebook.buck.core.rules.SourcePathRuleFinder)}

        -   #### getBuildDeps

            ``` methodSignature
            com.google.common.collect.ImmutableSet<BuildRule> getBuildDeps​(SourcePathRuleFinder ruleFinder)
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
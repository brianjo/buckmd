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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.core](package-summary.html)
:::

## Class EmptyJavaAbiInfo {#class-emptyjavaabiinfo .title title="Class EmptyJavaAbiInfo"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.core.EmptyJavaAbiInfo

::: description
-   

    All Implemented Interfaces:
    :   `JavaAbiInfo`

    ------------------------------------------------------------------------

        public class EmptyJavaAbiInfo
        extends Object
        implements JavaAbiInfo

    ::: block
    The implementation of JavaAbiInfo for targets that have no sources.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                   Description
          --------------------------------------------- -------------
          `EmptyJavaAbiInfo​(BuildTarget buildTarget)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                            Method                                           Description
          ------------------------------------------------------------ ------------------------------------------------ -------------
          `BuildTarget`                                                `getBuildTarget()`                                
          `com.google.common.collect.ImmutableSortedSet<SourcePath>`   `getJarContents()`                                
          `void`                                                       `invalidate()`                                    
          `boolean`                                                    `jarContains​(String path)`                        
          `void`                                                       `load​(SourcePathResolverAdapter pathResolver)`    

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

        []{#<init>(com.facebook.buck.core.model.BuildTarget)}

        -   #### EmptyJavaAbiInfo

                public EmptyJavaAbiInfo​(BuildTarget buildTarget)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBuildTarget()}

        -   #### getBuildTarget

            ``` methodSignature
            public BuildTarget getBuildTarget()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildTarget` in interface `JavaAbiInfo`

        []{#getJarContents()}

        -   #### getJarContents

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<SourcePath> getJarContents()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getJarContents` in interface `JavaAbiInfo`

        []{#jarContains(java.lang.String)}

        -   #### jarContains

            ``` methodSignature
            public boolean jarContains​(String path)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `jarContains` in interface `JavaAbiInfo`

        []{#load(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### load

            ``` methodSignature
            public void load​(SourcePathResolverAdapter pathResolver)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `load` in interface `JavaAbiInfo`

        []{#invalidate()}

        -   #### invalidate

            ``` methodSignature
            public void invalidate()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `invalidate` in interface `JavaAbiInfo`
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

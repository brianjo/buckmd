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
[Package]{.packageLabelInType} [com.facebook.buck.features.lua](package-summary.html)
:::

## Class LuaUtil {#class-luautil .title title="Class LuaUtil"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.lua.LuaUtil

::: description
-   

    ------------------------------------------------------------------------

        public class LuaUtil
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                    Method                                                                                                                                                                                                               Description
          -------------------------------------------------------------------- -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `static String`                                                      `getBaseModule​(BuildTarget target,              Optional<String> override)`                                                                                                                                           
          `static com.google.common.collect.ImmutableList<BuildTarget>`        `getDeps​(CxxPlatform cxxPlatform,        com.google.common.collect.ImmutableSortedSet<BuildTarget> deps,        PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<BuildTarget>> platformDeps)`    
          `static com.google.common.collect.ImmutableMap<String,​SourcePath>`   `toModuleMap​(BuildTarget target,            SourcePathResolverAdapter resolver,            String parameter,            String baseModule,            Iterable<SourceSortedSet> inputs)`                              

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

        []{#toModuleMap(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,java.lang.String,java.lang.String,java.lang.Iterable)}

        -   #### toModuleMap

            ``` methodSignature
            public static com.google.common.collect.ImmutableMap<String,​SourcePath> toModuleMap​(BuildTarget target,
                                                                                                      SourcePathResolverAdapter resolver,
                                                                                                      String parameter,
                                                                                                      String baseModule,
                                                                                                      Iterable<SourceSortedSet> inputs)
            ```

        []{#getBaseModule(com.facebook.buck.core.model.BuildTarget,java.util.Optional)}

        -   #### getBaseModule

            ``` methodSignature
            public static String getBaseModule​(BuildTarget target,
                                               Optional<String> override)
            ```

        []{#getDeps(com.facebook.buck.cxx.toolchain.CxxPlatform,com.google.common.collect.ImmutableSortedSet,com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### getDeps

            ``` methodSignature
            public static com.google.common.collect.ImmutableList<BuildTarget> getDeps​(CxxPlatform cxxPlatform,
                                                                                       com.google.common.collect.ImmutableSortedSet<BuildTarget> deps,
                                                                                       PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<BuildTarget>> platformDeps)
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

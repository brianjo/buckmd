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
[Package]{.packageLabelInType} [com.facebook.buck.rules.macros](package-summary.html)
:::

## Class StringWithMacrosConverter {#class-stringwithmacrosconverter .title title="Class StringWithMacrosConverter"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.macros.StringWithMacrosConverter

::: description
-   

    ------------------------------------------------------------------------

        public abstract class StringWithMacrosConverter
        extends Object

    ::: block
    Converts a
    [`StringWithMacros`](StringWithMacros.html "class in com.facebook.buck.rules.macros")
    into an
    [`Arg`](../args/Arg.html "interface in com.facebook.buck.rules.args").
    Performs conversion eagerly, and meant as a replacement for the lazy
    [`Arg`](../args/Arg.html "interface in com.facebook.buck.rules.args").
    As this holds a reference to an
    [`ActionGraphBuilder`](../../core/rules/ActionGraphBuilder.html "interface in com.facebook.buck.core.rules"),
    instances of this object should not be capture by anything in the
    action graph.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                     Description
          ------------------------------- -------------
          `StringWithMacrosConverter()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                                                   Method                                                                                                                                                                                                                                                                                                               Description
          --------------------------------------------------------------------------------------------------- -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `Arg`                                                                                               `convert​(StringWithMacros val)`                                                                                                                                                                                                                                                                                       
          `abstract ActionGraphBuilder`                                                                       `getActionGraphBuilder()`                                                                                                                                                                                                                                                                                             
          `abstract BuildTarget`                                                                              `getBuildTarget()`                                                                                                                                                                                                                                                                                                    
          `protected abstract CellNameResolver`                                                               `getCellNameResolver()`                                                                                                                                                                                                                                                                                               
          `com.google.common.collect.ImmutableMap<Class<? extends Macro>,​MacroExpander<? extends Macro,​?>>`   `getClassExpanders()`                                                                                                                                                                                                                                                                                                 
          `abstract com.google.common.collect.ImmutableList<MacroExpander<? extends Macro,​?>>`                `getExpanders()`                                                                                                                                                                                                                                                                                                      
          `abstract HashMap<Macro,​Object>`                                                                    `getPrecomputedWorkCache()`                                                                                                                                                                                                                                                                                           
          `abstract Optional<java.util.function.Function<String,​String>>`                                     `getSanitizer()`                                                                                                                                                                                                                                                                                                      
          `static StringWithMacrosConverter`                                                                  `of​(BuildTarget buildTarget,   CellNameResolver cellNameResolver,   ActionGraphBuilder actionGraphBuilder,   com.google.common.collect.ImmutableList<MacroExpander<? extends Macro,​?>> expanders)`                                                                                                                    
          `static StringWithMacrosConverter`                                                                  `of​(BuildTarget buildTarget,   CellNameResolver cellNameResolver,   ActionGraphBuilder actionGraphBuilder,   com.google.common.collect.ImmutableList<MacroExpander<? extends Macro,​?>> expanders,   Optional<java.util.function.Function<String,​String>> sanitizer)`                                                  
          `static StringWithMacrosConverter`                                                                  `of​(BuildTarget buildTarget,   CellNameResolver cellNameResolver,   ActionGraphBuilder actionGraphBuilder,   com.google.common.collect.ImmutableList<MacroExpander<? extends Macro,​?>> expanders,   Optional<java.util.function.Function<String,​String>> sanitizer,   HashMap<Macro,​Object> precomputedWorkCache)`    

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

        -   #### StringWithMacrosConverter

                public StringWithMacrosConverter()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBuildTarget()}

        -   #### getBuildTarget

            ``` methodSignature
            public abstract BuildTarget getBuildTarget()
            ```

        []{#getCellNameResolver()}

        -   #### getCellNameResolver

            ``` methodSignature
            protected abstract CellNameResolver getCellNameResolver()
            ```

        []{#getActionGraphBuilder()}

        -   #### getActionGraphBuilder

            ``` methodSignature
            public abstract ActionGraphBuilder getActionGraphBuilder()
            ```

        []{#getExpanders()}

        -   #### getExpanders

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<MacroExpander<? extends Macro,​?>> getExpanders()
            ```

        []{#getSanitizer()}

        -   #### getSanitizer

            ``` methodSignature
            public abstract Optional<java.util.function.Function<String,​String>> getSanitizer()
            ```

        []{#of(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.core.rules.ActionGraphBuilder,com.google.common.collect.ImmutableList)}

        -   #### of

            ``` methodSignature
            public static StringWithMacrosConverter of​(BuildTarget buildTarget,
                                                       CellNameResolver cellNameResolver,
                                                       ActionGraphBuilder actionGraphBuilder,
                                                       com.google.common.collect.ImmutableList<MacroExpander<? extends Macro,​?>> expanders)
            ```

        []{#of(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.core.rules.ActionGraphBuilder,com.google.common.collect.ImmutableList,java.util.Optional)}

        -   #### of

            ``` methodSignature
            public static StringWithMacrosConverter of​(BuildTarget buildTarget,
                                                       CellNameResolver cellNameResolver,
                                                       ActionGraphBuilder actionGraphBuilder,
                                                       com.google.common.collect.ImmutableList<MacroExpander<? extends Macro,​?>> expanders,
                                                       Optional<java.util.function.Function<String,​String>> sanitizer)
            ```

        []{#of(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.core.rules.ActionGraphBuilder,com.google.common.collect.ImmutableList,java.util.Optional,java.util.HashMap)}

        -   #### of

            ``` methodSignature
            public static StringWithMacrosConverter of​(BuildTarget buildTarget,
                                                       CellNameResolver cellNameResolver,
                                                       ActionGraphBuilder actionGraphBuilder,
                                                       com.google.common.collect.ImmutableList<MacroExpander<? extends Macro,​?>> expanders,
                                                       Optional<java.util.function.Function<String,​String>> sanitizer,
                                                       HashMap<Macro,​Object> precomputedWorkCache)
            ```

        []{#getPrecomputedWorkCache()}

        -   #### getPrecomputedWorkCache

            ``` methodSignature
            @Auxiliary
            public abstract HashMap<Macro,​Object> getPrecomputedWorkCache()
            ```

        []{#getClassExpanders()}

        -   #### getClassExpanders

            ``` methodSignature
            @Derived
            public com.google.common.collect.ImmutableMap<Class<? extends Macro>,​MacroExpander<? extends Macro,​?>> getClassExpanders()
            ```

        []{#convert(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### convert

            ``` methodSignature
            public Arg convert​(StringWithMacros val)
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

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

## Class JavacFactory {#class-javacfactory .title title="Class JavacFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.JavacFactory

::: description
-   

    ------------------------------------------------------------------------

        public final class JavacFactory
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                    Description
          ---------------------------------------------------------------------------------------------- -------------
          `JavacFactory​(java.util.function.Function<TargetConfiguration,​JavacProvider> javacProvider)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `addP                 | ::: block             |
        |                       | arseTimeDeps​(com.goog | Adds the parse time   |
        |                       | le.common.collect.Imm | deps required for     |
        |                       | utableCollection.Buil | javac based on the    |
        |                       | der<BuildTarget> targ | args.                 |
        |                       | etGraphOnlyDepsBuilde | :::                   |
        |                       | r,                 Jv |                       |
        |                       | mLibraryArg args,     |                       |
        |                       |              TargetCo |                       |
        |                       | nfiguration toolchain |                       |
        |                       | TargetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Javac`               | `create​(SourcePath    | ::: block             |
        |                       | RuleFinder ruleFinder | Returns either the    |
        |                       | ,       JvmLibraryArg | defautl javac or one  |
        |                       |  args,       TargetCo | created from the      |
        |                       | nfiguration toolchain | provided args.        |
        |                       | TargetConfiguration)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.goog             | `get                  |                       |
        | le.common.collect.Imm | BuildDeps​(SourcePathR |                       |
        | utableSet<BuildRule>` | uleFinder ruleFinder, |                       |
        |                       |              TargetCo |                       |
        |                       | nfiguration toolchain |                       |
        |                       | TargetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static JavacFactory` | `getDef               | ::: block             |
        |                       | ault​(ToolchainProvide | Creates a             |
        |                       | r toolchainProvider)` | JavacFactory for the  |
        |                       |                       | default Java          |
        |                       |                       | toolchain.            |
        |                       |                       | :::                   |
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

        []{#<init>(java.util.function.Function)}

        -   #### JavacFactory

                public JavacFactory​(java.util.function.Function<TargetConfiguration,​JavacProvider> javacProvider)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#create(com.facebook.buck.core.rules.SourcePathRuleFinder,com.facebook.buck.jvm.java.JvmLibraryArg,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### create

            ``` methodSignature
            public Javac create​(SourcePathRuleFinder ruleFinder,
                                @Nullable
                                JvmLibraryArg args,
                                TargetConfiguration toolchainTargetConfiguration)
            ```

            ::: block
            Returns either the defautl javac or one created from the
            provided args.
            :::

        []{#getDefault(com.facebook.buck.core.toolchain.ToolchainProvider)}

        -   #### getDefault

            ``` methodSignature
            public static JavacFactory getDefault​(ToolchainProvider toolchainProvider)
            ```

            ::: block
            Creates a JavacFactory for the default Java toolchain.
            :::

        []{#addParseTimeDeps(com.google.common.collect.ImmutableCollection.Builder,com.facebook.buck.jvm.java.JvmLibraryArg,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### addParseTimeDeps

            ``` methodSignature
            public void addParseTimeDeps​(com.google.common.collect.ImmutableCollection.Builder<BuildTarget> targetGraphOnlyDepsBuilder,
                                         @Nullable
                                         JvmLibraryArg args,
                                         TargetConfiguration toolchainTargetConfiguration)
            ```

            ::: block
            Adds the parse time deps required for javac based on the
            args. If the args has a spec for javac, we assume that the
            parse time deps will be derived elsewhere.
            :::

        []{#getBuildDeps(com.facebook.buck.core.rules.SourcePathRuleFinder,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getBuildDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<BuildRule> getBuildDeps​(SourcePathRuleFinder ruleFinder,
                                                                                  TargetConfiguration toolchainTargetConfiguration)
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

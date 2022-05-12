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
-   [Nested](#nested.class.summary) \| 
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.rules.coercer](package-summary.html)
:::

## Class SourceSet {#class-sourceset .title title="Class SourceSet"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.coercer.SourceSet

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`, `TargetTranslatable<SourceSet>`

    ------------------------------------------------------------------------

        public abstract class SourceSet
        extends Object
        implements TargetTranslatable<SourceSet>, AddsToRuleKey

    ::: block
    A group of ordered sources, stored as either a
    [`Set`](http://docs.oracle.com/javase/7/docs/api/java/util/Set.html?is-external=true "class or interface in java.util"){.externalLink}
    of unnamed
    [`SourcePath`](../../core/sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")s
    or a
    [`Map`](http://docs.oracle.com/javase/7/docs/api/java/util/Map.html?is-external=true "class or interface in java.util"){.externalLink}
    of names to
    [`SourcePath`](../../core/sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")s.
    Commonly used to represent the input `srcs` parameter of rules where
    source \"names\" may be important (e.g. to control layout of C++
    headers).
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class              Description
          ------------------- ------------------ -------------
          `static class `     `SourceSet.Type`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type    Field     Description
          -------------------- --------- -------------
          `static SourceSet`   `EMPTY`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor     Description
          --------------- -------------
          `SourceSet()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `protected void`      | `check()`             |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static SourceSet`    | `concat​(Iterable<     | ::: block             |
        |                       | SourceSet> elements)` | Concatenates elements |
        |                       |                       | of the given lists    |
        |                       |                       | into a single list.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Optio       | `getNamedSources()`   |                       |
        | nal<com.google.common |                       |                       |
        | .collect.ImmutableMap |                       |                       |
        | <String,​SourcePath>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `getPaths()`          |                       |
        | .common.collect.Immut |                       |                       |
        | ableList<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abs                  | `getType()`           |                       |
        | tract SourceSet.Type` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstrac              | `getUnnamedSources()` |                       |
        | t Optional<com.google |                       |                       |
        | .common.collect.Immut |                       |                       |
        | ableSet<SourcePath>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isEmpty()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static SourceSet`    | `of​(SourceSet.Type    |                       |
        |                       | type,   Optional<? ex |                       |
        |                       | tends com.google.comm |                       |
        |                       | on.collect.ImmutableS |                       |
        |                       | et<SourcePath>> unnam |                       |
        |                       | edSources,   Optional |                       |
        |                       | <? extends com.google |                       |
        |                       | .common.collect.Immut |                       |
        |                       | ableMap<String,​Source |                       |
        |                       | Path>> namedSources)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static SourceSet`    | `ofN                  |                       |
        |                       | amedSources​(com.googl |                       |
        |                       | e.common.collect.Immu |                       |
        |                       | tableMap<String,​Sourc |                       |
        |                       | ePath> namedSources)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static SourceSet`    | `                     |                       |
        |                       | ofUnnamedSources​(com. |                       |
        |                       | google.common.collect |                       |
        |                       | .ImmutableSet<SourceP |                       |
        |                       | ath> unnamedSources)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `toNameMap​(           |                       |
        | n.collect.ImmutableMa | BuildTarget buildTarg |                       |
        | p<String,​SourcePath>` | et,          SourcePa |                       |
        |                       | thResolverAdapter pat |                       |
        |                       | hResolver,          S |                       |
        |                       | tring parameterName)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `toNameMap​(Bui        |                       |
        | n.collect.ImmutableMa | ldTarget buildTarget, |                       |
        | p<String,​SourcePath>` |           SourcePathR |                       |
        |                       | esolverAdapter pathRe |                       |
        |                       | solver,          Stri |                       |
        |                       | ng parameterName,     |                       |
        |                       |       java.util.funct |                       |
        |                       | ion.Predicate<SourceP |                       |
        |                       | ath> filter,          |                       |
        |                       |  java.util.function.F |                       |
        |                       | unction<SourcePath,​So |                       |
        |                       | urcePath> transform)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<SourceSet>` | `translateTargets     |                       |
        |                       | ​(CellNameResolver cel |                       |
        |                       | lPathResolver,        |                       |
        |                       |           BaseName ta |                       |
        |                       | rgetBaseName,         |                       |
        |                       |          TargetNodeTr |                       |
        |                       | anslator translator)` |                       |
        +-----------------------+-----------------------+-----------------------+

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
    -   []{#field.detail}

        ### Field Detail

        []{#EMPTY}

        -   #### EMPTY

                public static final SourceSet EMPTY
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### SourceSet

                public SourceSet()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getType()}

        -   #### getType

            ``` methodSignature
            public abstract SourceSet.Type getType()
            ```

        []{#getUnnamedSources()}

        -   #### getUnnamedSources

            ``` methodSignature
            public abstract Optional<com.google.common.collect.ImmutableSet<SourcePath>> getUnnamedSources()
            ```

        []{#getNamedSources()}

        -   #### getNamedSources

            ``` methodSignature
            public abstract Optional<com.google.common.collect.ImmutableMap<String,​SourcePath>> getNamedSources()
            ```

        []{#check()}

        -   #### check

            ``` methodSignature
            @Check
            protected void check()
            ```

        []{#ofUnnamedSources(com.google.common.collect.ImmutableSet)}

        -   #### ofUnnamedSources

            ``` methodSignature
            public static SourceSet ofUnnamedSources​(com.google.common.collect.ImmutableSet<SourcePath> unnamedSources)
            ```

        []{#ofNamedSources(com.google.common.collect.ImmutableMap)}

        -   #### ofNamedSources

            ``` methodSignature
            public static SourceSet ofNamedSources​(com.google.common.collect.ImmutableMap<String,​SourcePath> namedSources)
            ```

        []{#isEmpty()}

        -   #### isEmpty

            ``` methodSignature
            public boolean isEmpty()
            ```

        []{#toNameMap(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,java.lang.String,java.util.function.Predicate,java.util.function.Function)}

        -   #### toNameMap

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​SourcePath> toNameMap​(BuildTarget buildTarget,
                                                                                             SourcePathResolverAdapter pathResolver,
                                                                                             String parameterName,
                                                                                             java.util.function.Predicate<SourcePath> filter,
                                                                                             java.util.function.Function<SourcePath,​SourcePath> transform)
            ```

        []{#toNameMap(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,java.lang.String)}

        -   #### toNameMap

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​SourcePath> toNameMap​(BuildTarget buildTarget,
                                                                                             SourcePathResolverAdapter pathResolver,
                                                                                             String parameterName)
            ```

        []{#getPaths()}

        -   #### getPaths

            ``` methodSignature
            public com.google.common.collect.ImmutableList<SourcePath> getPaths()
            ```

        []{#translateTargets(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.core.model.BaseName,com.facebook.buck.versions.TargetNodeTranslator)}

        -   #### translateTargets

            ``` methodSignature
            public Optional<SourceSet> translateTargets​(CellNameResolver cellPathResolver,
                                                        BaseName targetBaseName,
                                                        TargetNodeTranslator translator)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `translateTargets` in
                interface `TargetTranslatable<SourceSet>`

            [Returns:]{.returnLabel}
            :   if any changes are required, return the translated
                object.

        []{#concat(java.lang.Iterable)}

        -   #### concat

            ``` methodSignature
            public static SourceSet concat​(Iterable<SourceSet> elements)
            ```

            ::: block
            Concatenates elements of the given lists into a single list.
            :::

        []{#of(com.facebook.buck.rules.coercer.SourceSet.Type,java.util.Optional,java.util.Optional)}

        -   #### of

            ``` methodSignature
            public static SourceSet of​(SourceSet.Type type,
                                       Optional<? extends com.google.common.collect.ImmutableSet<SourcePath>> unnamedSources,
                                       Optional<? extends com.google.common.collect.ImmutableMap<String,​SourcePath>> namedSources)
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
-   [Nested](#nested.class.summary) \| 
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

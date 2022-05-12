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

## Class SourceSortedSet {#class-sourcesortedset .title title="Class SourceSortedSet"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.coercer.SourceSortedSet

::: description
-   

    All Implemented Interfaces:
    :   `TargetTranslatable<SourceSortedSet>`

    ------------------------------------------------------------------------

        public abstract class SourceSortedSet
        extends Object
        implements TargetTranslatable<SourceSortedSet>

    ::: block
    A group of sources, stored as either a
    [`SortedSet`](http://docs.oracle.com/javase/7/docs/api/java/util/SortedSet.html?is-external=true "class or interface in java.util"){.externalLink}
    of unnamed
    [`SourcePath`](../../core/sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")s
    or a
    [`SortedMap`](http://docs.oracle.com/javase/7/docs/api/java/util/SortedMap.html?is-external=true "class or interface in java.util"){.externalLink}
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

          Modifier and Type   Class                    Description
          ------------------- ------------------------ -------------
          `static class `     `SourceSortedSet.Type`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type          Field     Description
          -------------------------- --------- -------------
          `static SourceSortedSet`   `EMPTY`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor           Description
          --------------------- -------------
          `SourceSortedSet()`    

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
        | `st                   | `c                    | ::: block             |
        | atic SourceSortedSet` | oncat​(Iterable<Source | Concatenates elements |
        |                       | SortedSet> elements)` | of the given lists    |
        |                       |                       | into a single list.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Optional<co | `getNamedSources()`   |                       |
        | m.google.common.colle |                       |                       |
        | ct.ImmutableSortedMap |                       |                       |
        | <String,​SourcePath>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `getPaths()`          |                       |
        | .common.collect.Immut |                       |                       |
        | ableList<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract             | `getType()`           |                       |
        | SourceSortedSet.Type` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Opti        | `getUnnamedSources()` |                       |
        | onal<com.google.commo |                       |                       |
        | n.collect.ImmutableSo |                       |                       |
        | rtedSet<SourcePath>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isEmpty()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `of​(SourceSorted      |                       |
        | atic SourceSortedSet` | Set.Type type,   Opti |                       |
        |                       | onal<? extends com.go |                       |
        |                       | ogle.common.collect.I |                       |
        |                       | mmutableSortedSet<Sou |                       |
        |                       | rcePath>> unnamedSour |                       |
        |                       | ces,   Optional<? ext |                       |
        |                       | ends com.google.commo |                       |
        |                       | n.collect.ImmutableSo |                       |
        |                       | rtedMap<String,​Source |                       |
        |                       | Path>> namedSources)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `ofNamedSo            |                       |
        | atic SourceSortedSet` | urces​(com.google.comm |                       |
        |                       | on.collect.ImmutableS |                       |
        |                       | ortedMap<String,​Sourc |                       |
        |                       | ePath> namedSources)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `ofUnna               |                       |
        | atic SourceSortedSet` | medSources​(com.google |                       |
        |                       | .common.collect.Immut |                       |
        |                       | ableSortedSet<SourceP |                       |
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
        | `Optio                | `translateTargets     |                       |
        | nal<SourceSortedSet>` | ​(CellNameResolver cel |                       |
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

                public static final SourceSortedSet EMPTY
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### SourceSortedSet

                public SourceSortedSet()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getType()}

        -   #### getType

            ``` methodSignature
            public abstract SourceSortedSet.Type getType()
            ```

        []{#getUnnamedSources()}

        -   #### getUnnamedSources

            ``` methodSignature
            public abstract Optional<com.google.common.collect.ImmutableSortedSet<SourcePath>> getUnnamedSources()
            ```

        []{#getNamedSources()}

        -   #### getNamedSources

            ``` methodSignature
            public abstract Optional<com.google.common.collect.ImmutableSortedMap<String,​SourcePath>> getNamedSources()
            ```

        []{#check()}

        -   #### check

            ``` methodSignature
            @Check
            protected void check()
            ```

        []{#ofUnnamedSources(com.google.common.collect.ImmutableSortedSet)}

        -   #### ofUnnamedSources

            ``` methodSignature
            public static SourceSortedSet ofUnnamedSources​(com.google.common.collect.ImmutableSortedSet<SourcePath> unnamedSources)
            ```

        []{#ofNamedSources(com.google.common.collect.ImmutableSortedMap)}

        -   #### ofNamedSources

            ``` methodSignature
            public static SourceSortedSet ofNamedSources​(com.google.common.collect.ImmutableSortedMap<String,​SourcePath> namedSources)
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
            public Optional<SourceSortedSet> translateTargets​(CellNameResolver cellPathResolver,
                                                              BaseName targetBaseName,
                                                              TargetNodeTranslator translator)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `translateTargets` in
                interface `TargetTranslatable<SourceSortedSet>`

            [Returns:]{.returnLabel}
            :   if any changes are required, return the translated
                object.

        []{#concat(java.lang.Iterable)}

        -   #### concat

            ``` methodSignature
            public static SourceSortedSet concat​(Iterable<SourceSortedSet> elements)
            ```

            ::: block
            Concatenates elements of the given lists into a single list.
            :::

        []{#of(com.facebook.buck.rules.coercer.SourceSortedSet.Type,java.util.Optional,java.util.Optional)}

        -   #### of

            ``` methodSignature
            public static SourceSortedSet of​(SourceSortedSet.Type type,
                                             Optional<? extends com.google.common.collect.ImmutableSortedSet<SourcePath>> unnamedSources,
                                             Optional<? extends com.google.common.collect.ImmutableSortedMap<String,​SourcePath>> namedSources)
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

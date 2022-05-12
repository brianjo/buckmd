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
[Package]{.packageLabelInType} [com.facebook.buck.cxx](package-summary.html)
:::

## Class CxxFlags {#class-cxxflags .title title="Class CxxFlags"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.CxxFlags

::: description
-   

    ------------------------------------------------------------------------

        public class CxxFlags
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `CxxFlags.Transla     | ::: block             |
        |                       | teMacrosArgsFunction` | Function for          |
        |                       |                       | translating cxx flag  |
        |                       |                       | macros in list of     |
        |                       |                       | Arg.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `CxxFlags.Tra         | ::: block             |
        |                       | nslateMacrosFunction` | Function for          |
        |                       |                       | translating cxx flag  |
        |                       |                       | macros.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static <T> c         | `getFlags​(com.        |                       |
        | om.google.common.coll | google.common.collect |                       |
        | ect.ImmutableList<T>` | .ImmutableList<T> fla |                       |
        |                       | gs,         PatternMa |                       |
        |                       | tchedCollection<com.g |                       |
        |                       | oogle.common.collect. |                       |
        |                       | ImmutableList<T>> pla |                       |
        |                       | tformFlags,         C |                       |
        |                       | xxPlatform platform)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `getF                 |                       |
        | atic com.google.commo | lagsWithMacrosWithPla |                       |
        | n.collect.ImmutableLi | tformMacroExpansion​(c |                       |
        | st<StringWithMacros>` | om.google.common.coll |                       |
        |                       | ect.ImmutableList<Str |                       |
        |                       | ingWithMacros> flags, |                       |
        |                       |                       |                       |
        |                       |                       |                       |
        |                       |    PatternMatchedColl |                       |
        |                       | ection<com.google.com |                       |
        |                       | mon.collect.Immutable |                       |
        |                       | List<StringWithMacros |                       |
        |                       | >> platformFlags,     |                       |
        |                       |                       |                       |
        |                       |                     C |                       |
        |                       | xxPlatform platform)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static com.go        | `getFlagsWithPlatf    |                       |
        | ogle.common.collect.I | ormMacroExpansion​(com |                       |
        | mmutableList<String>` | .google.common.collec |                       |
        |                       | t.ImmutableList<Strin |                       |
        |                       | g> flags,             |                       |
        |                       |                       |                       |
        |                       |   PatternMatchedColle |                       |
        |                       | ction<com.google.comm |                       |
        |                       | on.collect.ImmutableL |                       |
        |                       | ist<String>> platform |                       |
        |                       | Flags,                |                       |
        |                       |                     C |                       |
        |                       | xxPlatform platform)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static com.goog      | `getLanguageFl        |                       |
        | le.common.collect.Imm | ags​(com.google.common |                       |
        | utableListMultimap<Cx | .collect.ImmutableLis |                       |
        | xSource.Type,​String>` | t<String> flags,      |                       |
        |                       |             PatternMa |                       |
        |                       | tchedCollection<com.g |                       |
        |                       | oogle.common.collect. |                       |
        |                       | ImmutableList<String> |                       |
        |                       | > platformFlags,      |                       |
        |                       |             com.googl |                       |
        |                       | e.common.collect.Immu |                       |
        |                       | tableMap<CxxSource.Ty |                       |
        |                       | pe,​com.google.common. |                       |
        |                       | collect.ImmutableList |                       |
        |                       | <String>> languageFla |                       |
        |                       | gs,                 C |                       |
        |                       | xxPlatform platform)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `stat                 | `                     |                       |
        | ic com.google.common. | getLanguageFlagsWithM |                       |
        | collect.ImmutableList | acros​(com.google.comm |                       |
        | Multimap<CxxSource.Ty | on.collect.ImmutableL |                       |
        | pe,​StringWithMacros>` | ist<StringWithMacros> |                       |
        |                       |  flags,               |                       |
        |                       |              PatternM |                       |
        |                       | atchedCollection<com. |                       |
        |                       | google.common.collect |                       |
        |                       | .ImmutableList<String |                       |
        |                       | WithMacros>> platform |                       |
        |                       | Flags,                |                       |
        |                       |             com.googl |                       |
        |                       | e.common.collect.Immu |                       |
        |                       | tableMap<CxxSource.Ty |                       |
        |                       | pe,​? extends Collecti |                       |
        |                       | on<StringWithMacros>> |                       |
        |                       |  languageFlags,       |                       |
        |                       |                       |                       |
        |                       | com.google.common.col |                       |
        |                       | lect.ImmutableMap<Cxx |                       |
        |                       | Source.Type,​PatternMa |                       |
        |                       | tchedCollection<com.g |                       |
        |                       | oogle.common.collect. |                       |
        |                       | ImmutableList<StringW |                       |
        |                       | ithMacros>>> language |                       |
        |                       | PlatformFlags,        |                       |
        |                       |                     C |                       |
        |                       | xxPlatform platform)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `translateCxxPla      | ::: block             |
        |                       | tformFlags​(CxxPlatfor | Expand flag macros in |
        |                       | m.Builder cxxPlatform | all CxxPlatform       |
        |                       | Builder,              | StringArg flags.      |
        |                       |              CxxPlatf | :::                   |
        |                       | orm cxxPlatform,      |                       |
        |                       |                       |                       |
        |                       | com.google.common.col |                       |
        |                       | lect.ImmutableMap<Str |                       |
        |                       | ing,​Arg> flagMacros)` |                       |
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
    -   []{#method.detail}

        ### Method Detail

        []{#getFlagsWithPlatformMacroExpansion(com.google.common.collect.ImmutableList,com.facebook.buck.rules.coercer.PatternMatchedCollection,com.facebook.buck.cxx.toolchain.CxxPlatform)}

        -   #### getFlagsWithPlatformMacroExpansion

            ``` methodSignature
            public static com.google.common.collect.ImmutableList<String> getFlagsWithPlatformMacroExpansion​(com.google.common.collect.ImmutableList<String> flags,
                                                                                                             PatternMatchedCollection<com.google.common.collect.ImmutableList<String>> platformFlags,
                                                                                                             CxxPlatform platform)
            ```

        []{#getFlagsWithMacrosWithPlatformMacroExpansion(com.google.common.collect.ImmutableList,com.facebook.buck.rules.coercer.PatternMatchedCollection,com.facebook.buck.cxx.toolchain.CxxPlatform)}

        -   #### getFlagsWithMacrosWithPlatformMacroExpansion

            ``` methodSignature
            public static com.google.common.collect.ImmutableList<StringWithMacros> getFlagsWithMacrosWithPlatformMacroExpansion​(com.google.common.collect.ImmutableList<StringWithMacros> flags,
                                                                                                                                 PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> platformFlags,
                                                                                                                                 CxxPlatform platform)
            ```

        []{#getFlags(com.google.common.collect.ImmutableList,com.facebook.buck.rules.coercer.PatternMatchedCollection,com.facebook.buck.cxx.toolchain.CxxPlatform)}

        -   #### getFlags

            ``` methodSignature
            public static <T> com.google.common.collect.ImmutableList<T> getFlags​(com.google.common.collect.ImmutableList<T> flags,
                                                                                  PatternMatchedCollection<com.google.common.collect.ImmutableList<T>> platformFlags,
                                                                                  CxxPlatform platform)
            ```

        []{#getLanguageFlags(com.google.common.collect.ImmutableList,com.facebook.buck.rules.coercer.PatternMatchedCollection,com.google.common.collect.ImmutableMap,com.facebook.buck.cxx.toolchain.CxxPlatform)}

        -   #### getLanguageFlags

            ``` methodSignature
            public static com.google.common.collect.ImmutableListMultimap<CxxSource.Type,​String> getLanguageFlags​(com.google.common.collect.ImmutableList<String> flags,
                                                                                                                        PatternMatchedCollection<com.google.common.collect.ImmutableList<String>> platformFlags,
                                                                                                                        com.google.common.collect.ImmutableMap<CxxSource.Type,​com.google.common.collect.ImmutableList<String>> languageFlags,
                                                                                                                        CxxPlatform platform)
            ```

        []{#getLanguageFlagsWithMacros(com.google.common.collect.ImmutableList,com.facebook.buck.rules.coercer.PatternMatchedCollection,com.google.common.collect.ImmutableMap,com.google.common.collect.ImmutableMap,com.facebook.buck.cxx.toolchain.CxxPlatform)}

        -   #### getLanguageFlagsWithMacros

            ``` methodSignature
            public static com.google.common.collect.ImmutableListMultimap<CxxSource.Type,​StringWithMacros> getLanguageFlagsWithMacros​(com.google.common.collect.ImmutableList<StringWithMacros> flags,
                                                                                                                                            PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>> platformFlags,
                                                                                                                                            com.google.common.collect.ImmutableMap<CxxSource.Type,​? extends Collection<StringWithMacros>> languageFlags,
                                                                                                                                            com.google.common.collect.ImmutableMap<CxxSource.Type,​PatternMatchedCollection<com.google.common.collect.ImmutableList<StringWithMacros>>> languagePlatformFlags,
                                                                                                                                            CxxPlatform platform)
            ```

        []{#translateCxxPlatformFlags(com.facebook.buck.cxx.toolchain.CxxPlatform.Builder,com.facebook.buck.cxx.toolchain.CxxPlatform,com.google.common.collect.ImmutableMap)}

        -   #### translateCxxPlatformFlags

            ``` methodSignature
            public static void translateCxxPlatformFlags​(CxxPlatform.Builder cxxPlatformBuilder,
                                                         CxxPlatform cxxPlatform,
                                                         com.google.common.collect.ImmutableMap<String,​Arg> flagMacros)
            ```

            ::: block
            Expand flag macros in all CxxPlatform StringArg flags.
            :::
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

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

## Class CxxGenruleFilterAndTargetsMacro {#class-cxxgenrulefilterandtargetsmacro .title title="Class CxxGenruleFilterAndTargetsMacro"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.macros.CxxGenruleFilterAndTargetsMacro

::: description
-   

    All Implemented Interfaces:
    :   `Macro`, `TargetTranslatable<Macro>`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `CppFlagsMacro`, `CxxppFlagsMacro`, `LdflagsSharedFilterMacro`,
        `LdflagsSharedMacro`, `LdflagsStaticFilterMacro`,
        `LdflagsStaticMacro`, `LdflagsStaticPicFilterMacro`,
        `LdflagsStaticPicMacro`

    ------------------------------------------------------------------------

        public abstract class CxxGenruleFilterAndTargetsMacro
        extends Object
        implements Macro

    ::: block
    Base class for `cxx_genrule` flags-based macros.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                           Description
          ------------------------------------- -------------
          `CxxGenruleFilterAndTargetsMacro()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                 Method                                                                                                                                            Description
          ----------------------------------------------------------------- ------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `abstract Optional<Pattern>`                                      `getFilter()`                                                                                                                                      
          `abstract com.google.common.collect.ImmutableList<BuildTarget>`   `getTargets()`                                                                                                                                     
          `Optional<Macro>`                                                 `translateTargets​(CellNameResolver cellPathResolver,                 BaseName targetBaseName,                 TargetNodeTranslator translator)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.rules.macros.Macro}

            ### Methods inherited from interface com.facebook.buck.rules.macros.[Macro](Macro.html "interface in com.facebook.buck.rules.macros")

            `getMacroClass`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### CxxGenruleFilterAndTargetsMacro

                public CxxGenruleFilterAndTargetsMacro()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getFilter()}

        -   #### getFilter

            ``` methodSignature
            public abstract Optional<Pattern> getFilter()
            ```

        []{#getTargets()}

        -   #### getTargets

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<BuildTarget> getTargets()
            ```

        []{#translateTargets(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.core.model.BaseName,com.facebook.buck.versions.TargetNodeTranslator)}

        -   #### translateTargets

            ``` methodSignature
            public Optional<Macro> translateTargets​(CellNameResolver cellPathResolver,
                                                    BaseName targetBaseName,
                                                    TargetNodeTranslator translator)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `translateTargets` in interface `Macro`

            [Specified by:]{.overrideSpecifyLabel}
            :   `translateTargets` in
                interface `TargetTranslatable<Macro>`

            [Returns:]{.returnLabel}
            :   if any changes are required, return the translated
                object.
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

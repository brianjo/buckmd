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
-   Package
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

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
# Package com.facebook.buck.core.macros {#package-com.facebook.buck.core.macros .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [MacroCombiner](Mac               | ::: block                         |
    | roCombiner.html "interface in com | Used by MacroFinder to process a  |
    | .facebook.buck.core.macros")\<T\> | string containing macros.         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [MacroMatchResult](M              |                                   |
    | acroMatchResult.html "interface i |                                   |
    | n com.facebook.buck.core.macros") |                                   |
    +-----------------------------------+-----------------------------------+
    | [MacroReplacer](Mac               | ::: block                         |
    | roReplacer.html "interface in com | Interface to define replacement   |
    | .facebook.buck.core.macros")\<T\> | behavior for \@{link              |
    |                                   | MacroFinder}.                     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [Macro                            | ::: block                         |
    | Finder](MacroFinder.html "class i | Replace and extracts macros from  |
    | n com.facebook.buck.core.macros") | input strings.                    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [MacroFinderAutomaton](M          | ::: block                         |
    | acroFinderAutomaton.html "class i | A push-down automaton that        |
    | n com.facebook.buck.core.macros") | searches for occurrences of a     |
    |                                   | macro in linear time with respect |
    |                                   | to the search string.             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [StringMacroCombiner](            | ::: block                         |
    | StringMacroCombiner.html "class i | A simple MacroCombiner for        |
    | n com.facebook.buck.core.macros") | `MacroReplacer<String>` that just |
    |                                   | concatenates the strings and      |
    |                                   | expanded macros.                  |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   
      Exception                                                                        Description
      -------------------------------------------------------------------------------- -------------
      [MacroException](MacroException.html "class in com.facebook.buck.core.macros")    

      : Exception Summary[ ]{.tabEnd}
:::
:::

::: bottomNav
[]{#navbar.bottom}

::: skipNav
[Skip navigation links](#skip.navbar.bottom "Skip navigation links")
:::

[]{#navbar.bottom.firstrow}

-   [Overview](../../../../../index.html)
-   Package
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

[]{#skip.navbar.bottom}
:::

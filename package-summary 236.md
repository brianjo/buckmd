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
# Package com.facebook.buck.core.select {#package-com.facebook.buck.core.select .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [ProvidesSelectable](Pro          | ::: block                         |
    | videsSelectable.html "interface i | Interface indicating that a class |
    | n com.facebook.buck.core.select") | can provide a                     |
    |                                   | [`Selectab                        |
    |                                   | le`](Selectable.html "interface i |
    |                                   | n com.facebook.buck.core.select") |
    |                                   | and its instances can be used as  |
    |                                   | keys in                           |
    |                                   | [`S                               |
    |                                   | elector`](Selector.html "class in |
    |                                   |  com.facebook.buck.core.select"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Selecta                          | ::: block                         |
    | ble](Selectable.html "interface i | A condition in `select`           |
    | n com.facebook.buck.core.select") | statements.                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [SelectableConf                   | ::: block                         |
    | igurationContext](SelectableConfi | Contains context that can be      |
    | gurationContext.html "interface i | accessed by                       |
    | n com.facebook.buck.core.select") | [`Selectab                        |
    |                                   | le`](Selectable.html "interface i |
    |                                   | n com.facebook.buck.core.select") |
    |                                   | to get information about the      |
    |                                   | current configuration.            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [SelectableResolver](Sel          | ::: block                         |
    | ectableResolver.html "interface i | Provides access to instances of   |
    | n com.facebook.buck.core.select") | [`Selectabl                       |
    |                                   | e`](Selectable.html "interface in |
    |                                   |  com.facebook.buck.core.select"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [SelectorListResolver](Selec      | ::: block                         |
    | torListResolver.html "interface i | A resolver that analyzes          |
    | n com.facebook.buck.core.select") | [`SelectorL                       |
    |                                   | ist`](SelectorList.html "class in |
    |                                   |  com.facebook.buck.core.select"), |
    |                                   | evaluates selectable statements   |
    |                                   | and constructs the final value    |
    |                                   | that is produced by concatenating |
    |                                   | selected values (the type of the  |
    |                                   | elements determines the process   |
    |                                   | of concatenation.)                |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [Abstra                           | ::: block                         |
    | ctSelectorListResolver](AbstractS | Provides base functionality for   |
    | electorListResolver.html "class i | selector list resolvers.          |
    | n com.facebook.buck.core.select") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Sele                             | ::: block                         |
    | ctor](Selector.html "class in com | Keeps mapping of a single         |
    | .facebook.buck.core.select")\<T\> | `select` expression.              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Selec                            | ::: block                         |
    | torKey](SelectorKey.html "class i | A key in `select` statement.      |
    | n com.facebook.buck.core.select") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [SelectorList                     | ::: block                         |
    | ](SelectorList.html "class in com | Represents a list of              |
    | .facebook.buck.core.select")\<T\> | [`                                |
    |                                   | Selector`](Selector.html "class i |
    |                                   | n com.facebook.buck.core.select") |
    |                                   | objects                           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}
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

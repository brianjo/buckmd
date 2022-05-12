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
# Package com.facebook.buck.util.timing {#package-com.facebook.buck.util.timing .title title="Package"}
:::

::: contentContainer
-   
      Interface                                                          Description
      ------------------------------------------------------------------ -------------
      [Clock](Clock.html "interface in com.facebook.buck.util.timing")    

      : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [ClockDura                        | ::: block                         |
    | tion](ClockDuration.html "class i | Represents a difference between   |
    | n com.facebook.buck.util.timing") | two time points obtained by       |
    |                                   | [                                 |
    |                                   | `Clock`](Clock.html "interface in |
    |                                   |  com.facebook.buck.util.timing"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Default                          | ::: block                         |
    | Clock](DefaultClock.html "class i | [`Clock`](Clock.html "interface i |
    | n com.facebook.buck.util.timing") | n com.facebook.buck.util.timing") |
    |                                   | implementation that invokes the   |
    |                                   | [`System                          |
    |                                   | `](http://docs.oracle.com/javase/ |
    |                                   | 7/docs/api/java/lang/System.html? |
    |                                   | is-external=true "class or interf |
    |                                   | ace in java.lang"){.externalLink} |
    |                                   | calls.                            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [NanosAdjustedClock]              | ::: block                         |
    | (NanosAdjustedClock.html "class i | [`Clock`](Clock.html "interface i |
    | n com.facebook.buck.util.timing") | n com.facebook.buck.util.timing") |
    |                                   | implementation that invokes the   |
    |                                   | [`System                          |
    |                                   | `](http://docs.oracle.com/javase/ |
    |                                   | 7/docs/api/java/lang/System.html? |
    |                                   | is-external=true "class or interf |
    |                                   | ace in java.lang"){.externalLink} |
    |                                   | calls, adjusted to use the given  |
    |                                   | nanos epoch.                      |
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

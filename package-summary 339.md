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

-   [Overview](../../../../../../../../index.html)
-   Package
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../../index-all.html)
-   [Help](../../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../../allclasses.html)

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
# Package com.facebook.buck.jvm.java.abi.source.api {#package-com.facebook.buck.jvm.java.abi.source.api .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [FrontendOnlyJavacT               |                                   |
    | askProxy](FrontendOnlyJavacTaskPr |                                   |
    | oxy.html "interface in com.facebo |                                   |
    | ok.buck.jvm.java.abi.source.api") |                                   |
    +-----------------------------------+-----------------------------------+
    | [SourceOnlyAbiRuleInfoF           | ::: block                         |
    | actory](SourceOnlyAbiRuleInfoFact | Used to create the                |
    | ory.html "interface in com.facebo | SourceOnlyAbiRuleInfo for a       |
    | ok.buck.jvm.java.abi.source.api") | target given a JavaFileManager.   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [                                 | ::: block                         |
    | SourceOnlyAbiRuleInfoFactory.Sour | Provides information related to   |
    | ceOnlyAbiRuleInfo](SourceOnlyAbiR | source-only abi support.          |
    | uleInfoFactory.SourceOnlyAbiRuleI | :::                               |
    | nfo.html "interface in com.facebo |                                   |
    | ok.buck.jvm.java.abi.source.api") |                                   |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [ErrorSuppressingDiagnosticList   | ::: block                         |
    | ener](ErrorSuppressingDiagnosticL | When running the compiler with    |
    | istener.html "class in com.facebo | some dependencies missing (as     |
    | ok.buck.jvm.java.abi.source.api") | when generating ABIs from         |
    |                                   | source), by default it will abort |
    |                                   | after the last round of           |
    |                                   | annotation processing because it  |
    |                                   | believes there are missing types. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Exception                         | Description                       |
    +===================================+===================================+
    | [Ca                               |                                   |
    | nnotInferException](CannotInferEx |                                   |
    | ception.html "class in com.facebo |                                   |
    | ok.buck.jvm.java.abi.source.api") |                                   |
    +-----------------------------------+-----------------------------------+
    | [SourceCodeWillNotCompileExce     | ::: block                         |
    | ption](SourceCodeWillNotCompileEx | Thrown when a source ABI cannot   |
    | ception.html "class in com.facebo | be generated because the source   |
    | ok.buck.jvm.java.abi.source.api") | code will not compile.            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [StopCompilation](StopComp        | ::: block                         |
    | ilation.html "class in com.facebo | Thrown by our ABI generating      |
    | ok.buck.jvm.java.abi.source.api") | plugin to stop the compiler.      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Exception Summary[ ]{.tabEnd}
:::
:::

::: bottomNav
[]{#navbar.bottom}

::: skipNav
[Skip navigation links](#skip.navbar.bottom "Skip navigation links")
:::

[]{#navbar.bottom.firstrow}

-   [Overview](../../../../../../../../index.html)
-   Package
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../../index-all.html)
-   [Help](../../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

[]{#skip.navbar.bottom}
:::

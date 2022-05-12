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
# Package com.facebook.buck.jvm.core {#package-com.facebook.buck.jvm.core .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [Calculat                         | ::: block                         |
    | eAbi](CalculateAbi.html "interfac | Tag interface for rules that      |
    | e in com.facebook.buck.jvm.core") | calculate ABIs for Java code.     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [HasClasspathDeps                 | ::: block                         |
    | ](HasClasspathDeps.html "interfac | A convenience interface for items |
    | e in com.facebook.buck.jvm.core") | which contribute to the classpath |
    |                                   | of a java packageable.            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [HasClasspathEntries](H           | ::: block                         |
    | asClasspathEntries.html "interfac | Implemented by build rules where  |
    | e in com.facebook.buck.jvm.core") | the output has a classpath        |
    |                                   | environment.                      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [HasDesugarSupport]               | ::: block                         |
    | (HasDesugarSupport.html "interfac | Implemented by build rules that   |
    | e in com.facebook.buck.jvm.core") | support desugar process to the    |
    |                                   | lower java versions, for example  |
    |                                   | java 8 to java 7 desugar for      |
    |                                   | Android builds.                   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [HasJ                             |                                   |
    | avaAbi](HasJavaAbi.html "interfac |                                   |
    | e in com.facebook.buck.jvm.core") |                                   |
    +-----------------------------------+-----------------------------------+
    | [HasJavaClassHashes](             | ::: block                         |
    | HasJavaClassHashes.html "interfac | This should be considered         |
    | e in com.facebook.buck.jvm.core") | deprecated.                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [HasMavenCoordinates](H           |                                   |
    | asMavenCoordinates.html "interfac |                                   |
    | e in com.facebook.buck.jvm.core") |                                   |
    +-----------------------------------+-----------------------------------+
    | [HasS                             | ::: block                         |
    | ources](HasSources.html "interfac | Provides information about        |
    | e in com.facebook.buck.jvm.core") | sources that build rule have.     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JavaAb                           | ::: block                         |
    | iInfo](JavaAbiInfo.html "interfac | Provides information about a java |
    | e in com.facebook.buck.jvm.core") | abi.                              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JavaClassHashesProvider](JavaC   | ::: block                         |
    | lassHashesProvider.html "interfac | Provider that can load java class |
    | e in com.facebook.buck.jvm.core") | hashes from the filesystem.       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JavaLi                           |                                   |
    | brary](JavaLibrary.html "interfac |                                   |
    | e in com.facebook.buck.jvm.core") |                                   |
    +-----------------------------------+-----------------------------------+
    | [JavaPackageFinder]               |                                   |
    | (JavaPackageFinder.html "interfac |                                   |
    | e in com.facebook.buck.jvm.core") |                                   |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [DefaultJavaAbiIn                 | ::: block                         |
    | fo](DefaultJavaAbiInfo.html "clas | The default inmplementation of    |
    | s in com.facebook.buck.jvm.core") | JavaAbiInfo.                      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [EmptyJavaAbi                     | ::: block                         |
    | Info](EmptyJavaAbiInfo.html "clas | The implementation of JavaAbiInfo |
    | s in com.facebook.buck.jvm.core") | for targets that have no sources. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JavaAbis](JavaAbis.html "clas    | ::: block                         |
    | s in com.facebook.buck.jvm.core") | Provides some utilities for       |
    |                                   | dealing with Java abis and abi    |
    |                                   | rules.                            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [JavaLibrary.                     |                                   |
    | Data](JavaLibrary.Data.html "clas |                                   |
    | s in com.facebook.buck.jvm.core") |                                   |
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

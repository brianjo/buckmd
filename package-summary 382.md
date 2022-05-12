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

-   [Overview](../../../../../../../index.html)
-   Package
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
# Package com.facebook.buck.jvm.java.plugin.api {#package-com.facebook.buck.jvm.java.plugin.api .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [Buck                             | ::: block                         |
    | JavacTaskListener](BuckJavacTaskL | Listens to events coming from the |
    | istener.html "interface in com.fa | Java compiler.                    |
    | cebook.buck.jvm.java.plugin.api") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuckJavacTaskProxy](BuckJavacTa  | ::: block                         |
    | skProxy.html "interface in com.fa | `JavacTask` is included with the  |
    | cebook.buck.jvm.java.plugin.api") | compiler and is thus not directly |
    |                                   | accessible from within Buck\'s    |
    |                                   | class loader.                     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Compilatio                       | ::: block                         |
    | nUnitTreeProxy](CompilationUnitTr | `CompilationUnitTree` is included |
    | eeProxy.html "interface in com.fa | with the compiler and is thus not |
    | cebook.buck.jvm.java.plugin.api") | directly accessible from within   |
    |                                   | Buck\'s class loader.             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PluginClassLoader](PluginClas    | ::: block                         |
    | sLoader.html "interface in com.fa | Utility interface for loading     |
    | cebook.buck.jvm.java.plugin.api") | classes that live in Buck\'s Java |
    |                                   | compiler plugin.                  |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PluginClas                       | ::: block                         |
    | sLoaderFactory](PluginClassLoader | Factory interface for             |
    | Factory.html "interface in com.fa | [`PluginClassLoader`](PluginClass |
    | cebook.buck.jvm.java.plugin.api") | Loader.html "interface in com.fac |
    |                                   | ebook.buck.jvm.java.plugin.api")s |
    |                                   | for different compiler instances  |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [TaskEventMirror](Task            | ::: block                         |
    | EventMirror.html "class in com.fa | `TaskEvent` is included with the  |
    | cebook.buck.jvm.java.plugin.api") | compiler and is thus not directly |
    |                                   | accessible from within Buck\'s    |
    |                                   | class loader.                     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   
      Enum                                                                                                Description
      --------------------------------------------------------------------------------------------------- -------------
      [TaskEventMirror.Kind](TaskEventMirror.Kind.html "enum in com.facebook.buck.jvm.java.plugin.api")    

      : Enum Summary[ ]{.tabEnd}
:::
:::

::: bottomNav
[]{#navbar.bottom}

::: skipNav
[Skip navigation links](#skip.navbar.bottom "Skip navigation links")
:::

[]{#navbar.bottom.firstrow}

-   [Overview](../../../../../../../index.html)
-   Package
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

[]{#skip.navbar.bottom}
:::

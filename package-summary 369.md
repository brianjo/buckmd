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
# Package com.facebook.buck.jvm.java.plugin.adapter {#package-com.facebook.buck.jvm.java.plugin.adapter .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [BuckJavacPlugin](BuckJavacPlu    | ::: block                         |
    | gin.html "interface in com.facebo | Analogue to javac 8\'s `Plugin`   |
    | ok.buck.jvm.java.plugin.adapter") | class for use within Buck, even   |
    |                                   | on older versions of javac.       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [BridgeMethods](Bridge            |                                   |
    | Methods.html "class in com.facebo |                                   |
    | ok.buck.jvm.java.plugin.adapter") |                                   |
    +-----------------------------------+-----------------------------------+
    | [BuckJavacTask](BuckJa            | ::: block                         |
    | vacTask.html "class in com.facebo | Extends `JavacTask` with          |
    | ok.buck.jvm.java.plugin.adapter") | functionality that is useful for  |
    |                                   | Buck: Exposes the enter method    |
    |                                   | from JavacTaskImpl Pre-javac-8    |
    |                                   | support for                       |
    |                                   | a                                 |
    |                                   | ddTaskListener/removeTaskListener |
    |                                   | Wraps                             |
    |                                   | [`E                               |
    |                                   | lements`](http://docs.oracle.com/ |
    |                                   | javase/7/docs/api/javax/lang/mode |
    |                                   | l/util/Elements.html?is-external= |
    |                                   | true "class or interface in javax |
    |                                   | .lang.model.util"){.externalLink} |
    |                                   | with some extended functionality  |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuckJavacTaskL                   | ::: block                         |
    | istenerProxy](BuckJavacTaskListen | Implements `TaskListener` by      |
    | erProxy.html "class in com.facebo | proxying calls to an inner        |
    | ok.buck.jvm.java.plugin.adapter") | [`BuckJavacTask                   |
    |                                   | Listener`](../api/BuckJavacTaskLi |
    |                                   | stener.html "interface in com.fac |
    |                                   | ebook.buck.jvm.java.plugin.api"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuckJa                           | ::: block                         |
    | vacTaskProxyImpl](BuckJavacTaskPr | NOTE: A Java8 copy of this file   |
    | oxyImpl.html "class in com.facebo | exists in                         |
    | ok.buck.jvm.java.plugin.adapter") | ../j                              |
    |                                   | ava8/BuckJavacTaskProxyImpl.java. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CompilationUnitTre               |                                   |
    | eProxyImpl](CompilationUnitTreePr |                                   |
    | oxyImpl.html "class in com.facebo |                                   |
    | ok.buck.jvm.java.plugin.adapter") |                                   |
    +-----------------------------------+-----------------------------------+
    | [El                               | ::: block                         |
    | ementsExtendedImpl](ElementsExten | Wraps and extends                 |
    | dedImpl.html "class in com.facebo | [`E                               |
    | ok.buck.jvm.java.plugin.adapter") | lements`](http://docs.oracle.com/ |
    |                                   | javase/7/docs/api/javax/lang/mode |
    |                                   | l/util/Elements.html?is-external= |
    |                                   | true "class or interface in javax |
    |                                   | .lang.model.util"){.externalLink} |
    |                                   | with methods that cannot be added |
    |                                   | as pure extension methods on      |
    |                                   | [`                                |
    |                                   | MoreElements`](../../lang/model/M |
    |                                   | oreElements.html "class in com.fa |
    |                                   | cebook.buck.jvm.java.lang.model") |
    |                                   | because they require per-instance |
    |                                   | state.                            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Post                             | ::: block                         |
    | EnterTaskListener](PostEnterTaskL | A `TaskListener` that runs some   |
    | istener.html "class in com.facebo | code after the final enter phase. |
    | ok.buck.jvm.java.plugin.adapter") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [TaskListenerProxy](TaskListen    | ::: block                         |
    | erProxy.html "class in com.facebo | Implements                        |
    | ok.buck.jvm.java.plugin.adapter") | [`BuckJavacTas                    |
    |                                   | kListener`](../api/BuckJavacTaskL |
    |                                   | istener.html "interface in com.fa |
    |                                   | cebook.buck.jvm.java.plugin.api") |
    |                                   | by proxying calls to an inner     |
    |                                   | `TaskListener`.                   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [                                 |                                   |
    | TaskListenerWrapper](TaskListener |                                   |
    | Wrapper.html "class in com.facebo |                                   |
    | ok.buck.jvm.java.plugin.adapter") |                                   |
    +-----------------------------------+-----------------------------------+
    | [TreesMessager](TreesM            |                                   |
    | essager.html "class in com.facebo |                                   |
    | ok.buck.jvm.java.plugin.adapter") |                                   |
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

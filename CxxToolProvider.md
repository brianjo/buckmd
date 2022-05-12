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
[Package]{.packageLabelInType} [com.facebook.buck.cxx.toolchain](package-summary.html)
:::

## Class CxxToolProvider\<T\> {#class-cxxtoolprovidert .title title="Class CxxToolProvider"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.toolchain.CxxToolProvider\<T\>

::: description
-   

    Direct Known Subclasses:
    :   `CompilerProvider`, `PreprocessorProvider`

    ------------------------------------------------------------------------

        public abstract class CxxToolProvider<T>
        extends Object

    ::: block
    A provide for the
    [`Preprocessor`](Preprocessor.html "interface in com.facebook.buck.cxx.toolchain")
    and
    [`Compiler`](Compiler.html "interface in com.facebook.buck.cxx.toolchain")
    C/C++ drivers.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                    Description
          ------------------- ------------------------ -------------
          `static class `     `CxxToolProvider.Type`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `CxxToolProvider​(Tool             | ::: block                         |
        | Provider toolProvider,            | Build using a                     |
        |      CxxToolProvider.Type type,   | [`ToolProvider`](../../core/too   |
        |               ToolType toolType)` | lchain/toolprovider/ToolProvider. |
        |                                   | html "interface in com.facebook.b |
        |                                   | uck.core.toolchain.toolprovider") |
        |                                   | and a required type.              |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `CxxToolProvider​(ToolProvider too | ::: block                         |
        | lProvider,                CxxTool | Build using a                     |
        | Provider.Type type,               | [`ToolProvider`](../../core/too   |
        |   ToolType toolType,              | lchain/toolprovider/ToolProvider. |
        |    boolean useUnixFileSeparator)` | html "interface in com.facebook.b |
        |                                   | uck.core.toolchain.toolprovider") |
        |                                   | and a required type.              |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `CxxToolProvider​(ToolProvider     |                                   |
        |  toolProvider,                jav |                                   |
        | a.util.function.Supplier<CxxToolP |                                   |
        | rovider.Type> type,               |                                   |
        |   ToolType toolType,              |                                   |
        |    boolean useUnixFileSeparator)` |                                   |
        +-----------------------------------+-----------------------------------+

        : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `                     | `build​(C              |                       |
        | protected abstract T` | xxToolProvider.Type t |                       |
        |                       | ype,      Tool tool)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `I                    | `getParseTimeDeps     |                       |
        | terable<BuildTarget>` | ​(TargetConfiguration  |                       |
        |                       | targetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ToolType`            | `getToolType()`       | ::: block             |
        |                       |                       | Return tool type of   |
        |                       |                       | this provider         |
        |                       |                       | instance              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getUs                |                       |
        |                       | eUnixPathSeparator()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `T`                   | `                     |                       |
        |                       | resolve​(BuildRuleReso |                       |
        |                       | lver resolver,        |                       |
        |                       |  TargetConfiguration  |                       |
        |                       | targetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.toolchain.toolprovider.ToolProvider,java.util.function.Supplier,com.facebook.buck.cxx.toolchain.ToolType,boolean)}

        -   #### CxxToolProvider

                public CxxToolProvider​(ToolProvider toolProvider,
                                       java.util.function.Supplier<CxxToolProvider.Type> type,
                                       ToolType toolType,
                                       boolean useUnixFileSeparator)

        []{#<init>(com.facebook.buck.core.toolchain.toolprovider.ToolProvider,com.facebook.buck.cxx.toolchain.CxxToolProvider.Type,com.facebook.buck.cxx.toolchain.ToolType,boolean)}

        -   #### CxxToolProvider

                public CxxToolProvider​(ToolProvider toolProvider,
                                       CxxToolProvider.Type type,
                                       ToolType toolType,
                                       boolean useUnixFileSeparator)

            ::: block
            Build using a
            [`ToolProvider`](../../core/toolchain/toolprovider/ToolProvider.html "interface in com.facebook.buck.core.toolchain.toolprovider")
            and a required type. It also allows to specify to use Unix
            path separators for the NDK compiler.
            :::

        []{#<init>(com.facebook.buck.core.toolchain.toolprovider.ToolProvider,com.facebook.buck.cxx.toolchain.CxxToolProvider.Type,com.facebook.buck.cxx.toolchain.ToolType)}

        -   #### CxxToolProvider

                public CxxToolProvider​(ToolProvider toolProvider,
                                       CxxToolProvider.Type type,
                                       ToolType toolType)

            ::: block
            Build using a
            [`ToolProvider`](../../core/toolchain/toolprovider/ToolProvider.html "interface in com.facebook.buck.core.toolchain.toolprovider")
            and a required type.
            :::
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#build(com.facebook.buck.cxx.toolchain.CxxToolProvider.Type,com.facebook.buck.core.toolchain.tool.Tool)}

        -   #### build

            ``` methodSignature
            protected abstract T build​(CxxToolProvider.Type type,
                                       Tool tool)
            ```

        []{#resolve(com.facebook.buck.core.rules.BuildRuleResolver,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### resolve

            ``` methodSignature
            public T resolve​(BuildRuleResolver resolver,
                             TargetConfiguration targetConfiguration)
            ```

        []{#getParseTimeDeps(com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getParseTimeDeps

            ``` methodSignature
            public Iterable<BuildTarget> getParseTimeDeps​(TargetConfiguration targetConfiguration)
            ```

        []{#getToolType()}

        -   #### getToolType

            ``` methodSignature
            public ToolType getToolType()
            ```

            ::: block
            Return tool type of this provider instance
            :::

        []{#getUseUnixPathSeparator()}

        -   #### getUseUnixPathSeparator

            ``` methodSignature
            public boolean getUseUnixPathSeparator()
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

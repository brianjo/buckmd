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
-   [Package](package-summary.html)
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
[Package]{.packageLabelInType} [com.facebook.buck.features.python.toolchain.impl](package-summary.html)
:::

## Class LazyPythonPlatform {#class-lazypythonplatform .title title="Class LazyPythonPlatform"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.python.toolchain.impl.LazyPythonPlatform

::: description
-   

    All Implemented Interfaces:
    :   `FlavorConvertible`, `PythonPlatform`

    ------------------------------------------------------------------------

        public class LazyPythonPlatform
        extends Object
        implements PythonPlatform

    ::: block
    An implementation of
    [`PythonPlatform`](../PythonPlatform.html "interface in com.facebook.buck.features.python.toolchain")
    that lazily creates
    [`PythonEnvironment`](../PythonEnvironment.html "class in com.facebook.buck.features.python.toolchain")
    and cxx library.
    This should be used to avoid creating all registered Python
    platform.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                             Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `LazyPythonPlatform​(ToolchainProvider toolchainProvider,                   PythonBuckConfig pythonBuckConfig,                   ProcessExecutor processExecutor,                   TargetConfiguration targetConfiguration,                   Flavor flavor,                   String configSection)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                   Method                                 Description
          --------------------------------------------------- -------------------------------------- -------------
          `Optional<BuildTarget>`                             `getCxxLibrary()`                       
          `PythonEnvironment`                                 `getEnvironment()`                      
          `Flavor`                                            `getFlavor()`                           
          `com.google.common.collect.ImmutableList<String>`   `getInplaceBinaryInterpreterFlags()`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
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

        []{#<init>(com.facebook.buck.core.toolchain.ToolchainProvider,com.facebook.buck.features.python.PythonBuckConfig,com.facebook.buck.util.ProcessExecutor,com.facebook.buck.core.model.TargetConfiguration,com.facebook.buck.core.model.Flavor,java.lang.String)}

        -   #### LazyPythonPlatform

                public LazyPythonPlatform​(ToolchainProvider toolchainProvider,
                                          PythonBuckConfig pythonBuckConfig,
                                          ProcessExecutor processExecutor,
                                          TargetConfiguration targetConfiguration,
                                          Flavor flavor,
                                          String configSection)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getFlavor()}

        -   #### getFlavor

            ``` methodSignature
            public Flavor getFlavor()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFlavor` in interface `FlavorConvertible`

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFlavor` in interface `PythonPlatform`

            [Returns:]{.returnLabel}
            :   the
                [`Flavor`](../../../../core/model/Flavor.html "interface in com.facebook.buck.core.model")
                associated with this python platform.

        []{#getEnvironment()}

        -   #### getEnvironment

            ``` methodSignature
            public PythonEnvironment getEnvironment()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getEnvironment` in interface `PythonPlatform`

            [Returns:]{.returnLabel}
            :   the
                [`PythonEnvironment`](../PythonEnvironment.html "class in com.facebook.buck.features.python.toolchain")
                for this python platform.

        []{#getCxxLibrary()}

        -   #### getCxxLibrary

            ``` methodSignature
            public Optional<BuildTarget> getCxxLibrary()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCxxLibrary` in interface `PythonPlatform`

            [Returns:]{.returnLabel}
            :   the
                [`BuildTarget`](../../../../core/model/BuildTarget.html "class in com.facebook.buck.core.model")
                wrapping the C/C++ library used by C/C++ extensions.

        []{#getInplaceBinaryInterpreterFlags()}

        -   #### getInplaceBinaryInterpreterFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getInplaceBinaryInterpreterFlags()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getInplaceBinaryInterpreterFlags` in
                interface `PythonPlatform`

            [Returns:]{.returnLabel}
            :   flags that should be added to the hashbang of inplace
                python binaries
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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
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

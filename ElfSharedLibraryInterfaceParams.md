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

## Class ElfSharedLibraryInterfaceParams {#class-elfsharedlibraryinterfaceparams .title title="Class ElfSharedLibraryInterfaceParams"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.toolchain.ElfSharedLibraryInterfaceParams

::: description
-   

    All Implemented Interfaces:
    :   `SharedLibraryInterfaceParams`

    ------------------------------------------------------------------------

        public abstract class ElfSharedLibraryInterfaceParams
        extends Object
        implements SharedLibraryInterfaceParams
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.cxx.toolchain.SharedLibraryInterfaceParams}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.cxx.toolchain.[SharedLibraryInterfaceParams](SharedLibraryInterfaceParams.html "interface in com.facebook.buck.cxx.toolchain")

            `SharedLibraryInterfaceParams.Kind, SharedLibraryInterfaceParams.Type`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                           Description
          ------------------------------------- -------------
          `ElfSharedLibraryInterfaceParams()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                            Method                                                                                                                    Description
          ------------------------------------------------------------ ------------------------------------------------------------------------------------------------------------------------- -------------
          `SharedLibraryInterfaceParams.Kind`                          `getKind()`                                                                                                                
          `abstract com.google.common.collect.ImmutableList<String>`   `getLdflags()`                                                                                                             
          `abstract ToolProvider`                                      `getObjcopy()`                                                                                                             
          `Iterable<BuildTarget>`                                      `getParseTimeDeps​(TargetConfiguration targetConfiguration)`                                                                
          `abstract boolean`                                           `isRemoveUndefinedSymbols()`                                                                                               
          `static ElfSharedLibraryInterfaceParams`                     `of​(ToolProvider objcopy,   com.google.common.collect.ImmutableList<String> ldflags,   boolean removeUndefinedSymbols)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
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

        []{#<init>()}

        -   #### ElfSharedLibraryInterfaceParams

                public ElfSharedLibraryInterfaceParams()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#of(com.facebook.buck.core.toolchain.toolprovider.ToolProvider,com.google.common.collect.ImmutableList,boolean)}

        -   #### of

            ``` methodSignature
            public static ElfSharedLibraryInterfaceParams of​(ToolProvider objcopy,
                                                             com.google.common.collect.ImmutableList<String> ldflags,
                                                             boolean removeUndefinedSymbols)
            ```

        []{#getObjcopy()}

        -   #### getObjcopy

            ``` methodSignature
            public abstract ToolProvider getObjcopy()
            ```

        []{#getLdflags()}

        -   #### getLdflags

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<String> getLdflags()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLdflags` in interface `SharedLibraryInterfaceParams`

            [Returns:]{.returnLabel}
            :   additional flags to pass to the linker when linking
                interfaces.

        []{#isRemoveUndefinedSymbols()}

        -   #### isRemoveUndefinedSymbols

            ``` methodSignature
            public abstract boolean isRemoveUndefinedSymbols()
            ```

        []{#getParseTimeDeps(com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getParseTimeDeps

            ``` methodSignature
            public Iterable<BuildTarget> getParseTimeDeps​(TargetConfiguration targetConfiguration)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getParseTimeDeps` in
                interface `SharedLibraryInterfaceParams`

        []{#getKind()}

        -   #### getKind

            ``` methodSignature
            public SharedLibraryInterfaceParams.Kind getKind()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getKind` in interface `SharedLibraryInterfaceParams`
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

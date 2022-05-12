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

## Class MachoDylibStubParams {#class-machodylibstubparams .title title="Class MachoDylibStubParams"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.toolchain.MachoDylibStubParams

::: description
-   

    All Implemented Interfaces:
    :   `SharedLibraryInterfaceParams`

    ------------------------------------------------------------------------

        public abstract class MachoDylibStubParams
        extends Object
        implements SharedLibraryInterfaceParams

    ::: block
    Represents the params needed to create scrubbed dylib stubs.
    :::
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

          Constructor                Description
          -------------------------- -------------
          `MachoDylibStubParams()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                   Method                                                        Description
          --------------------------------------------------- ------------------------------------------------------------- -------------
          `SharedLibraryInterfaceParams.Kind`                 `getKind()`                                                    
          `com.google.common.collect.ImmutableList<String>`   `getLdflags()`                                                 
          `Iterable<BuildTarget>`                             `getParseTimeDeps​(TargetConfiguration targetConfiguration)`    
          `abstract Tool`                                     `getStrip()`                                                   
          `static MachoDylibStubParams`                       `of​(Tool strip)`                                               

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

        -   #### MachoDylibStubParams

                public MachoDylibStubParams()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#of(com.facebook.buck.core.toolchain.tool.Tool)}

        -   #### of

            ``` methodSignature
            public static MachoDylibStubParams of​(Tool strip)
            ```

        []{#getStrip()}

        -   #### getStrip

            ``` methodSignature
            public abstract Tool getStrip()
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

        []{#getLdflags()}

        -   #### getLdflags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getLdflags()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLdflags` in interface `SharedLibraryInterfaceParams`

            [Returns:]{.returnLabel}
            :   additional flags to pass to the linker when linking
                interfaces.
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

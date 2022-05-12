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
[Package]{.packageLabelInType} [com.facebook.buck.cxx.toolchain.linker.impl](package-summary.html)
:::

## Class DefaultLinkerProvider {#class-defaultlinkerprovider .title title="Class DefaultLinkerProvider"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.toolchain.linker.impl.DefaultLinkerProvider

::: description
-   

    All Implemented Interfaces:
    :   `LinkerProvider`

    ------------------------------------------------------------------------

        public class DefaultLinkerProvider
        extends Object
        implements LinkerProvider
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.cxx.toolchain.linker.LinkerProvider}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.cxx.toolchain.linker.[LinkerProvider](../LinkerProvider.html "interface in com.facebook.buck.cxx.toolchain.linker")

            `LinkerProvider.Type`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                  Description
          -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `DefaultLinkerProvider​(LinkerProvider.Type type,                      ToolProvider toolProvider,                      boolean cacheLinks)`                                                    
          `DefaultLinkerProvider​(LinkerProvider.Type type,                      ToolProvider toolProvider,                      boolean cacheLinks,                      boolean scrubConcurrently)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type         Method                                                                                  Description
          ------------------------- --------------------------------------------------------------------------------------- -------------
          `Iterable<BuildTarget>`   `getParseTimeDeps​(TargetConfiguration targetConfiguration)`                              
          `LinkerProvider.Type`     `getType()`                                                                              
          `Linker`                  `resolve​(BuildRuleResolver resolver,        TargetConfiguration targetConfiguration)`    

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

        []{#<init>(com.facebook.buck.cxx.toolchain.linker.LinkerProvider.Type,com.facebook.buck.core.toolchain.toolprovider.ToolProvider,boolean)}

        -   #### DefaultLinkerProvider

                public DefaultLinkerProvider​(LinkerProvider.Type type,
                                             ToolProvider toolProvider,
                                             boolean cacheLinks)

        []{#<init>(com.facebook.buck.cxx.toolchain.linker.LinkerProvider.Type,com.facebook.buck.core.toolchain.toolprovider.ToolProvider,boolean,boolean)}

        -   #### DefaultLinkerProvider

                public DefaultLinkerProvider​(LinkerProvider.Type type,
                                             ToolProvider toolProvider,
                                             boolean cacheLinks,
                                             boolean scrubConcurrently)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#resolve(com.facebook.buck.core.rules.BuildRuleResolver,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### resolve

            ``` methodSignature
            public Linker resolve​(BuildRuleResolver resolver,
                                  TargetConfiguration targetConfiguration)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `resolve` in interface `LinkerProvider`

        []{#getType()}

        -   #### getType

            ``` methodSignature
            public LinkerProvider.Type getType()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getType` in interface `LinkerProvider`

        []{#getParseTimeDeps(com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getParseTimeDeps

            ``` methodSignature
            public Iterable<BuildTarget> getParseTimeDeps​(TargetConfiguration targetConfiguration)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getParseTimeDeps` in interface `LinkerProvider`
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

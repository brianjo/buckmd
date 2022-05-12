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
[Package]{.packageLabelInType} [com.facebook.buck.core.starlark.rule.data](package-summary.html)
:::

## Class SkylarkDependency {#class-skylarkdependency .title title="Class SkylarkDependency"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.starlark.rule.data.SkylarkDependency

::: description
-   

    All Implemented Interfaces:
    :   `com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable`,
        `com.google.devtools.build.lib.skylarkinterface.SkylarkValue`,
        `com.google.devtools.build.lib.syntax.SkylarkIndexable`,
        `com.google.devtools.build.lib.syntax.SkylarkQueryable`

    ------------------------------------------------------------------------

        public class SkylarkDependency
        extends Object
        implements com.google.devtools.build.lib.skylarkinterface.SkylarkValue, com.google.devtools.build.lib.syntax.SkylarkIndexable

    ::: block
    Skylark object provided to users to get extra information about a
    dependency, including its original build target, its
    [`ProviderInfoCollection`](../../../rules/providers/collect/ProviderInfoCollection.html "interface in com.facebook.buck.core.rules.providers.collect"),
    and more in the future. `SkylarkIndexable` operations are proxied to
    the provided
    [`ProviderInfoCollection`](../../../rules/providers/collect/ProviderInfoCollection.html "interface in com.facebook.buck.core.rules.providers.collect")
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                      Description
          ------------------------------------------------------------------------------------------------ -------------
          `SkylarkDependency​(BuildTarget target,                  ProviderInfoCollection providerInfos)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                               Method                                                                                                                                                                       Description
          ----------------------------------------------- ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `boolean`                                       `containsKey​(Object key,            com.google.devtools.build.lib.events.Location loc,            com.google.devtools.build.lib.skylarkinterface.StarlarkContext context)`    
          `Object`                                        `getIndex​(Object key,         com.google.devtools.build.lib.events.Location loc,         com.google.devtools.build.lib.skylarkinterface.StarlarkContext context)`             
          `ProviderInfoCollection`                        `getProviderInfos()`                                                                                                                                                          
          `com.google.devtools.build.lib.cmdline.Label`   `label()`                                                                                                                                                                     
          `void`                                          `repr​(com.google.devtools.build.lib.skylarkinterface.SkylarkPrinter printer)`                                                                                                 

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable}

            ### Methods inherited from interface com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable

            `debugPrint, str`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.google.devtools.build.lib.syntax.SkylarkQueryable}

            ### Methods inherited from interface com.google.devtools.build.lib.syntax.SkylarkQueryable

            `containsKey`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.google.devtools.build.lib.skylarkinterface.SkylarkValue}

            ### Methods inherited from interface com.google.devtools.build.lib.skylarkinterface.SkylarkValue

            `isHashable, isImmutable`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.providers.collect.ProviderInfoCollection)}

        -   #### SkylarkDependency

                public SkylarkDependency​(BuildTarget target,
                                         ProviderInfoCollection providerInfos)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#label()}

        -   #### label

            ``` methodSignature
            public com.google.devtools.build.lib.cmdline.Label label()
            ```

        []{#getProviderInfos()}

        -   #### getProviderInfos

            ``` methodSignature
            public ProviderInfoCollection getProviderInfos()
            ```

        []{#repr(com.google.devtools.build.lib.skylarkinterface.SkylarkPrinter)}

        -   #### repr

            ``` methodSignature
            public void repr​(com.google.devtools.build.lib.skylarkinterface.SkylarkPrinter printer)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `repr` in
                interface `com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable`

        []{#getIndex(java.lang.Object,com.google.devtools.build.lib.events.Location,com.google.devtools.build.lib.skylarkinterface.StarlarkContext)}

        -   #### getIndex

            ``` methodSignature
            public Object getIndex​(Object key,
                                   com.google.devtools.build.lib.events.Location loc,
                                   com.google.devtools.build.lib.skylarkinterface.StarlarkContext context)
                            throws com.google.devtools.build.lib.syntax.EvalException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getIndex` in
                interface `com.google.devtools.build.lib.syntax.SkylarkIndexable`

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`

        []{#containsKey(java.lang.Object,com.google.devtools.build.lib.events.Location,com.google.devtools.build.lib.skylarkinterface.StarlarkContext)}

        -   #### containsKey

            ``` methodSignature
            public boolean containsKey​(Object key,
                                       com.google.devtools.build.lib.events.Location loc,
                                       com.google.devtools.build.lib.skylarkinterface.StarlarkContext context)
                                throws com.google.devtools.build.lib.syntax.EvalException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `containsKey` in
                interface `com.google.devtools.build.lib.syntax.SkylarkQueryable`

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`
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

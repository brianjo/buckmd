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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.android](package-summary.html)
:::

## Class IdentityResourcesProvider {#class-identityresourcesprovider .title title="Class IdentityResourcesProvider"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.IdentityResourcesProvider

::: description
-   

    All Implemented Interfaces:
    :   `FilteredResourcesProvider`

    ------------------------------------------------------------------------

        public class IdentityResourcesProvider
        extends Object
        implements FilteredResourcesProvider
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                       Description
          ------------------------------------------------------------------------------------------------- -------------
          `IdentityResourcesProvider​(com.google.common.collect.ImmutableList<SourcePath> resDirectories)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                       Method                       Description
          ------------------------------------------------------- ---------------------------- -------------
          `Optional<SourcePath>`                                  `getOverrideSymbolsPath()`    
          `com.google.common.collect.ImmutableList<SourcePath>`   `getResDirectories()`         
          `Optional<BuildRule>`                                   `getResourceFilterRule()`     
          `com.google.common.collect.ImmutableList<Path>`         `getStringFiles()`            
          `boolean`                                               `hasResources()`              

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
        -   []{#methods.inherited.from.class.com.facebook.buck.android.FilteredResourcesProvider}

            ### Methods inherited from interface com.facebook.buck.android.[FilteredResourcesProvider](FilteredResourcesProvider.html "interface in com.facebook.buck.android")

            `getRelativeResDirectories`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.google.common.collect.ImmutableList)}

        -   #### IdentityResourcesProvider

                public IdentityResourcesProvider​(com.google.common.collect.ImmutableList<SourcePath> resDirectories)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getResDirectories()}

        -   #### getResDirectories

            ``` methodSignature
            public com.google.common.collect.ImmutableList<SourcePath> getResDirectories()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getResDirectories` in
                interface `FilteredResourcesProvider`

            [Returns:]{.returnLabel}
            :   The set of res/ directories that should be used to
                calculate the final R.java file.

        []{#getStringFiles()}

        -   #### getStringFiles

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Path> getStringFiles()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getStringFiles` in
                interface `FilteredResourcesProvider`

            [Returns:]{.returnLabel}
            :   The list of `strings.xml` files excluding whitelisted
                strings. Empty unless
                `ResourceCompressionMode.isStoreStringsAsAssets` is
                true.

        []{#getResourceFilterRule()}

        -   #### getResourceFilterRule

            ``` methodSignature
            public Optional<BuildRule> getResourceFilterRule()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getResourceFilterRule` in
                interface `FilteredResourcesProvider`

        []{#getOverrideSymbolsPath()}

        -   #### getOverrideSymbolsPath

            ``` methodSignature
            public Optional<SourcePath> getOverrideSymbolsPath()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getOverrideSymbolsPath` in
                interface `FilteredResourcesProvider`

        []{#hasResources()}

        -   #### hasResources

            ``` methodSignature
            public boolean hasResources()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `hasResources` in interface `FilteredResourcesProvider`
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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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

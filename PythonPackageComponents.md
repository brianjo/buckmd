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
[Package]{.packageLabelInType} [com.facebook.buck.features.python](package-summary.html)
:::

## Class PythonPackageComponents {#class-pythonpackagecomponents .title title="Class PythonPackageComponents"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.python.PythonPackageComponents

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`

    ------------------------------------------------------------------------

        public abstract class PythonPackageComponents
        extends Object
        implements AddsToRuleKey

    ::: block
    All per-rule components that contribute to a Python binary.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `PythonPacka          | ::: block             |
        |                       | geComponents.Builder` | A helper class to     |
        |                       |                       | construct a           |
        |                       |                       | Py                    |
        |                       |                       | thonPackageComponents |
        |                       |                       | instance which throws |
        |                       |                       | human readable error  |
        |                       |                       | messages on           |
        |                       |                       | duplicates.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                   Description
          ----------------------------- -------------
          `PythonPackageComponents()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                                          Method                                                             Description
          ------------------------------------------------------------------------------------------ ------------------------------------------------------------------ -------------
          `Symlinks`                                                                                 `asSymlinks()`                                                      
          `void`                                                                                     `forEachInput​(java.util.function.Consumer<SourcePath> consumer)`    
          `abstract Optional<SourcePath>`                                                            `getDefaultInitPy()`                                                
          `com.google.common.collect.ImmutableCollection<BuildRule>`                                 `getDeps​(SourcePathRuleFinder ruleFinder)`                          
          `abstract com.google.common.collect.ImmutableListMultimap<BuildTarget,​PythonComponents>`   `getModules()`                                                      
          `abstract com.google.common.collect.ImmutableListMultimap<BuildTarget,​PythonComponents>`   `getNativeLibraries()`                                              
          `abstract com.google.common.collect.ImmutableListMultimap<BuildTarget,​PythonComponents>`   `getResources()`                                                    
          `abstract Optional<Boolean>`                                                               `isZipSafe()`                                                       
          `com.facebook.buck.features.python.PythonResolvedPackageComponents`                        `resolve​(SourcePathResolverAdapter resolver)`                       
          `PythonPackageComponents`                                                                  `withDefaultInitPy​(SourcePath emptyInit)`                           

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

        []{#<init>()}

        -   #### PythonPackageComponents

                public PythonPackageComponents()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getModules()}

        -   #### getModules

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableListMultimap<BuildTarget,​PythonComponents> getModules()
            ```

        []{#getResources()}

        -   #### getResources

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableListMultimap<BuildTarget,​PythonComponents> getResources()
            ```

        []{#getNativeLibraries()}

        -   #### getNativeLibraries

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableListMultimap<BuildTarget,​PythonComponents> getNativeLibraries()
            ```

        []{#getDefaultInitPy()}

        -   #### getDefaultInitPy

            ``` methodSignature
            public abstract Optional<SourcePath> getDefaultInitPy()
            ```

        []{#isZipSafe()}

        -   #### isZipSafe

            ``` methodSignature
            public abstract Optional<Boolean> isZipSafe()
            ```

        []{#forEachInput(java.util.function.Consumer)}

        -   #### forEachInput

            ``` methodSignature
            public void forEachInput​(java.util.function.Consumer<SourcePath> consumer)
            ```

        []{#getDeps(com.facebook.buck.core.rules.SourcePathRuleFinder)}

        -   #### getDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableCollection<BuildRule> getDeps​(SourcePathRuleFinder ruleFinder)
            ```

        []{#resolve(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### resolve

            ``` methodSignature
            public com.facebook.buck.features.python.PythonResolvedPackageComponents resolve​(SourcePathResolverAdapter resolver)
            ```

        []{#asSymlinks()}

        -   #### asSymlinks

            ``` methodSignature
            public Symlinks asSymlinks()
            ```

        []{#withDefaultInitPy(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### withDefaultInitPy

            ``` methodSignature
            public PythonPackageComponents withDefaultInitPy​(@Nullable
                                                             SourcePath emptyInit)
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

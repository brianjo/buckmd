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
[Package]{.packageLabelInType} [com.facebook.buck.features.python](package-summary.html)
:::

## Class PythonPackageComponents.Builder {#class-pythonpackagecomponents.builder .title title="Class PythonPackageComponents.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.python.PythonPackageComponents.Builder

::: description
-   

    Enclosing class:
    :   [PythonPackageComponents](PythonPackageComponents.html "class in com.facebook.buck.features.python")

    ------------------------------------------------------------------------

        public static class PythonPackageComponents.Builder
        extends Object

    ::: block
    A helper class to construct a PythonPackageComponents instance which
    throws human readable error messages on duplicates.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor   Description
          ------------- -------------
          `Builder()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                   Method                                                                                   Description
          ----------------------------------- ---------------------------------------------------------------------------------------- -------------
          `PythonPackageComponents.Builder`   `addZipSafe​(Optional<Boolean> zipSafe)`                                                   
          `PythonPackageComponents`           `build()`                                                                                 
          `PythonPackageComponents.Builder`   `putModules​(BuildTarget owner,           PythonComponents components)`                    
          `PythonPackageComponents.Builder`   `putNativeLibraries​(BuildTarget owner,                   PythonComponents components)`    
          `PythonPackageComponents.Builder`   `putResources​(BuildTarget owner,             PythonComponents components)`                

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

        []{#<init>()}

        -   #### Builder

                public Builder()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#putModules(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.features.python.PythonComponents)}

        -   #### putModules

            ``` methodSignature
            public PythonPackageComponents.Builder putModules​(BuildTarget owner,
                                                              PythonComponents components)
            ```

        []{#putResources(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.features.python.PythonComponents)}

        -   #### putResources

            ``` methodSignature
            public PythonPackageComponents.Builder putResources​(BuildTarget owner,
                                                                PythonComponents components)
            ```

        []{#putNativeLibraries(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.features.python.PythonComponents)}

        -   #### putNativeLibraries

            ``` methodSignature
            public PythonPackageComponents.Builder putNativeLibraries​(BuildTarget owner,
                                                                      PythonComponents components)
            ```

        []{#addZipSafe(java.util.Optional)}

        -   #### addZipSafe

            ``` methodSignature
            public PythonPackageComponents.Builder addZipSafe​(Optional<Boolean> zipSafe)
            ```

        []{#build()}

        -   #### build

            ``` methodSignature
            public PythonPackageComponents build()
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

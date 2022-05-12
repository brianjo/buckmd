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
[Package]{.packageLabelInType} [com.facebook.buck.core.toolchain](package-summary.html)
:::

## Class BaseToolchainProvider {#class-basetoolchainprovider .title title="Class BaseToolchainProvider"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.toolchain.BaseToolchainProvider

::: description
-   

    All Implemented Interfaces:
    :   `ToolchainProvider`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `DefaultToolchainProvider`

    ------------------------------------------------------------------------

        public abstract class BaseToolchainProvider
        extends Object
        implements ToolchainProvider
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                 Description
          --------------------------- -------------
          `BaseToolchainProvider()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                    Method                                                                                                                                                      Description
          ------------------------------------ ----------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `<T extends Toolchain>T`             `getByName​(String toolchainName,          TargetConfiguration toolchainTargetConfiguration,          Class<T> toolchainClass)`                               
          `<T extends Toolchain>Optional<T>`   `getByNameIfPresent​(String toolchainName,                   TargetConfiguration toolchainTargetConfiguration,                   Class<T> toolchainClass)`    

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
        -   []{#methods.inherited.from.class.com.facebook.buck.core.toolchain.ToolchainProvider}

            ### Methods inherited from interface com.facebook.buck.core.toolchain.[ToolchainProvider](ToolchainProvider.html "interface in com.facebook.buck.core.toolchain")

            `getByName, getToolchainInstantiationException, getToolchainsWithCapability, isToolchainCreated, isToolchainFailed, isToolchainPresent`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### BaseToolchainProvider

                public BaseToolchainProvider()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getByName(java.lang.String,com.facebook.buck.core.model.TargetConfiguration,java.lang.Class)}

        -   #### getByName

            ``` methodSignature
            public <T extends Toolchain> T getByName​(String toolchainName,
                                                     TargetConfiguration toolchainTargetConfiguration,
                                                     Class<T> toolchainClass)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getByName` in interface `ToolchainProvider`

        []{#getByNameIfPresent(java.lang.String,com.facebook.buck.core.model.TargetConfiguration,java.lang.Class)}

        -   #### getByNameIfPresent

            ``` methodSignature
            public <T extends Toolchain> Optional<T> getByNameIfPresent​(String toolchainName,
                                                                        TargetConfiguration toolchainTargetConfiguration,
                                                                        Class<T> toolchainClass)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getByNameIfPresent` in interface `ToolchainProvider`
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

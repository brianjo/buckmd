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
[Package]{.packageLabelInType} [com.facebook.buck.apple.clang](package-summary.html)
:::

## Class ModuleMapFactory {#class-modulemapfactory .title title="Class ModuleMapFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.clang.ModuleMapFactory

::: description
-   

    ------------------------------------------------------------------------

        public class ModuleMapFactory
        extends Object

    ::: block
    Creates module map instances.
    Use this instead of directly creating a module map instance
    directory.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor            Description
          ---------------------- -------------
          `ModuleMapFactory()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static ModuleMap`    | `createMod            | ::: block             |
        |                       | uleMap​(String moduleN | Creates a module map. |
        |                       | ame,                M | :::                   |
        |                       | oduleMapMode moduleMa |                       |
        |                       | pMode,                |                       |
        |                       |  UmbrellaHeaderModule |                       |
        |                       | Map.SwiftMode swiftMo |                       |
        |                       | de,                Se |                       |
        |                       | t<Path> headerPaths)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
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

        -   #### ModuleMapFactory

                public ModuleMapFactory()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#createModuleMap(java.lang.String,com.facebook.buck.apple.clang.ModuleMapMode,com.facebook.buck.apple.clang.UmbrellaHeaderModuleMap.SwiftMode,java.util.Set)}

        -   #### createModuleMap

            ``` methodSignature
            public static ModuleMap createModuleMap​(String moduleName,
                                                    ModuleMapMode moduleMapMode,
                                                    UmbrellaHeaderModuleMap.SwiftMode swiftMode,
                                                    Set<Path> headerPaths)
            ```

            ::: block
            Creates a module map.
            :::

            [Parameters:]{.paramLabel}
            :   `moduleName` - The name of the module.
            :   `moduleMapMode` - The module map mode to use.
            :   `swiftMode` - The Swift mode to use for umbrella header
                module maps. This parameter is unused with umbrella
                directory module maps.
            :   `headerPaths` - The exported headers of the module. This
                parameter is only used with headers module maps.

            [Returns:]{.returnLabel}
            :   A module map instance.
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

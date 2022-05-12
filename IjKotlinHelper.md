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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.features.project.intellij](package-summary.html)
:::

## Class IjKotlinHelper {#class-ijkotlinhelper .title title="Class IjKotlinHelper"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.project.intellij.IjKotlinHelper

::: description
-   

    ------------------------------------------------------------------------

        public final class IjKotlinHelper
        extends Object

    ::: block
    Helper class related to Kotlin
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static void`         | `a                    | ::: block             |
        |                       | ddKotlinJavaRuntimeLi | Add KotlinJavaRuntime |
        |                       | braryDependencyIfNece | library dependency to |
        |                       | ssary​(TargetNode<? ex | a module if necessary |
        |                       | tends JvmLibraryArg>  | :::                   |
        |                       | target,               |                       |
        |                       |                       |                       |
        |                       |               ModuleB |                       |
        |                       | uildContext context)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `isK                  | ::: block             |
        |                       | otlinModule​(JvmLibrar | Whether the target    |
        |                       | yArg constructorArg)` | node associated with  |
        |                       |                       | the constructorArg    |
        |                       |                       | will produce a Kotlin |
        |                       |                       | module                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `r                    | ::: block             |
        |                       | equiresKapt​(JvmLibrar | Whether the target    |
        |                       | yArg constructorArg)` | node associated with  |
        |                       |                       | the constructorArg    |
        |                       |                       | requires kapt         |
        |                       |                       | :::                   |
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
    -   []{#method.detail}

        ### Method Detail

        []{#isKotlinModule(com.facebook.buck.jvm.java.JvmLibraryArg)}

        -   #### isKotlinModule

            ``` methodSignature
            public static boolean isKotlinModule​(JvmLibraryArg constructorArg)
            ```

            ::: block
            Whether the target node associated with the constructorArg
            will produce a Kotlin module
            :::

        []{#requiresKapt(com.facebook.buck.jvm.java.JvmLibraryArg)}

        -   #### requiresKapt

            ``` methodSignature
            public static boolean requiresKapt​(JvmLibraryArg constructorArg)
            ```

            ::: block
            Whether the target node associated with the constructorArg
            requires kapt
            :::

        []{#addKotlinJavaRuntimeLibraryDependencyIfNecessary(com.facebook.buck.core.model.targetgraph.TargetNode,com.facebook.buck.features.project.intellij.ModuleBuildContext)}

        -   #### addKotlinJavaRuntimeLibraryDependencyIfNecessary

            ``` methodSignature
            public static void addKotlinJavaRuntimeLibraryDependencyIfNecessary​(TargetNode<? extends JvmLibraryArg> target,
                                                                                ModuleBuildContext context)
            ```

            ::: block
            Add KotlinJavaRuntime library dependency to a module if
            necessary
            :::
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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

<div>

-   Summary: 
-   Nested \| 
-   Field \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

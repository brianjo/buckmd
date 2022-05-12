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

## Class JavaLanguageLevelHelper {#class-javalanguagelevelhelper .title title="Class JavaLanguageLevelHelper"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.project.intellij.JavaLanguageLevelHelper

::: description
-   

    ------------------------------------------------------------------------

        public final class JavaLanguageLevelHelper
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static String`       | `convertLang          |                       |
        |                       | uageLevelToIjFormat​(S |                       |
        |                       | tring languageLevel)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `getLan               | ::: block             |
        | <T extends JvmLibrary | guageLevel​(IjProjectC | Get Java language     |
        | Arg>Optional<String>` | onfig projectConfig,  | level for a JVM       |
        |                       |                 Targe | library target        |
        |                       | tNode<T> targetNode)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `normalizeSourceLeve  | ::: block             |
        |                       | l​(String jdkVersion)` | Ensures that source   |
        |                       |                       | level has format      |
        |                       |                       | \"majorVe             |
        |                       |                       | rsion.minorVersion\". |
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

        []{#getLanguageLevel(com.facebook.buck.features.project.intellij.model.IjProjectConfig,com.facebook.buck.core.model.targetgraph.TargetNode)}

        -   #### getLanguageLevel

            ``` methodSignature
            public static <T extends JvmLibraryArg> Optional<String> getLanguageLevel​(IjProjectConfig projectConfig,
                                                                                      TargetNode<T> targetNode)
            ```

            ::: block
            Get Java language level for a JVM library target
            :::

        []{#normalizeSourceLevel(java.lang.String)}

        -   #### normalizeSourceLevel

            ``` methodSignature
            public static String normalizeSourceLevel​(String jdkVersion)
            ```

            ::: block
            Ensures that source level has format
            \"majorVersion.minorVersion\".
            :::

        []{#convertLanguageLevelToIjFormat(java.lang.String)}

        -   #### convertLanguageLevelToIjFormat

            ``` methodSignature
            public static String convertLanguageLevelToIjFormat​(String languageLevel)
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

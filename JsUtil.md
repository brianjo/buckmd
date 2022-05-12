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
[Package]{.packageLabelInType} [com.facebook.buck.features.js](package-summary.html)
:::

## Class JsUtil {#class-jsutil .title title="Class JsUtil"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.js.JsUtil

::: description
-   

    ------------------------------------------------------------------------

        public class JsUtil
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static String`       | `e                    |                       |
        |                       | scapeJsonForStringEmb |                       |
        |                       | edding​(String input)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `ge                   | ::: block             |
        | static Optional<Arg>` | tExtraJson​(HasExtraJs | Wraps the             |
        |                       | on args,              | [`StringWithMacros`]  |
        |                       | BuildTarget target,   | (../../rules/macros/S |
        |                       |            ActionGrap | tringWithMacros.html  |
        |                       | hBuilder graphBuilder | "class in com.faceboo |
        |                       | ,             CellPat | k.buck.rules.macros") |
        |                       | hResolver cellRoots)` | coming from           |
        |                       |                       | [`HasExtraJson`](     |
        |                       |                       | HasExtraJson.html "in |
        |                       |                       | terface in com.facebo |
        |                       |                       | ok.buck.features.js") |
        |                       |                       | so that it can be     |
        |                       |                       | added to rule keys    |
        |                       |                       | and expanded easily.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `getSourc             |                       |
        |                       | emapPath​(JsBundleOutp |                       |
        |                       | uts jsBundleOutputs)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `getSourcemapPat      |                       |
        |                       | h​(String bundleName)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `getValue             |                       |
        |                       | ForFlavor​(com.google. |                       |
        |                       | common.collect.Immuta |                       |
        |                       | bleMap<UserFlavor,​Str |                       |
        |                       | ing> map,             |                       |
        |                       |       Flavor flavor)` |                       |
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

        []{#getValueForFlavor(com.google.common.collect.ImmutableMap,com.facebook.buck.core.model.Flavor)}

        -   #### getValueForFlavor

            ``` methodSignature
            public static String getValueForFlavor​(com.google.common.collect.ImmutableMap<UserFlavor,​String> map,
                                                   Flavor flavor)
            ```

        []{#getSourcemapPath(com.facebook.buck.features.js.JsBundleOutputs)}

        -   #### getSourcemapPath

            ``` methodSignature
            public static String getSourcemapPath​(JsBundleOutputs jsBundleOutputs)
            ```

        []{#getSourcemapPath(java.lang.String)}

        -   #### getSourcemapPath

            ``` methodSignature
            public static String getSourcemapPath​(String bundleName)
            ```

        []{#getExtraJson(com.facebook.buck.features.js.HasExtraJson,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.cell.CellPathResolver)}

        -   #### getExtraJson

            ``` methodSignature
            public static Optional<Arg> getExtraJson​(HasExtraJson args,
                                                     BuildTarget target,
                                                     ActionGraphBuilder graphBuilder,
                                                     CellPathResolver cellRoots)
            ```

            ::: block
            Wraps the
            [`StringWithMacros`](../../rules/macros/StringWithMacros.html "class in com.facebook.buck.rules.macros")
            coming from
            [`HasExtraJson`](HasExtraJson.html "interface in com.facebook.buck.features.js")
            so that it can be added to rule keys and expanded easily.
            :::

        []{#escapeJsonForStringEmbedding(java.lang.String)}

        -   #### escapeJsonForStringEmbedding

            ``` methodSignature
            public static String escapeJsonForStringEmbedding​(String input)
            ```

            [Returns:]{.returnLabel}
            :   The input with all special JSON characters escaped, but
                not wrapped in quotes.
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

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
[Package]{.packageLabelInType} [com.facebook.buck.parser](package-summary.html)
:::

## Class UnflavoredBuildTargetFactory {#class-unflavoredbuildtargetfactory .title title="Class UnflavoredBuildTargetFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.parser.UnflavoredBuildTargetFactory

::: description
-   

    ------------------------------------------------------------------------

        public class UnflavoredBuildTargetFactory
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                Method                                                                                                                                                          Description
          -------------------------------- --------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `static UnflavoredBuildTarget`   `createFromRawNode​(Path cellRoot,                  CanonicalCellName cellName,                  Map<String,​Object> map,                  Path buildFilePath)`    

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

        []{#createFromRawNode(java.nio.file.Path,com.facebook.buck.core.cell.name.CanonicalCellName,java.util.Map,java.nio.file.Path)}

        -   #### createFromRawNode

            ``` methodSignature
            public static UnflavoredBuildTarget createFromRawNode​(Path cellRoot,
                                                                  CanonicalCellName cellName,
                                                                  Map<String,​Object> map,
                                                                  Path buildFilePath)
            ```

            [Parameters:]{.paramLabel}
            :   `cellRoot` - Absolute path to the root of the cell the
                rule is defined in.
            :   `map` - the map of values that define the rule.
            :   `buildFilePath` - Absolute path to the build file the
                rule is defined in

            [Returns:]{.returnLabel}
            :   the build target defined by the rule.
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
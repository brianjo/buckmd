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
[Package]{.packageLabelInType} [com.facebook.buck.cxx](package-summary.html)
:::

## Class OmnibusRoots {#class-omnibusroots .title title="Class OmnibusRoots"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.OmnibusRoots

::: description
-   

    ------------------------------------------------------------------------

        public abstract class OmnibusRoots
        extends Object

    ::: block
    A helper class for building the included and excluded omnibus roots
    to pass to the omnibus builder.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                    Description
          ------------------- ------------------------ -------------
          `static class `     `OmnibusRoots.Builder`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor        Description
          ------------------ -------------
          `OmnibusRoots()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                                 Method                                                                                                            Description
          --------------------------------------------------------------------------------- ----------------------------------------------------------------------------------------------------------------- -------------
          `static OmnibusRoots.Builder`                                                     `builder​(com.google.common.collect.ImmutableSet<BuildTarget> excludes,        ActionGraphBuilder graphBuilder)`    
          `abstract com.google.common.collect.ImmutableMap<BuildTarget,​NativeLinkable>`     `getExcludedRoots()`                                                                                               
          `abstract com.google.common.collect.ImmutableMap<BuildTarget,​NativeLinkTarget>`   `getIncludedRoots()`                                                                                               

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
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

        -   #### OmnibusRoots

                public OmnibusRoots()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getIncludedRoots()}

        -   #### getIncludedRoots

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableMap<BuildTarget,​NativeLinkTarget> getIncludedRoots()
            ```

            [Returns:]{.returnLabel}
            :   the
                [`NativeLinkTarget`](toolchain/nativelink/NativeLinkTarget.html "interface in com.facebook.buck.cxx.toolchain.nativelink")
                roots that are included in omnibus linking.

        []{#getExcludedRoots()}

        -   #### getExcludedRoots

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableMap<BuildTarget,​NativeLinkable> getExcludedRoots()
            ```

            [Returns:]{.returnLabel}
            :   the
                [`NativeLinkable`](toolchain/nativelink/NativeLinkable.html "interface in com.facebook.buck.cxx.toolchain.nativelink")
                roots that are excluded from omnibus linking.

        []{#builder(com.google.common.collect.ImmutableSet,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### builder

            ``` methodSignature
            public static OmnibusRoots.Builder builder​(com.google.common.collect.ImmutableSet<BuildTarget> excludes,
                                                       ActionGraphBuilder graphBuilder)
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

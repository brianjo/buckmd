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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.scala](package-summary.html)
:::

## Class ScalaBuckConfig {#class-scalabuckconfig .title title="Class ScalaBuckConfig"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.scala.ScalaBuckConfig

::: description
-   

    ------------------------------------------------------------------------

        public class ScalaBuckConfig
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                              Description
          ---------------------------------------- -------------
          `ScalaBuckConfig​(BuckConfig delegate)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                   Method                                                                                      Description
          --------------------------------------------------- ------------------------------------------------------------------------------------------- -------------
          `com.google.common.collect.ImmutableList<String>`   `getCompilerFlags()`                                                                         
          `Iterable<BuildTarget>`                             `getCompilerPlugins​(TargetConfiguration targetConfiguration)`                                
          `Tool`                                              `getScalac​(BuildRuleResolver resolver,          TargetConfiguration targetConfiguration)`    
          `Optional<BuildTarget>`                             `getScalacTarget​(TargetConfiguration targetConfiguration)`                                   
          `BuildTarget`                                       `getScalaLibraryTarget​(TargetConfiguration targetConfiguration)`                             

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

        []{#<init>(com.facebook.buck.core.config.BuckConfig)}

        -   #### ScalaBuckConfig

                public ScalaBuckConfig​(BuckConfig delegate)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getScalac(com.facebook.buck.core.rules.BuildRuleResolver,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getScalac

            ``` methodSignature
            public Tool getScalac​(BuildRuleResolver resolver,
                                  TargetConfiguration targetConfiguration)
            ```

        []{#getScalaLibraryTarget(com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getScalaLibraryTarget

            ``` methodSignature
            public BuildTarget getScalaLibraryTarget​(TargetConfiguration targetConfiguration)
            ```

        []{#getCompilerPlugins(com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getCompilerPlugins

            ``` methodSignature
            public Iterable<BuildTarget> getCompilerPlugins​(TargetConfiguration targetConfiguration)
            ```

        []{#getScalacTarget(com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getScalacTarget

            ``` methodSignature
            public Optional<BuildTarget> getScalacTarget​(TargetConfiguration targetConfiguration)
            ```

        []{#getCompilerFlags()}

        -   #### getCompilerFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getCompilerFlags()
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

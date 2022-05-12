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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java](package-summary.html)
:::

## Class JavaOptions {#class-javaoptions .title title="Class JavaOptions"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.JavaOptions

::: description
-   

    ------------------------------------------------------------------------

        public abstract class JavaOptions
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor       Description
          ----------------- -------------
          `JavaOptions()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type         Method                                                                                                                                                        Description
          ------------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `void`                    `addParseTimeDeps​(com.google.common.collect.ImmutableCollection.Builder<BuildTarget> depsBuilder,                 TargetConfiguration targetConfiguration)`    
          `Tool`                    `getJavaRuntimeLauncher​(BuildRuleResolver ruleResolver,                       TargetConfiguration targetConfiguration)`                                        
          `abstract ToolProvider`   `getJavaRuntimeProvider()`                                                                                                                                     
          `static JavaOptions`      `of​(ToolProvider javaRuntimeProvider)`                                                                                                                         

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

        -   #### JavaOptions

                public JavaOptions()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getJavaRuntimeProvider()}

        -   #### getJavaRuntimeProvider

            ``` methodSignature
            public abstract ToolProvider getJavaRuntimeProvider()
            ```

        []{#getJavaRuntimeLauncher(com.facebook.buck.core.rules.BuildRuleResolver,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getJavaRuntimeLauncher

            ``` methodSignature
            public Tool getJavaRuntimeLauncher​(BuildRuleResolver ruleResolver,
                                               TargetConfiguration targetConfiguration)
            ```

        []{#addParseTimeDeps(com.google.common.collect.ImmutableCollection.Builder,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### addParseTimeDeps

            ``` methodSignature
            public void addParseTimeDeps​(com.google.common.collect.ImmutableCollection.Builder<BuildTarget> depsBuilder,
                                         TargetConfiguration targetConfiguration)
            ```

        []{#of(com.facebook.buck.core.toolchain.toolprovider.ToolProvider)}

        -   #### of

            ``` methodSignature
            public static JavaOptions of​(ToolProvider javaRuntimeProvider)
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

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

## Class JarBackedJavacProvider {#class-jarbackedjavacprovider .title title="Class JarBackedJavacProvider"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.JarBackedJavacProvider

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`, `JavacProvider`

    ------------------------------------------------------------------------

        public class JarBackedJavacProvider
        extends Object
        implements JavacProvider, AddsToRuleKey
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                         Description
          --------------------------------------------------------------------------------------------------- -------------
          `JarBackedJavacProvider​(SourcePath javacJarPath,                       String compilerClassName)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                     Method                                                                                                Description
          ----------------------------------------------------- ----------------------------------------------------------------------------------------------------- -------------
          `void`                                                `addParseTimeDeps​(com.google.common.collect.ImmutableCollection.Builder<BuildTarget> depsConsumer)`    
          `com.google.common.collect.ImmutableSet<BuildRule>`   `getBuildDeps​(SourcePathRuleFinder ruleFinder)`                                                        
          `Javac`                                               `resolve​(SourcePathRuleFinder ruleFinder)`                                                             

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

        []{#<init>(com.facebook.buck.core.sourcepath.SourcePath,java.lang.String)}

        -   #### JarBackedJavacProvider

                public JarBackedJavacProvider​(SourcePath javacJarPath,
                                              String compilerClassName)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#resolve(com.facebook.buck.core.rules.SourcePathRuleFinder)}

        -   #### resolve

            ``` methodSignature
            public Javac resolve​(SourcePathRuleFinder ruleFinder)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `resolve` in interface `JavacProvider`

        []{#addParseTimeDeps(com.google.common.collect.ImmutableCollection.Builder)}

        -   #### addParseTimeDeps

            ``` methodSignature
            public void addParseTimeDeps​(com.google.common.collect.ImmutableCollection.Builder<BuildTarget> depsConsumer)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `addParseTimeDeps` in interface `JavacProvider`

        []{#getBuildDeps(com.facebook.buck.core.rules.SourcePathRuleFinder)}

        -   #### getBuildDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<BuildRule> getBuildDeps​(SourcePathRuleFinder ruleFinder)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildDeps` in interface `JavacProvider`
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

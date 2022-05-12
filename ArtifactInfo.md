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
[Package]{.packageLabelInType} [com.facebook.buck.artifact_cache](package-summary.html)
:::

## Class ArtifactInfo {#class-artifactinfo .title title="Class ArtifactInfo"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.artifact_cache.ArtifactInfo

::: description
-   

    ------------------------------------------------------------------------

        public abstract class ArtifactInfo
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                    Description
          ------------------- ------------------------ -------------
          `static class `     `ArtifactInfo.Builder`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor        Description
          ------------------ -------------
          `ArtifactInfo()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                  Method               Description
          ------------------------------------------------------------------ -------------------- -------------
          `static ArtifactInfo.Builder`                                      `builder()`           
          `abstract Optional<BuildTarget>`                                   `getBuildTarget()`    
          `long`                                                             `getBuildTimeMs()`    
          `abstract com.google.common.collect.ImmutableMap<String,​String>`   `getMetadata()`       
          `abstract Optional<String>`                                        `getRepository()`     
          `abstract com.google.common.collect.ImmutableSet<RuleKey>`         `getRuleKeys()`       
          `boolean`                                                          `isManifest()`        

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

        -   #### ArtifactInfo

                public ArtifactInfo()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getRuleKeys()}

        -   #### getRuleKeys

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSet<RuleKey> getRuleKeys()
            ```

        []{#getMetadata()}

        -   #### getMetadata

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableMap<String,​String> getMetadata()
            ```

        []{#getBuildTarget()}

        -   #### getBuildTarget

            ``` methodSignature
            public abstract Optional<BuildTarget> getBuildTarget()
            ```

        []{#getRepository()}

        -   #### getRepository

            ``` methodSignature
            public abstract Optional<String> getRepository()
            ```

        []{#getBuildTimeMs()}

        -   #### getBuildTimeMs

            ``` methodSignature
            @Default
            public long getBuildTimeMs()
            ```

        []{#isManifest()}

        -   #### isManifest

            ``` methodSignature
            @Default
            public boolean isManifest()
            ```

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static ArtifactInfo.Builder builder()
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
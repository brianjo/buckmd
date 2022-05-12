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
[Package]{.packageLabelInType} [com.facebook.buck.rules.coercer](package-summary.html)
:::

## Class ManifestEntries {#class-manifestentries .title title="Class ManifestEntries"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.coercer.ManifestEntries

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`

    ------------------------------------------------------------------------

        public abstract class ManifestEntries
        extends Object
        implements AddsToRuleKey

    ::: block
    Manifest entries to be injected into the AndroidManifest.xml file
    via AAPT command line flags.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                       Description
          ------------------- --------------------------- -------------
          `static class `     `ManifestEntries.Builder`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor           Description
          --------------------- -------------
          `ManifestEntries()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                            Method                    Description
          ---------------------------------------------------------------------------- ------------------------- -------------
          `static ManifestEntries.Builder`                                             `builder()`                
          `static ManifestEntries`                                                     `empty()`                  
          `abstract Optional<Boolean>`                                                 `getDebugMode()`           
          `abstract Optional<Integer>`                                                 `getMinSdkVersion()`       
          `abstract Optional<com.google.common.collect.ImmutableMap<String,​String>>`   `getPlaceholders()`        
          `abstract Optional<Integer>`                                                 `getTargetSdkVersion()`    
          `abstract Optional<Integer>`                                                 `getVersionCode()`         
          `abstract Optional<String>`                                                  `getVersionName()`         
          `boolean`                                                                    `hasAny()`                 

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

        -   #### ManifestEntries

                public ManifestEntries()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getMinSdkVersion()}

        -   #### getMinSdkVersion

            ``` methodSignature
            public abstract Optional<Integer> getMinSdkVersion()
            ```

        []{#getTargetSdkVersion()}

        -   #### getTargetSdkVersion

            ``` methodSignature
            public abstract Optional<Integer> getTargetSdkVersion()
            ```

        []{#getVersionCode()}

        -   #### getVersionCode

            ``` methodSignature
            public abstract Optional<Integer> getVersionCode()
            ```

        []{#getVersionName()}

        -   #### getVersionName

            ``` methodSignature
            public abstract Optional<String> getVersionName()
            ```

        []{#getDebugMode()}

        -   #### getDebugMode

            ``` methodSignature
            public abstract Optional<Boolean> getDebugMode()
            ```

        []{#getPlaceholders()}

        -   #### getPlaceholders

            ``` methodSignature
            public abstract Optional<com.google.common.collect.ImmutableMap<String,​String>> getPlaceholders()
            ```

        []{#hasAny()}

        -   #### hasAny

            ``` methodSignature
            public boolean hasAny()
            ```

            [Returns:]{.returnLabel}
            :   true if and only if at least one of the parameters is
                non-absent.

        []{#empty()}

        -   #### empty

            ``` methodSignature
            public static ManifestEntries empty()
            ```

            [Returns:]{.returnLabel}
            :   an empty (all items set to Optional.empty())
                ManifestEntries

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static ManifestEntries.Builder builder()
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

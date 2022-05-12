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

## Class VersionMatchedCollection\<T\> {#class-versionmatchedcollectiont .title title="Class VersionMatchedCollection"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.coercer.VersionMatchedCollection\<T\>

::: description
-   

    All Implemented Interfaces:
    :   `TargetTranslatable<VersionMatchedCollection<T>>`

    ------------------------------------------------------------------------

        public class VersionMatchedCollection<T>
        extends Object
        implements TargetTranslatable<VersionMatchedCollection<T>>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                                   Description
          ------------------- --------------------------------------- -------------
          `static class `     `VersionMatchedCollection.Builder<T>`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                       Description
          ------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `VersionMatchedCollection​(com.google.common.collect.ImmutableList<Pair<com.google.common.collect.ImmutableMap<BuildTarget,​Version>,​T>> values)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                                                                Method                                                                                                                                            Description
          ---------------------------------------------------------------------------------------------------------------- ------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `static <T> VersionMatchedCollection.Builder<T>`                                                                 `builder()`                                                                                                                                        
          `boolean`                                                                                                        `equals​(Object o)`                                                                                                                                 
          `com.google.common.collect.ImmutableList<T>`                                                                     `getMatchingValues​(com.google.common.collect.ImmutableMap<BuildTarget,​Version> selected)`                                                          
          `T`                                                                                                              `getOnlyMatchingValue​(String source,                     com.google.common.collect.ImmutableMap<BuildTarget,​Version> selected)`                    
          `com.google.common.collect.ImmutableList<Pair<com.google.common.collect.ImmutableMap<BuildTarget,​Version>,​T>>`   `getValuePairs()`                                                                                                                                  
          `com.google.common.collect.ImmutableList<T>`                                                                     `getValues()`                                                                                                                                      
          `int`                                                                                                            `hashCode()`                                                                                                                                       
          `static <T> VersionMatchedCollection<T>`                                                                         `of()`                                                                                                                                             
          `String`                                                                                                         `toString()`                                                                                                                                       
          `Optional<VersionMatchedCollection<T>>`                                                                          `translateTargets​(CellNameResolver cellPathResolver,                 BaseName targetBaseName,                 TargetNodeTranslator translator)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.google.common.collect.ImmutableList)}

        -   #### VersionMatchedCollection

                public VersionMatchedCollection​(com.google.common.collect.ImmutableList<Pair<com.google.common.collect.ImmutableMap<BuildTarget,​Version>,​T>> values)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getMatchingValues(com.google.common.collect.ImmutableMap)}

        -   #### getMatchingValues

            ``` methodSignature
            public com.google.common.collect.ImmutableList<T> getMatchingValues​(com.google.common.collect.ImmutableMap<BuildTarget,​Version> selected)
            ```

        []{#getOnlyMatchingValue(java.lang.String,com.google.common.collect.ImmutableMap)}

        -   #### getOnlyMatchingValue

            ``` methodSignature
            public T getOnlyMatchingValue​(String source,
                                          com.google.common.collect.ImmutableMap<BuildTarget,​Version> selected)
            ```

            [Returns:]{.returnLabel}
            :   the only item that matches the given version map, or
                throw.

        []{#getValues()}

        -   #### getValues

            ``` methodSignature
            public com.google.common.collect.ImmutableList<T> getValues()
            ```

        []{#getValuePairs()}

        -   #### getValuePairs

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Pair<com.google.common.collect.ImmutableMap<BuildTarget,​Version>,​T>> getValuePairs()
            ```

        []{#of()}

        -   #### of

            ``` methodSignature
            public static <T> VersionMatchedCollection<T> of()
            ```

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(Object o)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `Object`

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `Object`

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static <T> VersionMatchedCollection.Builder<T> builder()
            ```

        []{#translateTargets(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.core.model.BaseName,com.facebook.buck.versions.TargetNodeTranslator)}

        -   #### translateTargets

            ``` methodSignature
            public Optional<VersionMatchedCollection<T>> translateTargets​(CellNameResolver cellPathResolver,
                                                                          BaseName targetBaseName,
                                                                          TargetNodeTranslator translator)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `translateTargets` in interface `TargetTranslatable<T>`

            [Returns:]{.returnLabel}
            :   if any changes are required, return the translated
                object.
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

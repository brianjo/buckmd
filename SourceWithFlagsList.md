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

## Class SourceWithFlagsList {#class-sourcewithflagslist .title title="Class SourceWithFlagsList"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.coercer.SourceWithFlagsList

::: description
-   

    ------------------------------------------------------------------------

        public abstract class SourceWithFlagsList
        extends Object

    ::: block
    Simple type representing a list of
    [`SourceWithFlags`](../../core/sourcepath/SourceWithFlags.html "class in com.facebook.buck.core.sourcepath").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                        Description
          ------------------- ---------------------------- -------------
          `static class `     `SourceWithFlagsList.Type`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor               Description
          ------------------------- -------------
          `SourceWithFlagsList()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                                           Method                                                                                                Description
          ------------------------------------------------------------------------------------------- ----------------------------------------------------------------------------------------------------- -------------
          `protected void`                                                                            `check()`                                                                                              
          `abstract Optional<com.google.common.collect.ImmutableSortedMap<String,​SourceWithFlags>>`   `getNamedSources()`                                                                                    
          `abstract SourceWithFlagsList.Type`                                                         `getType()`                                                                                            
          `abstract Optional<com.google.common.collect.ImmutableSortedSet<SourceWithFlags>>`          `getUnnamedSources()`                                                                                  
          `static SourceWithFlagsList`                                                                `ofNamedSources​(com.google.common.collect.ImmutableSortedMap<String,​SourceWithFlags> namedSources)`    
          `static SourceWithFlagsList`                                                                `ofUnnamedSources​(com.google.common.collect.ImmutableSortedSet<SourceWithFlags> unnamedSources)`       

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

        -   #### SourceWithFlagsList

                public SourceWithFlagsList()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getType()}

        -   #### getType

            ``` methodSignature
            public abstract SourceWithFlagsList.Type getType()
            ```

        []{#getUnnamedSources()}

        -   #### getUnnamedSources

            ``` methodSignature
            public abstract Optional<com.google.common.collect.ImmutableSortedSet<SourceWithFlags>> getUnnamedSources()
            ```

        []{#getNamedSources()}

        -   #### getNamedSources

            ``` methodSignature
            public abstract Optional<com.google.common.collect.ImmutableSortedMap<String,​SourceWithFlags>> getNamedSources()
            ```

        []{#check()}

        -   #### check

            ``` methodSignature
            @Check
            protected void check()
            ```

        []{#ofUnnamedSources(com.google.common.collect.ImmutableSortedSet)}

        -   #### ofUnnamedSources

            ``` methodSignature
            public static SourceWithFlagsList ofUnnamedSources​(com.google.common.collect.ImmutableSortedSet<SourceWithFlags> unnamedSources)
            ```

        []{#ofNamedSources(com.google.common.collect.ImmutableSortedMap)}

        -   #### ofNamedSources

            ``` methodSignature
            public static SourceWithFlagsList ofNamedSources​(com.google.common.collect.ImmutableSortedMap<String,​SourceWithFlags> namedSources)
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

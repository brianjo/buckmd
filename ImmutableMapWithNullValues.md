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
[Package]{.packageLabelInType} [com.facebook.buck.util](package-summary.html)
:::

## Class ImmutableMapWithNullValues\<K,​V\> {#class-immutablemapwithnullvalueskv .title title="Class ImmutableMapWithNullValues"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.util.AbstractMap](http://docs.oracle.com/javase/7/docs/api/java/util/AbstractMap.html?is-external=true "class or interface in java.util"){.externalLink}\<K,​V\>

    -   -   com.facebook.buck.util.ImmutableMapWithNullValues\<K,​V\>

::: description
-   

    All Implemented Interfaces:
    :   `Map<K,​V>`

    ------------------------------------------------------------------------

        public final class ImmutableMapWithNullValues<K,​V>
        extends AbstractMap<K,​V>

    ::: block
    `ImmutableMap` uses 16 fewer bytes per entry than
    [`TreeMap`](http://docs.oracle.com/javase/7/docs/api/java/util/TreeMap.html?is-external=true "class or interface in java.util"){.externalLink},
    but does not allow null values. This wrapper class lets us have our
    cake and eat it too \-- we use a sentinel object in the underlying
    `ImmutableMap` and translate it on any read path.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                                       Description
          ------------------- ------------------------------------------- -------------
          `static class `     `ImmutableMapWithNullValues.Builder<K,​V>`    

          : Nested Classes[ ]{.tabEnd}

        -   []{#nested.classes.inherited.from.class.java.util.AbstractMap}

            ### Nested classes/interfaces inherited from class java.util.[AbstractMap](http://docs.oracle.com/javase/7/docs/api/java/util/AbstractMap.html?is-external=true "class or interface in java.util"){.externalLink}

            `AbstractMap.SimpleEntry<K extends Object,​V extends Object>, AbstractMap.SimpleImmutableEntry<K extends Object,​V extends Object>`

        ```{=html}
        <!-- -->
        ```
        -   []{#nested.classes.inherited.from.class.java.util.Map}

            ### Nested classes/interfaces inherited from interface java.util.[Map](http://docs.oracle.com/javase/7/docs/api/java/util/Map.html?is-external=true "class or interface in java.util"){.externalLink}

            `Map.Entry<K extends Object,​V extends Object>`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type       Method                   Description
          ----------------------- ------------------------ -------------
          `Set<Map.Entry<K,​V>>`   `entrySet()`              
          `boolean`               `equals​(Object other)`    
          `V`                     `get​(Object key)`         
          `int`                   `hashCode()`              
          `String`                `toString()`              
          `Collection<V>`         `values()`                

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.util.AbstractMap}

            ### Methods inherited from class java.util.[AbstractMap](http://docs.oracle.com/javase/7/docs/api/java/util/AbstractMap.html?is-external=true "class or interface in java.util"){.externalLink}

            `clear, clone, containsKey, containsValue, isEmpty, keySet, put, putAll, remove, size`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `finalize, getClass, notify, notifyAll, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.util.Map}

            ### Methods inherited from interface java.util.[Map](http://docs.oracle.com/javase/7/docs/api/java/util/Map.html?is-external=true "class or interface in java.util"){.externalLink}

            `compute, computeIfAbsent, computeIfPresent, forEach, getOrDefault, merge, putIfAbsent, remove, replace, replace, replaceAll`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#get(java.lang.Object)}

        -   #### get

            ``` methodSignature
            @Nullable
            public V get​(@Nullable
                         Object key)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `get` in interface `Map<K,​V>`

            [Overrides:]{.overrideSpecifyLabel}
            :   `get` in class `AbstractMap<K,​V>`

        []{#values()}

        -   #### values

            ``` methodSignature
            public Collection<V> values()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `values` in interface `Map<K,​V>`

            [Overrides:]{.overrideSpecifyLabel}
            :   `values` in class `AbstractMap<K,​V>`

        []{#entrySet()}

        -   #### entrySet

            ``` methodSignature
            public Set<Map.Entry<K,​V>> entrySet()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `entrySet` in interface `Map<K,​V>`

            [Specified by:]{.overrideSpecifyLabel}
            :   `entrySet` in class `AbstractMap<K,​V>`

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(Object other)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `equals` in interface `Map<K,​V>`

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `AbstractMap<K,​V>`

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `hashCode` in interface `Map<K,​V>`

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `AbstractMap<K,​V>`

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `AbstractMap<K,​V>`
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

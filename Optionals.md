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
[Package]{.packageLabelInType} [com.facebook.buck.core.util](package-summary.html)
:::

## Class Optionals {#class-optionals .title title="Class Optionals"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.util.Optionals

::: description
-   

    ------------------------------------------------------------------------

        public class Optionals
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                       Method                                                                                                                                Description
          --------------------------------------- ------------------------------------------------------------------------------------------------------------------------------------- -------------
          `static <T> void`                       `addIfPresent​(Optional<T> optional,             com.google.common.collect.ImmutableCollection.Builder<T> collection)`                  
          `static <T,​U>Optional<U>`               `bind​(Optional<? extends T> optional,     java.util.function.Function<? super T,​Optional<U>> f)`                                       
          `static <T extends Comparable<T>>int`   `compare​(Optional<T> first,        Optional<T> second)`                                                                                
          `static Optional<Boolean>`              `ofBoolean​(boolean b)`                                                                                                                 
          `static <K,​T>void`                      `putIfPresent​(Optional<T> optional,             K key,             com.google.common.collect.ImmutableMap.Builder<K,​T> collection)`    
          `static <T> T`                          `require​(Optional<T> optional)`                                                                                                        

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

        []{#addIfPresent(java.util.Optional,com.google.common.collect.ImmutableCollection.Builder)}

        -   #### addIfPresent

            ``` methodSignature
            public static <T> void addIfPresent​(Optional<T> optional,
                                                com.google.common.collect.ImmutableCollection.Builder<T> collection)
            ```

        []{#putIfPresent(java.util.Optional,java.lang.Object,com.google.common.collect.ImmutableMap.Builder)}
        []{#putIfPresent(java.util.Optional,K,com.google.common.collect.ImmutableMap.Builder)}

        -   #### putIfPresent

            ``` methodSignature
            public static <K,​T> void putIfPresent​(Optional<T> optional,
                                                        K key,
                                                        com.google.common.collect.ImmutableMap.Builder<K,​T> collection)
            ```

        []{#bind(java.util.Optional,java.util.function.Function)}

        -   #### bind

            ``` methodSignature
            public static <T,​U> Optional<U> bind​(Optional<? extends T> optional,
                                                       java.util.function.Function<? super T,​Optional<U>> f)
            ```

        []{#compare(java.util.Optional,java.util.Optional)}

        -   #### compare

            ``` methodSignature
            public static <T extends Comparable<T>> int compare​(Optional<T> first,
                                                                Optional<T> second)
            ```

        []{#require(java.util.Optional)}

        -   #### require

            ``` methodSignature
            public static <T> T require​(Optional<T> optional)
            ```

        []{#ofBoolean(boolean)}

        -   #### ofBoolean

            ``` methodSignature
            public static Optional<Boolean> ofBoolean​(boolean b)
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

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
[Package]{.packageLabelInType} [com.facebook.buck.rules.coercer](package-summary.html)
:::

## Class PatternMatchedCollection\<T\> {#class-patternmatchedcollectiont .title title="Class PatternMatchedCollection"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.coercer.PatternMatchedCollection\<T\>

::: description
-   

    All Implemented Interfaces:
    :   `TargetTranslatable<PatternMatchedCollection<T>>`

    ------------------------------------------------------------------------

        public class PatternMatchedCollection<T>
        extends Object
        implements TargetTranslatable<PatternMatchedCollection<T>>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                                   Description
          ------------------- --------------------------------------- -------------
          `static class `     `PatternMatchedCollection.Builder<T>`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `stati                | `builder()`           |                       |
        | c <T> PatternMatchedC |                       |                       |
        | ollection.Builder<T>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static <T> Pattern   | `concat​(Iterable<     |                       |
        | MatchedCollection<T>` | PatternMatchedCollect |                       |
        |                       | ion<T>> collections)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `equals​(Object o)`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `forEachMatchi        | ::: block             |
        |                       | ngValue​(String string | Apply `consumer` to   |
        |                       | ,                     | all values whose      |
        |                       |  java.util.function.C | [`Patte               |
        |                       | onsumer<T> consumer)` | rn`](http://docs.orac |
        |                       |                       | le.com/javase/7/docs/ |
        |                       |                       | api/java/util/regex/P |
        |                       |                       | attern.html?is-extern |
        |                       |                       | al=true "class or int |
        |                       |                       | erface in java.util.r |
        |                       |                       | egex"){.externalLink} |
        |                       |                       | matches `string`.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `forEachValue         | ::: block             |
        |                       | ​(java.util.function.C | Apply `consumer` to   |
        |                       | onsumer<T> consumer)` | all values.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `c                    | `getMatchingV         |                       |
        | om.google.common.coll | alues​(String string)` |                       |
        | ect.ImmutableList<T>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.comm      | `ge                   |                       |
        | on.collect.ImmutableL | tPatternsAndValues()` |                       |
        | ist<Pair<Pattern,​T>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `c                    | `getValues()`         |                       |
        | om.google.common.coll |                       |                       |
        | ect.ImmutableList<T>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `<V> Pattern          | `m                    |                       |
        | MatchedCollection<V>` | ap​(java.util.function |                       |
        |                       | .Function<T,​V> func)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static <T> Pattern   | `of()`                |                       |
        | MatchedCollection<T>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<PatternM    | `translateTargets     |                       |
        | atchedCollection<T>>` | ​(CellNameResolver cel |                       |
        |                       | lPathResolver,        |                       |
        |                       |           BaseName ta |                       |
        |                       | rgetBaseName,         |                       |
        |                       |          TargetNodeTr |                       |
        |                       | anslator translator)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#forEachMatchingValue(java.lang.String,java.util.function.Consumer)}

        -   #### forEachMatchingValue

            ``` methodSignature
            public void forEachMatchingValue​(String string,
                                             java.util.function.Consumer<T> consumer)
            ```

            ::: block
            Apply `consumer` to all values whose
            [`Pattern`](http://docs.oracle.com/javase/7/docs/api/java/util/regex/Pattern.html?is-external=true "class or interface in java.util.regex"){.externalLink}
            matches `string`.
            :::

        []{#getMatchingValues(java.lang.String)}

        -   #### getMatchingValues

            ``` methodSignature
            public com.google.common.collect.ImmutableList<T> getMatchingValues​(String string)
            ```

            [Returns:]{.returnLabel}
            :   all values whose
                [`Pattern`](http://docs.oracle.com/javase/7/docs/api/java/util/regex/Pattern.html?is-external=true "class or interface in java.util.regex"){.externalLink}
                matches `string`.

        []{#getPatternsAndValues()}

        -   #### getPatternsAndValues

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Pair<Pattern,​T>> getPatternsAndValues()
            ```

        []{#forEachValue(java.util.function.Consumer)}

        -   #### forEachValue

            ``` methodSignature
            public void forEachValue​(java.util.function.Consumer<T> consumer)
            ```

            ::: block
            Apply `consumer` to all values.
            :::

        []{#getValues()}

        -   #### getValues

            ``` methodSignature
            public com.google.common.collect.ImmutableList<T> getValues()
            ```

        []{#translateTargets(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.core.model.BaseName,com.facebook.buck.versions.TargetNodeTranslator)}

        -   #### translateTargets

            ``` methodSignature
            public Optional<PatternMatchedCollection<T>> translateTargets​(CellNameResolver cellPathResolver,
                                                                          BaseName targetBaseName,
                                                                          TargetNodeTranslator translator)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `translateTargets` in interface `TargetTranslatable<T>`

            [Returns:]{.returnLabel}
            :   if any changes are required, return the translated
                object.

        []{#of()}

        -   #### of

            ``` methodSignature
            public static <T> PatternMatchedCollection<T> of()
            ```

        []{#map(java.util.function.Function)}

        -   #### map

            ``` methodSignature
            public <V> PatternMatchedCollection<V> map​(java.util.function.Function<T,​V> func)
            ```

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

        []{#concat(java.lang.Iterable)}

        -   #### concat

            ``` methodSignature
            public static <T> PatternMatchedCollection<T> concat​(Iterable<PatternMatchedCollection<T>> collections)
            ```

            [Returns:]{.returnLabel}
            :   a single
                [`PatternMatchedCollection`](PatternMatchedCollection.html "class in com.facebook.buck.rules.coercer")
                formed by combining the given input
                [`PatternMatchedCollection`](PatternMatchedCollection.html "class in com.facebook.buck.rules.coercer")s.

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static <T> PatternMatchedCollection.Builder<T> builder()
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

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
[Package]{.packageLabelInType} [com.facebook.buck.core.model](package-summary.html)
:::

## Class FlavorDomain\<T\> {#class-flavordomaint .title title="Class FlavorDomain"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.model.FlavorDomain\<T\>

::: description
-   

    ------------------------------------------------------------------------

        public class FlavorDomain<T>
        extends Object

    ::: block
    Provides a named flavor abstraction on top of boolean flavors.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                             Description
          ------------------------------------------------------------------------------------------------------- -------------
          `FlavorDomain​(String name,             com.google.common.collect.ImmutableMap<Flavor,​T> translation)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `boolean`             | `con                  |                       |
        |                       | tains​(Flavor flavor)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `containsAnyO         |                       |
        |                       | f​(FlavorSet flavors)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `containsAnyOf​(       |                       |
        |                       | Set<Flavor> flavors)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `<U                   | `convert​(String       | ::: block             |
        | extends FlavorConvert |  name,        java.ut | Provides a            |
        | ible>FlavorDomain<U>` | il.function.Function< | convenience for       |
        |                       | ? super T,​U> mapper)` | converting from one   |
        |                       |                       | domain to another.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static <E extends En | `from​(String nam      | ::: block             |
        | um<E> & FlavorConvert | e,     Class<E> cls)` | Create a FlavorDomain |
        | ible>FlavorDomain<E>` |                       | from FlavorConverbile |
        |                       |                       | Enum.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static <T            | `f                    | ::: block             |
        | extends FlavorConvert | rom​(String name,      | Create a FlavorDomain |
        | ible>FlavorDomain<T>` | Iterable<T> objects)` | from                  |
        |                       |                       | FlavorConvertible     |
        |                       |                       | objects.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Flavor>`    | `getFlavor​(Buil       |                       |
        |                       | dTarget buildTarget)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Flavor>`    | `getFlavor​(           |                       |
        |                       | FlavorSet flavorSet)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Flavor>`    | `getFlavor​(           |                       |
        |                       | Set<Flavor> flavors)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<            | `g                    |                       |
        | Map.Entry<Flavor,​T>>` | etFlavorAndValue​(Buil |                       |
        |                       | dTarget buildTarget)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<            | `getFlavorAndValu     |                       |
        | Map.Entry<Flavor,​T>>` | e​(FlavorSet flavors)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<            | `getFlavorAndValue​(   |                       |
        | Map.Entry<Flavor,​T>>` | Set<Flavor> flavors)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.g                | `getFlavors()`        |                       |
        | oogle.common.collect. |                       |                       |
        | ImmutableSet<Flavor>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getName()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `T`                   | `                     |                       |
        |                       | getRequiredValue​(Buil |                       |
        |                       | dTarget buildTarget)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<T>`         | `getValue​(Buil        |                       |
        |                       | dTarget buildTarget)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `T`                   | `get                  |                       |
        |                       | Value​(Flavor flavor)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<T>`         | `getValu              |                       |
        |                       | e​(FlavorSet flavors)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<T>`         | `getValue​(            |                       |
        |                       | Set<Flavor> flavors)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.goo              | `getValues()`         |                       |
        | gle.common.collect.Im |                       |                       |
        | mutableCollection<T>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `c                    | `getValues​(Buil       |                       |
        | om.google.common.coll | dTarget buildTarget)` |                       |
        | ect.ImmutableList<T>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `<U> FlavorDomain<U>` | `map​(St               | ::: block             |
        |                       | ring name,    java.ut | Provides a            |
        |                       | il.function.Function< | convenience function  |
        |                       | ? super T,​U> mapper)` | to map the values of  |
        |                       |                       | the domain.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `<U> FlavorDomain<U>` | `map​(java.ut          | ::: block             |
        |                       | il.function.Function< | Provides a            |
        |                       | ? super T,​U> mapper)` | convenience function  |
        |                       |                       | to map the values of  |
        |                       |                       | the domain (retaining |
        |                       |                       | the current name).    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static <T            | `of​(String n          | ::: block             |
        | extends FlavorConvert | ame,   T... objects)` | Create a FlavorDomain |
        | ible>FlavorDomain<T>` |                       | from array/varargs of |
        |                       |                       | FlavorConvertible     |
        |                       |                       | objects.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
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

        []{#<init>(java.lang.String,com.google.common.collect.ImmutableMap)}

        -   #### FlavorDomain

                public FlavorDomain​(String name,
                                    com.google.common.collect.ImmutableMap<Flavor,​T> translation)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getName()}

        -   #### getName

            ``` methodSignature
            public String getName()
            ```

        []{#getFlavors()}

        -   #### getFlavors

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<Flavor> getFlavors()
            ```

        []{#getValues()}

        -   #### getValues

            ``` methodSignature
            public com.google.common.collect.ImmutableCollection<T> getValues()
            ```

        []{#containsAnyOf(java.util.Set)}

        -   #### containsAnyOf

            ``` methodSignature
            public boolean containsAnyOf​(Set<Flavor> flavors)
            ```

        []{#containsAnyOf(com.facebook.buck.core.model.FlavorSet)}

        -   #### containsAnyOf

            ``` methodSignature
            public boolean containsAnyOf​(FlavorSet flavors)
            ```

        []{#map(java.util.function.Function)}

        -   #### map

            ``` methodSignature
            public <U> FlavorDomain<U> map​(java.util.function.Function<? super T,​U> mapper)
            ```

            ::: block
            Provides a convenience function to map the values of the
            domain (retaining the current name).
            :::

        []{#map(java.lang.String,java.util.function.Function)}

        -   #### map

            ``` methodSignature
            public <U> FlavorDomain<U> map​(String name,
                                           java.util.function.Function<? super T,​U> mapper)
            ```

            ::: block
            Provides a convenience function to map the values of the
            domain.
            :::

        []{#convert(java.lang.String,java.util.function.Function)}

        -   #### convert

            ``` methodSignature
            public <U extends FlavorConvertible> FlavorDomain<U> convert​(String name,
                                                                         java.util.function.Function<? super T,​U> mapper)
            ```

            ::: block
            Provides a convenience for converting from one domain to
            another. This is similar to map(), but the new domain has
            flavors derived from the mapped to
            [`FlavorConvertible`](FlavorConvertible.html "interface in com.facebook.buck.core.model").
            :::

        []{#contains(com.facebook.buck.core.model.Flavor)}

        -   #### contains

            ``` methodSignature
            public boolean contains​(Flavor flavor)
            ```

        []{#getFlavor(java.util.Set)}

        -   #### getFlavor

            ``` methodSignature
            public Optional<Flavor> getFlavor​(Set<Flavor> flavors)
            ```

        []{#getFlavor(com.facebook.buck.core.model.FlavorSet)}

        -   #### getFlavor

            ``` methodSignature
            public Optional<Flavor> getFlavor​(FlavorSet flavorSet)
            ```

        []{#getFlavor(com.facebook.buck.core.model.BuildTarget)}

        -   #### getFlavor

            ``` methodSignature
            public Optional<Flavor> getFlavor​(BuildTarget buildTarget)
            ```

        []{#getFlavorAndValue(java.util.Set)}

        -   #### getFlavorAndValue

            ``` methodSignature
            public Optional<Map.Entry<Flavor,​T>> getFlavorAndValue​(Set<Flavor> flavors)
            ```

        []{#getFlavorAndValue(com.facebook.buck.core.model.FlavorSet)}

        -   #### getFlavorAndValue

            ``` methodSignature
            public Optional<Map.Entry<Flavor,​T>> getFlavorAndValue​(FlavorSet flavors)
            ```

        []{#getFlavorAndValue(com.facebook.buck.core.model.BuildTarget)}

        -   #### getFlavorAndValue

            ``` methodSignature
            public Optional<Map.Entry<Flavor,​T>> getFlavorAndValue​(BuildTarget buildTarget)
            ```

        []{#getValue(java.util.Set)}

        -   #### getValue

            ``` methodSignature
            public Optional<T> getValue​(Set<Flavor> flavors)
            ```

        []{#getValue(com.facebook.buck.core.model.FlavorSet)}

        -   #### getValue

            ``` methodSignature
            public Optional<T> getValue​(FlavorSet flavors)
            ```

        []{#getValue(com.facebook.buck.core.model.BuildTarget)}

        -   #### getValue

            ``` methodSignature
            public Optional<T> getValue​(BuildTarget buildTarget)
            ```

        []{#getValues(com.facebook.buck.core.model.BuildTarget)}

        -   #### getValues

            ``` methodSignature
            public com.google.common.collect.ImmutableList<T> getValues​(BuildTarget buildTarget)
            ```

            [Returns:]{.returnLabel}
            :   a list of values for the flavors from the given target.
                Target\'s flavors that are not present in this domain
                are ignored.

        []{#getRequiredValue(com.facebook.buck.core.model.BuildTarget)}

        -   #### getRequiredValue

            ``` methodSignature
            public T getRequiredValue​(BuildTarget buildTarget)
            ```

        []{#getValue(com.facebook.buck.core.model.Flavor)}

        -   #### getValue

            ``` methodSignature
            public T getValue​(Flavor flavor)
            ```

        []{#from(java.lang.String,java.lang.Iterable)}

        -   #### from

            ``` methodSignature
            public static <T extends FlavorConvertible> FlavorDomain<T> from​(String name,
                                                                             Iterable<T> objects)
            ```

            ::: block
            Create a FlavorDomain from FlavorConvertible objects.
            :::

        []{#of(java.lang.String,com.facebook.buck.core.model.FlavorConvertible[])}
        []{#of(java.lang.String,T...)}

        -   #### of

            ``` methodSignature
            @SafeVarargs
            public static <T extends FlavorConvertible> FlavorDomain<T> of​(String name,
                                                                           T... objects)
            ```

            ::: block
            Create a FlavorDomain from array/varargs of
            FlavorConvertible objects.
            :::

        []{#from(java.lang.String,java.lang.Class)}

        -   #### from

            ``` methodSignature
            public static <E extends Enum<E> & FlavorConvertible> FlavorDomain<E> from​(String name,
                                                                                       Class<E> cls)
            ```

            ::: block
            Create a FlavorDomain from FlavorConverbile Enum.
            :::
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

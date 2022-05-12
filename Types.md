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
[Package]{.packageLabelInType} [com.facebook.buck.util](package-summary.html)
:::

## Class Types {#class-types .title title="Class Types"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.Types

::: description
-   

    ------------------------------------------------------------------------

        public class Types
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static Type`         | `getB                 | ::: block             |
        |                       | aseType​(Field field)` | Determine the \"base  |
        |                       |                       | type\" of a field.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Class<? ex    | `getContain           |                       |
        | tends Collection<?>>` | erClass​(Field field)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Type`         | `getFirstNonOptio     | ::: block             |
        |                       | nalType​(Field field)` | Get the first         |
        |                       |                       | complete              |
        |                       |                       | [`Typ                 |
        |                       |                       | e`](http://docs.oracl |
        |                       |                       | e.com/javase/7/docs/a |
        |                       |                       | pi/java/lang/reflect/ |
        |                       |                       | Type.html?is-external |
        |                       |                       | =true "class or inter |
        |                       |                       | face in java.lang.ref |
        |                       |                       | lect"){.externalLink} |
        |                       |                       | in a signature        |
        |                       |                       | that\'s non-optional, |
        |                       |                       | complete with the     |
        |                       |                       | information from the  |
        |                       |                       | [`Parameter           |
        |                       |                       | izedType`](http://doc |
        |                       |                       | s.oracle.com/javase/7 |
        |                       |                       | /docs/api/java/lang/r |
        |                       |                       | eflect/ParameterizedT |
        |                       |                       | ype.html?is-external= |
        |                       |                       | true "class or interf |
        |                       |                       | ace in java.lang.refl |
        |                       |                       | ect"){.externalLink}. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static com.goo       | `getSupert            | ::: block             |
        | gle.common.collect.Im | ypes​(Class<?> clazz)` | Returns a Set of      |
        | mutableSet<Class<?>>` |                       | classes and           |
        |                       |                       | interfaces inherited  |
        |                       |                       | or implemented by     |
        |                       |                       | clazz.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

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

        []{#getBaseType(java.lang.reflect.Field)}

        -   #### getBaseType

            ``` methodSignature
            public static Type getBaseType​(Field field)
            ```

            ::: block
            Determine the \"base type\" of a field. That is, the
            following will be returned:
            -   `String` -\> `String.class`
            -   `Optional&lt;String&gt;` -\> `String.class`
            -   `Set&lt;String&gt;` -\> `String.class`
            -   `Collection&lt;? extends Comparable&gt;` -\>
                `Comparable.class`
            -   `Collection&lt;? super Comparable` -\> `Object.class`
            :::

        []{#getContainerClass(java.lang.reflect.Field)}

        -   #### getContainerClass

            ``` methodSignature
            @Nullable
            public static Class<? extends Collection<?>> getContainerClass​(Field field)
            ```

            [Returns:]{.returnLabel}
            :   The raw type of the
                [`Collection`](http://docs.oracle.com/javase/7/docs/api/java/util/Collection.html?is-external=true "class or interface in java.util"){.externalLink}
                a field represents, even if contained in an
                [`Optional`](http://docs.oracle.com/javase/7/docs/api/java/util/Optional.html?is-external=true "class or interface in java.util"){.externalLink},
                but without the ParameterizedType information.

        []{#getFirstNonOptionalType(java.lang.reflect.Field)}

        -   #### getFirstNonOptionalType

            ``` methodSignature
            public static Type getFirstNonOptionalType​(Field field)
            ```

            ::: block
            Get the first complete
            [`Type`](http://docs.oracle.com/javase/7/docs/api/java/lang/reflect/Type.html?is-external=true "class or interface in java.lang.reflect"){.externalLink}
            in a signature that\'s non-optional, complete with the
            information from the
            [`ParameterizedType`](http://docs.oracle.com/javase/7/docs/api/java/lang/reflect/ParameterizedType.html?is-external=true "class or interface in java.lang.reflect"){.externalLink}.
            -   String -\> String
            -   Optional\<String\$gt; -\> String
            -   ImmutableSet\<String\> -\> ImmutableSet\<String\>
            -   Optional\<ImmutableSet\<String\>\> -\>
                ImmutableSet\<String\>
            :::

        []{#getSupertypes(java.lang.Class)}

        -   #### getSupertypes

            ``` methodSignature
            public static com.google.common.collect.ImmutableSet<Class<?>> getSupertypes​(Class<?> clazz)
            ```

            ::: block
            Returns a Set of classes and interfaces inherited or
            implemented by clazz.
            Result includes clazz itself. Result is ordered closest to
            furthest, i.e. first entry will always be clazz and last
            entry will always be
            [`Object`](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}.
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

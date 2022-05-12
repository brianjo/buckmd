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
[Package]{.packageLabelInType} [com.facebook.buck.parser.api](package-summary.html)
:::

## Class BuildFileManifestPojoizer.PojoTransformer {#class-buildfilemanifestpojoizer.pojotransformer .title title="Class BuildFileManifestPojoizer.PojoTransformer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.parser.api.BuildFileManifestPojoizer.PojoTransformer

::: description
-   

    Enclosing class:
    :   [BuildFileManifestPojoizer](BuildFileManifestPojoizer.html "class in com.facebook.buck.parser.api")

    ------------------------------------------------------------------------

        public abstract static class BuildFileManifestPojoizer.PojoTransformer
        extends Object

    ::: block
    Container to hold transformation function for classes assignable to
    a provided class. The result of the transformation is supposed to be
    a POJO class accepted by
    [`BuildFileManifest`](BuildFileManifest.html "class in com.facebook.buck.parser.api")
    protocol.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor           Description
          --------------------- -------------
          `PojoTransformer()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `abstract Class<?>`   | `getClazz()`          | ::: block             |
        |                       |                       | Return a type that    |
        |                       |                       | transformer is able   |
        |                       |                       | to transform from;    |
        |                       |                       | the real object       |
        |                       |                       | should be assignable  |
        |                       |                       | to this class, so     |
        |                       |                       | base classes and      |
        |                       |                       | interfaces can be     |
        |                       |                       | used too              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract j           | `ge                   | ::: block             |
        | ava.util.function.Fun | tTransformFunction()` | Function that         |
        | ction<Object,​Object>` |                       | transforms a parser   |
        |                       |                       | object to POJO object |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `of​(Class<?> clazz,   |                       |
        | BuildFileManifestPojo |  java.util.function.F |                       |
        | izer.PojoTransformer` | unction<Object,​Object |                       |
        |                       | > transformFunction)` |                       |
        +-----------------------+-----------------------+-----------------------+

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

        -   #### PojoTransformer

                public PojoTransformer()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getClazz()}

        -   #### getClazz

            ``` methodSignature
            public abstract Class<?> getClazz()
            ```

            ::: block
            Return a type that transformer is able to transform from;
            the real object should be assignable to this class, so base
            classes and interfaces can be used too
            :::

        []{#getTransformFunction()}

        -   #### getTransformFunction

            ``` methodSignature
            public abstract java.util.function.Function<Object,​Object> getTransformFunction()
            ```

            ::: block
            Function that transforms a parser object to POJO object
            :::

        []{#of(java.lang.Class,java.util.function.Function)}

        -   #### of

            ``` methodSignature
            public static BuildFileManifestPojoizer.PojoTransformer of​(Class<?> clazz,
                                                                       java.util.function.Function<Object,​Object> transformFunction)
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

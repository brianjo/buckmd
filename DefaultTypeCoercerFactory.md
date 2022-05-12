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
[Package]{.packageLabelInType} [com.facebook.buck.rules.coercer](package-summary.html)
:::

## Class DefaultTypeCoercerFactory {#class-defaulttypecoercerfactory .title title="Class DefaultTypeCoercerFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.coercer.DefaultTypeCoercerFactory

::: description
-   

    All Implemented Interfaces:
    :   `TypeCoercerFactory`

    ------------------------------------------------------------------------

        public class DefaultTypeCoercerFactory
        extends Object
        implements TypeCoercerFactory

    ::: block
    Create
    [`TypeCoercer`](TypeCoercer.html "interface in com.facebook.buck.rules.coercer")s
    that can convert incoming java structures (from json) into
    particular types.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                     Description
          ------------------------------- -------------
          `DefaultTypeCoercerFactory()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `<T extends DataTrans | `getC                 | ::: block             |
        | ferObject>DataTransfe | onstructorArgDescript | Returns an            |
        | rObjectDescriptor<T>` | or​(Class<T> dtoType)` | unpopulated DTO       |
        |                       |                       | object, and the build |
        |                       |                       | method which must be  |
        |                       |                       | called with it when   |
        |                       |                       | it is finished being  |
        |                       |                       | populated.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `typeCo               |                       |
        | <T> TypeCoercer<?,​T>` | ercerForType​(com.goog |                       |
        |                       | le.common.reflect.Typ |                       |
        |                       | eToken<T> typeToken)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
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

        []{#<init>()}

        -   #### DefaultTypeCoercerFactory

                public DefaultTypeCoercerFactory()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#typeCoercerForType(com.google.common.reflect.TypeToken)}

        -   #### typeCoercerForType

            ``` methodSignature
            public <T> TypeCoercer<?,​T> typeCoercerForType​(com.google.common.reflect.TypeToken<T> typeToken)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `typeCoercerForType` in interface `TypeCoercerFactory`

        []{#getConstructorArgDescriptor(java.lang.Class)}

        -   #### getConstructorArgDescriptor

            ``` methodSignature
            public <T extends DataTransferObject> DataTransferObjectDescriptor<T> getConstructorArgDescriptor​(Class<T> dtoType)
            ```

            ::: block
            [Description copied from
            interface: `TypeCoercerFactory`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns an unpopulated DTO object, and the build method
            which must be called with it when it is finished being
            populated.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getConstructorArgDescriptor` in
                interface `TypeCoercerFactory`
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

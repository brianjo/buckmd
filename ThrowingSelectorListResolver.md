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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.select.impl](package-summary.html)
:::

## Class ThrowingSelectorListResolver {#class-throwingselectorlistresolver .title title="Class ThrowingSelectorListResolver"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.select.impl.ThrowingSelectorListResolver

::: description
-   

    All Implemented Interfaces:
    :   `SelectorListResolver`

    ------------------------------------------------------------------------

        public class ThrowingSelectorListResolver
        extends Object
        implements SelectorListResolver

    ::: block
    Selector list resolver which throws unconditionally
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                        Description
          ---------------------------------- -------------
          `ThrowingSelectorListResolver()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `<T> T`               | `reso                 | ::: block             |
        |                       | lveList​(SelectableCon | Throw unconditionally |
        |                       | figurationContext con | :::                   |
        |                       | figurationContext,    |                       |
        |                       |          BuildTarget  |                       |
        |                       | buildTarget,          |                       |
        |                       |    String attributeNa |                       |
        |                       | me,            Select |                       |
        |                       | orList<T> selectorLis |                       |
        |                       | t,            Concata |                       |
        |                       | ble<T> concatable,    |                       |
        |                       |          DependencySt |                       |
        |                       | ack dependencyStack)` |                       |
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

        -   #### ThrowingSelectorListResolver

                public ThrowingSelectorListResolver()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#resolveList(com.facebook.buck.core.select.SelectableConfigurationContext,com.facebook.buck.core.model.BuildTarget,java.lang.String,com.facebook.buck.core.select.SelectorList,com.facebook.buck.rules.coercer.concat.Concatable,com.facebook.buck.core.exceptions.DependencyStack)}

        -   #### resolveList

            ``` methodSignature
            @Nullable
            public <T> T resolveList​(SelectableConfigurationContext configurationContext,
                                     BuildTarget buildTarget,
                                     String attributeName,
                                     SelectorList<T> selectorList,
                                     Concatable<T> concatable,
                                     DependencyStack dependencyStack)
            ```

            ::: block
            Throw unconditionally
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `resolveList` in interface `SelectorListResolver`

            [Type Parameters:]{.paramLabel}
            :   `T` - the type of elements stored in the provided
                selectable list
            :   `buildTarget` - the build target that contains the given
                list in its arguments
            :   `attributeName` - the name of the attribute that holds
                the given selector list
            :   `selectorList` - a list with selectable elements
            :   `concatable` - to be used when concatenating select
                items (e. g. lists or strings)
            :   `dependencyStack` - used to provide error stacks

            [Returns:]{.returnLabel}
            :   an object produced by concatenating resolved elements of
                the given list or `null` if the list is resolved to an
                absent element
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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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

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
-   [Field](#field.summary) \| 
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

## Class DefaultSelectorListResolver {#class-defaultselectorlistresolver .title title="Class DefaultSelectorListResolver"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.select.AbstractSelectorListResolver](../AbstractSelectorListResolver.html "class in com.facebook.buck.core.select")

    -   -   com.facebook.buck.core.select.impl.DefaultSelectorListResolver

::: description
-   

    All Implemented Interfaces:
    :   `SelectorListResolver`

    ------------------------------------------------------------------------

        public class DefaultSelectorListResolver
        extends AbstractSelectorListResolver

    ::: block
    A
    [`SelectorListResolver`](../SelectorListResolver.html "interface in com.facebook.buck.core.select")
    that finds the most specialized condition in the given list and
    concatenates the results.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.core.select.AbstractSelectorListResolver}

            ### Fields inherited from class com.facebook.buck.core.select.[AbstractSelectorListResolver](../AbstractSelectorListResolver.html "class in com.facebook.buck.core.select")

            `NULL_VALUE`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                            Description
          ---------------------------------------------------------------------- -------------
          `DefaultSelectorListResolver​(SelectableResolver selectableResolver)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                                                                                                                                                                     Description
          ------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `protected <T> T`   `resolveSelector​(SelectableConfigurationContext configurationContext,                BuildTarget buildTarget,                DependencyStack dependencyStack,                String attributeName,                Selector<T> selector)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.select.AbstractSelectorListResolver}

            ### Methods inherited from class com.facebook.buck.core.select.[AbstractSelectorListResolver](../AbstractSelectorListResolver.html "class in com.facebook.buck.core.select")

            `assertNotMultipleMatches, assertSelectorHasDefault, findMatchingConditions, resolveList`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.select.SelectableResolver)}

        -   #### DefaultSelectorListResolver

                public DefaultSelectorListResolver​(SelectableResolver selectableResolver)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#resolveSelector(com.facebook.buck.core.select.SelectableConfigurationContext,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.exceptions.DependencyStack,java.lang.String,com.facebook.buck.core.select.Selector)}

        -   #### resolveSelector

            ``` methodSignature
            @Nullable
            protected <T> T resolveSelector​(SelectableConfigurationContext configurationContext,
                                            BuildTarget buildTarget,
                                            DependencyStack dependencyStack,
                                            String attributeName,
                                            Selector<T> selector)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `resolveSelector` in
                class `AbstractSelectorListResolver`
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
-   [Field](#field.summary) \| 
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

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
-   [Field](#field.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.rules.keys](package-summary.html)
:::

## Class DefaultRuleKeyScopedHasher.DefaultContainerScope {#class-defaultrulekeyscopedhasher.defaultcontainerscope .title title="Class DefaultRuleKeyScopedHasher.DefaultContainerScope"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.keys.DefaultRuleKeyScopedHasher.DefaultContainerScope

::: description
-   

    All Implemented Interfaces:
    :   `RuleKeyScopedHasher.ContainerScope`, `Scope`, `AutoCloseable`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [DefaultRuleKeyScopedHasher](DefaultRuleKeyScopedHasher.html "class in com.facebook.buck.rules.keys")\<[HASH](DefaultRuleKeyScopedHasher.html "type parameter in DefaultRuleKeyScopedHasher")\>

    ------------------------------------------------------------------------

        public static class DefaultRuleKeyScopedHasher.DefaultContainerScope
        extends Object
        implements RuleKeyScopedHasher.ContainerScope
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.util.Scope}

            ### Fields inherited from interface com.facebook.buck.util.[Scope](../../util/Scope.html "interface in com.facebook.buck.util")

            `NOOP`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `close()`             | ::: block             |
        |                       |                       | Hashes the container  |
        |                       |                       | iff non-empty (i.e.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Scope`               | `elementScope()`      | ::: block             |
        |                       |                       | Increases element     |
        |                       |                       | count if anything     |
        |                       |                       | gets hashed during    |
        |                       |                       | the element scope.    |
        |                       |                       | :::                   |
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
    -   []{#method.detail}

        ### Method Detail

        []{#elementScope()}

        -   #### elementScope

            ``` methodSignature
            public Scope elementScope()
            ```

            ::: block
            Increases element count if anything gets hashed during the
            element scope.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `elementScope` in
                interface `RuleKeyScopedHasher.ContainerScope`

        []{#close()}

        -   #### close

            ``` methodSignature
            public void close()
            ```

            ::: block
            Hashes the container iff non-empty (i.e. if any element gets
            hashed during this scope).
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `Scope`
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
-   [Field](#field.summary) \| 
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

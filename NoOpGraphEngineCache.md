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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.graph.transformation.impl](package-summary.html)
:::

## Class NoOpGraphEngineCache\<Key extends [ComputeKey](../model/ComputeKey.html "interface in com.facebook.buck.core.graph.transformation.model")\<Value\>,​Value extends [ComputeResult](../model/ComputeResult.html "interface in com.facebook.buck.core.graph.transformation.model")\> {#class-noopgraphenginecachekey-extends-computekeyvaluevalue-extends-computeresult .title title="Class NoOpGraphEngineCache"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.graph.transformation.impl.NoOpGraphEngineCache\<Key,​Value\>

::: description
-   

    All Implemented Interfaces:
    :   `GraphEngineCache<Key,​Value>`

    ------------------------------------------------------------------------

        public class NoOpGraphEngineCache<Key extends ComputeKey<Value>,​Value extends ComputeResult>
        extends Object
        implements GraphEngineCache<Key,​Value>

    ::: block
    Graph Engine cache that does not store result, and always returns
    nothing on get. Can be used for testing or fast transformations that
    do not benefit from caching intermediate data.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                Description
          -------------------------- -------------
          `NoOpGraphEngineCache()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Optional<Value>`     | `get​(Key key)`        | ::: block             |
        |                       |                       | Optionally returns    |
        |                       |                       | the cached result     |
        |                       |                       | given the key         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `put​(Key              | ::: block             |
        |                       | key,    Value value)` | Offers the given key  |
        |                       |                       | and value for caching |
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### NoOpGraphEngineCache

                public NoOpGraphEngineCache()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#get(com.facebook.buck.core.graph.transformation.model.ComputeKey)}
        []{#get(Key)}

        -   #### get

            ``` methodSignature
            public Optional<Value> get​(Key key)
            ```

            ::: block
            [Description copied from
            interface: `GraphEngineCache`]{.descfrmTypeLabel}
            :::

            ::: block
            Optionally returns the cached result given the key
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `get` in
                interface `GraphEngineCache<Key extends ComputeKey<Value>,​Value extends ComputeResult>`

            [Parameters:]{.paramLabel}
            :   `key` - The desired key

            [Returns:]{.returnLabel}
            :   the result if cached, otherwise an empty Optional

        []{#put(com.facebook.buck.core.graph.transformation.model.ComputeKey,com.facebook.buck.core.graph.transformation.model.ComputeResult)}
        []{#put(Key,Value)}

        -   #### put

            ``` methodSignature
            public void put​(Key key,
                            Value value)
            ```

            ::: block
            [Description copied from
            interface: `GraphEngineCache`]{.descfrmTypeLabel}
            :::

            ::: block
            Offers the given key and value for caching
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `put` in
                interface `GraphEngineCache<Key extends ComputeKey<Value>,​Value extends ComputeResult>`

            [Parameters:]{.paramLabel}
            :   `key` - the key to cache
            :   `value` - the value to cache
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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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

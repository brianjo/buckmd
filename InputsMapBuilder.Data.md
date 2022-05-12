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
[Package]{.packageLabelInType} [com.facebook.buck.rules.modern.impl](package-summary.html)
:::

## Class InputsMapBuilder.Data {#class-inputsmapbuilder.data .title title="Class InputsMapBuilder.Data"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.modern.impl.InputsMapBuilder.Data

::: description
-   

    Enclosing class:
    :   [InputsMapBuilder](InputsMapBuilder.html "class in com.facebook.buck.rules.modern.impl")

    ------------------------------------------------------------------------

        public static class InputsMapBuilder.Data
        extends Object

    ::: block
    Holds the information derived from a rulekey appendable. For a
    particular appendable, the same Data instance will always be
    returned.
    The Data objects form a projection of the rulekey appendable graph
    with edges into an object with no (directly or indirectly)
    referenced inputs removed.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                      Description
          ------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `Data​(com.google.common.collect.ImmutableList<SourcePath> paths,     com.google.common.collect.ImmutableList<InputsMapBuilder.Data> children)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                  Method                                                                          Description
          ------------------------------------------------------------------ ------------------------------------------------------------------------------- -------------
          `void`                                                             `forAllData​(java.util.function.Consumer<InputsMapBuilder.Data> dataConsumer)`    
          `com.google.common.collect.ImmutableList<InputsMapBuilder.Data>`   `getChildren()`                                                                  
          `com.google.common.collect.ImmutableList<SourcePath>`              `getPaths()`                                                                     

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

        []{#<init>(com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableList)}

        -   #### Data

                public Data​(com.google.common.collect.ImmutableList<SourcePath> paths,
                            com.google.common.collect.ImmutableList<InputsMapBuilder.Data> children)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getPaths()}

        -   #### getPaths

            ``` methodSignature
            public com.google.common.collect.ImmutableList<SourcePath> getPaths()
            ```

        []{#getChildren()}

        -   #### getChildren

            ``` methodSignature
            public com.google.common.collect.ImmutableList<InputsMapBuilder.Data> getChildren()
            ```

        []{#forAllData(java.util.function.Consumer)}

        -   #### forAllData

            ``` methodSignature
            public void forAllData​(java.util.function.Consumer<InputsMapBuilder.Data> dataConsumer)
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

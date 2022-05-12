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
[Package]{.packageLabelInType} [com.facebook.buck.features.python](package-summary.html)
:::

## Class PythonMappedComponents.Resolved {#class-pythonmappedcomponents.resolved .title title="Class PythonMappedComponents.Resolved"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.python.PythonMappedComponents.Resolved

::: description
-   

    All Implemented Interfaces:
    :   `PythonComponents.Resolved`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [PythonMappedComponents](PythonMappedComponents.html "class in com.facebook.buck.features.python")

    ------------------------------------------------------------------------

        public static class PythonMappedComponents.Resolved
        extends Object
        implements PythonComponents.Resolved

    ::: block
    An implementation of
    [`PythonComponents.Resolved`](PythonComponents.Resolved.html "interface in com.facebook.buck.features.python")
    for
    [`PythonMappedComponents`](PythonMappedComponents.html "class in com.facebook.buck.features.python")
    with
    [`SourcePath`](../../core/sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")s
    resolved to
    [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}s
    for use with
    [`Step`](../../step/Step.html "interface in com.facebook.buck.step").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.features.python.PythonComponents.Resolved}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.features.python.[PythonComponents.Resolved](PythonComponents.Resolved.html "interface in com.facebook.buck.features.python")

            `PythonComponents.Resolved.ComponentConsumer`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                              Description
          ------------------------------------------------------------------------ -------------
          `Resolved​(com.google.common.collect.ImmutableMap<Path,​Path> resolved)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `forEachPythonC       | ::: block             |
        |                       | omponent​(PythonCompon | Called by executing   |
        |                       | ents.Resolved.Compone | [`Step                |
        |                       | ntConsumer consumer)` | `](../../step/Step.ht |
        |                       |                       | ml "interface in com. |
        |                       |                       | facebook.buck.step")s |
        |                       |                       | to iterate over the   |
        |                       |                       | components owned by   |
        |                       |                       | this                  |
        |                       |                       | [`PythonC             |
        |                       |                       | omponents`](PythonCom |
        |                       |                       | ponents.html "interfa |
        |                       |                       | ce in com.facebook.bu |
        |                       |                       | ck.features.python"). |
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

        []{#<init>(com.google.common.collect.ImmutableMap)}

        -   #### Resolved

                public Resolved​(com.google.common.collect.ImmutableMap<Path,​Path> resolved)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#forEachPythonComponent(com.facebook.buck.features.python.PythonComponents.Resolved.ComponentConsumer)}

        -   #### forEachPythonComponent

            ``` methodSignature
            public void forEachPythonComponent​(PythonComponents.Resolved.ComponentConsumer consumer)
                                        throws IOException
            ```

            ::: block
            [Description copied from
            interface: `PythonComponents.Resolved`]{.descfrmTypeLabel}
            :::

            ::: block
            Called by executing
            [`Step`](../../step/Step.html "interface in com.facebook.buck.step")s
            to iterate over the components owned by this
            [`PythonComponents`](PythonComponents.html "interface in com.facebook.buck.features.python").
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `forEachPythonComponent` in
                interface `PythonComponents.Resolved`

            [Throws:]{.throwsLabel}
            :   `IOException`
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

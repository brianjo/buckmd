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
[Package]{.packageLabelInType} [com.facebook.buck.rules.modern.builders](package-summary.html)
:::

## Class IsolatedBuildableBuilder {#class-isolatedbuildablebuilder .title title="Class IsolatedBuildableBuilder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.modern.builders.IsolatedBuildableBuilder

::: description
-   

    ------------------------------------------------------------------------

        public abstract class IsolatedBuildableBuilder
        extends Object

    ::: block
    IsolatedBuildableBuilder is used to build rules in isolation. Users
    need to construct a working directory with all the required inputs
    (including .buckconfig files for each cell). The data for
    deserializing build rules is expected to be contained in the
    \"\_\_data\_\_\" directory under the root (see getProvider() below
    for the expected layout of this directory).
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `bu                   | ::: block             |
        |                       | ild​(com.google.common | Deserializes the      |
        |                       | .hash.HashCode hash)` | BuildableAndTarget    |
        |                       |                       | corresponding to hash |
        |                       |                       | and builds it.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `protec               | `createConsole()`     |                       |
        | ted abstract Console` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected a          | `createEvent          |                       |
        | bstract BuckEventBus` | Bus​(Console console)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
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
    -   []{#method.detail}

        ### Method Detail

        []{#createConsole()}

        -   #### createConsole

            ``` methodSignature
            protected abstract Console createConsole()
            ```

        []{#createEventBus(com.facebook.buck.util.Console)}

        -   #### createEventBus

            ``` methodSignature
            protected abstract BuckEventBus createEventBus​(Console console)
            ```

        []{#build(com.google.common.hash.HashCode)}

        -   #### build

            ``` methodSignature
            public void build​(com.google.common.hash.HashCode hash)
                       throws IOException,
                              StepFailedException,
                              InterruptedException
            ```

            ::: block
            Deserializes the BuildableAndTarget corresponding to hash
            and builds it.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`
            :   `StepFailedException`
            :   `InterruptedException`
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

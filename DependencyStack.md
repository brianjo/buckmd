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
[Package]{.packageLabelInType} [com.facebook.buck.core.exceptions](package-summary.html)
:::

## Class DependencyStack {#class-dependencystack .title title="Class DependencyStack"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.exceptions.DependencyStack

::: description
-   

    ------------------------------------------------------------------------

        public final class DependencyStack
        extends Object

    ::: block
    Stack-trace for providing better diagnostics when working with
    dependency graph.
    This type must not be used for anything except for providing error
    diagnostics.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static interface `   | `Dep                  | ::: block             |
        |                       | endencyStack.Element` | Marker interface for  |
        |                       |                       | stack trace elements. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static interface `   | `DependencyS          | ::: block             |
        |                       | tack.ProvidesElement` | Types which have      |
        |                       |                       | something to be       |
        |                       |                       | stored in stack trace |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `DependencyStack`     | `child​(Dependency     | ::: block             |
        |                       | Stack.Element where)` | Cons                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `DependencyStack`     | `child​(String where)` | ::: block             |
        |                       |                       | Cons                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `collect()`           | ::: block             |
        | ogle.common.collect.I |                       | Collect the stack     |
        | mmutableList<Object>` |                       | elements, top first   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `collectStringsF      | ::: block             |
        | ogle.common.collect.I | ilterAdjacentDupes()` | Collect the stack     |
        | mmutableList<String>` |                       | elements, top first,  |
        |                       |                       | converting all        |
        |                       |                       | elements to strings,  |
        |                       |                       | and filtering out     |
        |                       |                       | adjacent duplicates.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `equals​(Object o)`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isEmpty()`           | ::: block             |
        |                       |                       | Check if stack is     |
        |                       |                       | empty                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `root()`              | ::: block             |
        | atic DependencyStack` |                       | Create an empty stack |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `top​(Dependen         | ::: block             |
        | atic DependencyStack` | cyStack.Element top)` | Create a single       |
        |                       |                       | element stack         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `top​(String top)`     | ::: block             |
        | atic DependencyStack` |                       | Create a single       |
        |                       |                       | element stack         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#root()}

        -   #### root

            ``` methodSignature
            public static DependencyStack root()
            ```

            ::: block
            Create an empty stack
            :::

        []{#top(com.facebook.buck.core.exceptions.DependencyStack.Element)}

        -   #### top

            ``` methodSignature
            public static DependencyStack top​(DependencyStack.Element top)
            ```

            ::: block
            Create a single element stack
            :::

        []{#top(java.lang.String)}

        -   #### top

            ``` methodSignature
            public static DependencyStack top​(String top)
            ```

            ::: block
            Create a single element stack
            :::

        []{#child(com.facebook.buck.core.exceptions.DependencyStack.Element)}

        -   #### child

            ``` methodSignature
            public DependencyStack child​(DependencyStack.Element where)
            ```

            ::: block
            Cons
            :::

        []{#child(java.lang.String)}

        -   #### child

            ``` methodSignature
            public DependencyStack child​(String where)
            ```

            ::: block
            Cons
            :::

        []{#isEmpty()}

        -   #### isEmpty

            ``` methodSignature
            public boolean isEmpty()
            ```

            ::: block
            Check if stack is empty
            :::

        []{#collect()}

        -   #### collect

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Object> collect()
            ```

            ::: block
            Collect the stack elements, top first
            :::

        []{#collectStringsFilterAdjacentDupes()}

        -   #### collectStringsFilterAdjacentDupes

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> collectStringsFilterAdjacentDupes()
            ```

            ::: block
            Collect the stack elements, top first, converting all
            elements to strings, and filtering out adjacent duplicates.
            :::

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(Object o)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `Object`

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `Object`

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`
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

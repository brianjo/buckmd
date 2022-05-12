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
[Package]{.packageLabelInType} [com.facebook.buck.features.project.intellij](package-summary.html)
:::

## Class IjDependencyListBuilder {#class-ijdependencylistbuilder .title title="Class IjDependencyListBuilder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.project.intellij.IjDependencyListBuilder

::: description
-   

    ------------------------------------------------------------------------

        public class IjDependencyListBuilder
        extends Object

    ::: block
    Represents the dependencies of an `IjModule` in a form intended to
    be consumable by the
    [`IjProjectWriter`](IjProjectWriter.html "class in com.facebook.buck.features.project.intellij").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `IjDependencyListBui  | ::: block             |
        |                       | lder.DependencyEntry` | The design of this    |
        |                       |                       | classes API is tied   |
        |                       |                       | to how the            |
        |                       |                       | corresponding         |
        |                       |                       | StringTemplate        |
        |                       |                       | template interacts    |
        |                       |                       | with it.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `IjDepende            | ::: block             |
        |                       | ncyListBuilder.Scope` | Set of scopes         |
        |                       |                       | supported by IntelliJ |
        |                       |                       | for the               |
        |                       |                       | \"orderEntry\"        |
        |                       |                       | element.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `IjDependencyL        |                       |
        |                       | istBuilder.SortOrder` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `IjDepend             | ::: block             |
        |                       | encyListBuilder.Type` | Set of types          |
        |                       |                       | supported by IntelliJ |
        |                       |                       | for the               |
        |                       |                       | \"orderEntry\"        |
        |                       |                       | element.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                   Description
          ----------------------------- -------------
          `IjDependencyListBuilder()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                                   Method                                                                                                 Description
          ----------------------------------------------------------------------------------- ------------------------------------------------------------------------------------------------------ -------------
          `void`                                                                              `addCompiledShadow​(String name)`                                                                        
          `void`                                                                              `addLibrary​(String name,           IjDependencyListBuilder.Scope scope,           boolean exported)`    
          `void`                                                                              `addModule​(String name,          IjDependencyListBuilder.Scope scope,          boolean exported)`       
          `com.google.common.collect.ImmutableSet<IjDependencyListBuilder.DependencyEntry>`   `build()`                                                                                               

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

        -   #### IjDependencyListBuilder

                public IjDependencyListBuilder()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#addModule(java.lang.String,com.facebook.buck.features.project.intellij.IjDependencyListBuilder.Scope,boolean)}

        -   #### addModule

            ``` methodSignature
            public void addModule​(String name,
                                  IjDependencyListBuilder.Scope scope,
                                  boolean exported)
            ```

        []{#addCompiledShadow(java.lang.String)}

        -   #### addCompiledShadow

            ``` methodSignature
            public void addCompiledShadow​(String name)
            ```

        []{#addLibrary(java.lang.String,com.facebook.buck.features.project.intellij.IjDependencyListBuilder.Scope,boolean)}

        -   #### addLibrary

            ``` methodSignature
            public void addLibrary​(String name,
                                   IjDependencyListBuilder.Scope scope,
                                   boolean exported)
            ```

        []{#build()}

        -   #### build

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<IjDependencyListBuilder.DependencyEntry> build()
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

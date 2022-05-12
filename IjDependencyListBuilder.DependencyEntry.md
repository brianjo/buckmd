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
[Package]{.packageLabelInType} [com.facebook.buck.features.project.intellij](package-summary.html)
:::

## Class IjDependencyListBuilder.DependencyEntry {#class-ijdependencylistbuilder.dependencyentry .title title="Class IjDependencyListBuilder.DependencyEntry"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.project.intellij.IjDependencyListBuilder.DependencyEntry

::: description
-   

    All Implemented Interfaces:
    :   `Comparable<IjDependencyListBuilder.DependencyEntry>`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [IjDependencyListBuilder](IjDependencyListBuilder.html "class in com.facebook.buck.features.project.intellij")

    ------------------------------------------------------------------------

        public abstract static class IjDependencyListBuilder.DependencyEntry
        extends Object
        implements Comparable<IjDependencyListBuilder.DependencyEntry>

    ::: block
    The design of this classes API is tied to how the corresponding
    StringTemplate template interacts with it.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor           Description
          --------------------- -------------
          `DependencyEntry()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                                                              Method                                                   Description
          -------------------------------------------------------------------------------------------------------------- -------------------------------------------------------- -------------
          `int`                                                                                                          `compareTo​(IjDependencyListBuilder.DependencyEntry o)`    
          `protected void`                                                                                               `dataOnlyAbsentForSourceFolder()`                         
          `abstract Optional<com.facebook.buck.features.project.intellij.IjDependencyListBuilder.DependencyEntryData>`   `getData()`                                               
          `com.facebook.buck.features.project.intellij.IjDependencyListBuilder.DependencyEntryData`                      `getLibrary()`                                            
          `com.facebook.buck.features.project.intellij.IjDependencyListBuilder.DependencyEntryData`                      `getModule()`                                             
          `abstract IjDependencyListBuilder.SortOrder`                                                                   `getSortOrder()`                                          
          `abstract IjDependencyListBuilder.Type`                                                                        `getType()`                                               

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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### DependencyEntry

                public DependencyEntry()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getType()}

        -   #### getType

            ``` methodSignature
            public abstract IjDependencyListBuilder.Type getType()
            ```

        []{#getSortOrder()}

        -   #### getSortOrder

            ``` methodSignature
            public abstract IjDependencyListBuilder.SortOrder getSortOrder()
            ```

        []{#getData()}

        -   #### getData

            ``` methodSignature
            public abstract Optional<com.facebook.buck.features.project.intellij.IjDependencyListBuilder.DependencyEntryData> getData()
            ```

        []{#getModule()}

        -   #### getModule

            ``` methodSignature
            @Nullable
            public com.facebook.buck.features.project.intellij.IjDependencyListBuilder.DependencyEntryData getModule()
            ```

        []{#getLibrary()}

        -   #### getLibrary

            ``` methodSignature
            @Nullable
            public com.facebook.buck.features.project.intellij.IjDependencyListBuilder.DependencyEntryData getLibrary()
            ```

        []{#dataOnlyAbsentForSourceFolder()}

        -   #### dataOnlyAbsentForSourceFolder

            ``` methodSignature
            @Check
            protected void dataOnlyAbsentForSourceFolder()
            ```

        []{#compareTo(com.facebook.buck.features.project.intellij.IjDependencyListBuilder.DependencyEntry)}

        -   #### compareTo

            ``` methodSignature
            public int compareTo​(IjDependencyListBuilder.DependencyEntry o)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `compareTo` in
                interface `Comparable<IjDependencyListBuilder.DependencyEntry>`
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

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
[Package]{.packageLabelInType} [com.facebook.buck.io.file](package-summary.html)
:::

## Class LazyPath {#class-lazypath .title title="Class LazyPath"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.io.file.LazyPath

::: description
-   

    ------------------------------------------------------------------------

        public abstract class LazyPath
        extends Object

    ::: block
    Class is intended to provide Paths to be used by cache
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor    Description
          -------------- -------------
          `LazyPath()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `pro                  | `create()`            |                       |
        | tected abstract Path` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `get()`               | ::: block             |
        |                       |                       | On first access it    |
        |                       |                       | will invoke the given |
        |                       |                       | supplier to obtain    |
        |                       |                       | the value of the      |
        |                       |                       | Path.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getUnchecked()`      | ::: block             |
        |                       |                       | Does not invoke the   |
        |                       |                       | path supplier,        |
        |                       |                       | assuming it was       |
        |                       |                       | invoked previously.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static LazyPath`     | `o                    | ::: block             |
        |                       | fInstance​(Path path)` | Creates an instance   |
        |                       |                       | with given path.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### LazyPath

                public LazyPath()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#ofInstance(java.nio.file.Path)}

        -   #### ofInstance

            ``` methodSignature
            public static LazyPath ofInstance​(Path path)
            ```

            ::: block
            Creates an instance with given path.
            :::

            [Parameters:]{.paramLabel}
            :   `path` - The path that get()/getUnchecked() methods
                should return.

            [Returns:]{.returnLabel}
            :   Instance that always returns the given path. It means
                there is no laziness.

        []{#get()}

        -   #### get

            ``` methodSignature
            public final Path get()
                           throws IOException
            ```

            ::: block
            On first access it will invoke the given supplier to obtain
            the value of the Path.
            :::

            [Returns:]{.returnLabel}
            :   Memoized path.

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getUnchecked()}

        -   #### getUnchecked

            ``` methodSignature
            public Path getUnchecked()
            ```

            ::: block
            Does not invoke the path supplier, assuming it was invoked
            previously.
            :::

            [Returns:]{.returnLabel}
            :   Memoized path.

        []{#create()}

        -   #### create

            ``` methodSignature
            protected abstract Path create()
                                    throws IOException
            ```

            [Returns:]{.returnLabel}
            :   Path that will be created lazily and memoized.

            [Throws:]{.throwsLabel}
            :   `IOException`

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

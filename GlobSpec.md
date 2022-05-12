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
[Package]{.packageLabelInType} [com.facebook.buck.skylark.io](package-summary.html)
:::

## Class GlobSpec {#class-globspec .title title="Class GlobSpec"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.skylark.io.GlobSpec

::: description
-   

    ------------------------------------------------------------------------

        public abstract class GlobSpec
        extends Object

    ::: block
    Glob specification includes parameters that affect glob evaluation
    within a single package.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor    Description
          -------------- -------------
          `GlobSpec()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `abstrac              | `getExclude()`        | ::: block             |
        | t Collection<String>` |                       | Wildcards of paths    |
        |                       |                       | that should be        |
        |                       |                       | skipped from the glob |
        |                       |                       | expansion.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract boolean`    | `get                  | ::: block             |
        |                       | ExcludeDirectories()` | Whether directories   |
        |                       |                       | should be excluded    |
        |                       |                       | from the glob         |
        |                       |                       | expansion.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstrac              | `getInclude()`        | ::: block             |
        | t Collection<String>` |                       | Wildcards of paths    |
        |                       |                       | that should be        |
        |                       |                       | returned.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static GlobSpec`     | `of​(Coll              |                       |
        |                       | ection<String> includ |                       |
        |                       | e,   Collection<Strin |                       |
        |                       | g> exclude,   boolean |                       |
        |                       |  excludeDirectories)` |                       |
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

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### GlobSpec

                public GlobSpec()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getInclude()}

        -   #### getInclude

            ``` methodSignature
            public abstract Collection<String> getInclude()
            ```

            ::: block
            Wildcards of paths that should be returned.
            :::

        []{#getExclude()}

        -   #### getExclude

            ``` methodSignature
            public abstract Collection<String> getExclude()
            ```

            ::: block
            Wildcards of paths that should be skipped from the glob
            expansion.
            :::

        []{#getExcludeDirectories()}

        -   #### getExcludeDirectories

            ``` methodSignature
            public abstract boolean getExcludeDirectories()
            ```

            ::: block
            Whether directories should be excluded from the glob
            expansion.
            :::

        []{#of(java.util.Collection,java.util.Collection,boolean)}

        -   #### of

            ``` methodSignature
            public static GlobSpec of​(Collection<String> include,
                                      Collection<String> exclude,
                                      boolean excludeDirectories)
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

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
[Package]{.packageLabelInType} [com.facebook.buck.cxx.toolchain](package-summary.html)
:::

## Class CxxToolTypeInferer {#class-cxxtooltypeinferer .title title="Class CxxToolTypeInferer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.toolchain.CxxToolTypeInferer

::: description
-   

    ------------------------------------------------------------------------

        public class CxxToolTypeInferer
        extends Object

    ::: block
    Utilities for inferring the
    [`CxxToolProvider.Type`](CxxToolProvider.Type.html "enum in com.facebook.buck.cxx.toolchain")
    of a cxx tool.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor              Description
          ------------------------ -------------
          `CxxToolTypeInferer()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static               | `getTypeFromPath​(     | ::: block             |
        | CxxToolProvider.Type` | PathSourcePath path)` | Invokes the tool with |
        |                       |                       | \`\--version\` and    |
        |                       |                       | parses the output to  |
        |                       |                       | determine the type of |
        |                       |                       | the compiler.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `protected static     | `getType              | ::: block             |
        | CxxToolProvider.Type` | FromVersionOutput​(Ite | Checks if the output  |
        |                       | rable<String> lines)` | looks like \`clang    |
        |                       |                       | \--version\`\'s       |
        |                       |                       | output.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
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

        -   #### CxxToolTypeInferer

                public CxxToolTypeInferer()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getTypeFromPath(com.facebook.buck.core.sourcepath.PathSourcePath)}

        -   #### getTypeFromPath

            ``` methodSignature
            public static CxxToolProvider.Type getTypeFromPath​(PathSourcePath path)
            ```

            ::: block
            Invokes the tool with \`\--version\` and parses the output
            to determine the type of the compiler.
            :::

        []{#getTypeFromVersionOutput(java.lang.Iterable)}

        -   #### getTypeFromVersionOutput

            ``` methodSignature
            protected static CxxToolProvider.Type getTypeFromVersionOutput​(Iterable<String> lines)
            ```

            ::: block
            Checks if the output looks like \`clang \--version\`\'s
            output.
            :::
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

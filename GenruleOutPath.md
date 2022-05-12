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
[Package]{.packageLabelInType} [com.facebook.buck.core.path](package-summary.html)
:::

## Class GenruleOutPath {#class-genruleoutpath .title title="Class GenruleOutPath"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.path.GenruleOutPath

::: description
-   

    ------------------------------------------------------------------------

        public class GenruleOutPath
        extends Object

    ::: block
    Class to store paths which are in out/outs argument of genrule.
    Checks if the paths are forward, relative, non empty and simple.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static void`         | `a                    | ::: block             |
        |                       | ssertValid​(String s)` | Don\'t allow empty    |
        |                       |                       | paths, absolute       |
        |                       |                       | paths, paths ending   |
        |                       |                       | with / or paths       |
        |                       |                       | containing            |
        |                       |                       | \".\"/\"..\" Only     |
        |                       |                       | exception is when out |
        |                       |                       | = \".\"               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `s                    | `of​(String s)`        | ::: block             |
        | tatic GenruleOutPath` |                       | Creates a GenruleOut  |
        |                       |                       | object from a string. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `stringMapp           |                       |
        |                       | er​(GenruleOutPath p)` |                       |
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

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#of(java.lang.String)}

        -   #### of

            ``` methodSignature
            public static GenruleOutPath of​(String s)
            ```

            ::: block
            Creates a GenruleOut object from a string. Uses assertValid
            to verify and returns a HumanReadableException.
            :::

        []{#assertValid(java.lang.String)}

        -   #### assertValid

            ``` methodSignature
            public static void assertValid​(String s)
            ```

            ::: block
            Don\'t allow empty paths, absolute paths, paths ending with
            / or paths containing \".\"/\"..\" Only exception is when
            out = \".\"
            :::

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

        []{#stringMapper(com.facebook.buck.core.path.GenruleOutPath)}

        -   #### stringMapper

            ``` methodSignature
            public static String stringMapper​(GenruleOutPath p)
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

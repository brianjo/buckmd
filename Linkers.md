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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.cxx.toolchain.linker.impl](package-summary.html)
:::

## Class Linkers {#class-linkers .title title="Class Linkers"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.toolchain.linker.impl.Linkers

::: description
-   

    ------------------------------------------------------------------------

        public class Linkers
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `sta                  | `iXlinker​(It          | ::: block             |
        | tic Iterable<String>` | erable<String> args)` | Prefixes each of the  |
        |                       |                       | given linker          |
        |                       |                       | arguments with        |
        |                       |                       | \"-Xlinker\" so that  |
        |                       |                       | the compiler linker   |
        |                       |                       | driver will pass      |
        |                       |                       | these arguments       |
        |                       |                       | directly down to the  |
        |                       |                       | linker rather than    |
        |                       |                       | interpreting them     |
        |                       |                       | itself.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `iXli                 |                       |
        | tic Iterable<String>` | nker​(String... args)` |                       |
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
    -   []{#method.detail}

        ### Method Detail

        []{#iXlinker(java.lang.Iterable)}

        -   #### iXlinker

            ``` methodSignature
            public static Iterable<String> iXlinker​(Iterable<String> args)
            ```

            ::: block
            Prefixes each of the given linker arguments with
            \"-Xlinker\" so that the compiler linker driver will pass
            these arguments directly down to the linker rather than
            interpreting them itself.
            e.g. \[\"-rpath\", \"hello/world\"\] -\> \[\"-Xlinker\",
            \"-rpath\", \"-Xlinker\", \"hello/world\"\]

            Arguments that do not contain commas can instead be passed
            using the shorter \"-Wl,ARGUMENT\" form.

            e.g., \[\"-rpath\", \"hello/world\"\] -\> \[\"-Wl,-rpath\",
            \"-Wl,hello/world\" \]
            :::

            [Parameters:]{.paramLabel}
            :   `args` - arguments for the linker.

            [Returns:]{.returnLabel}
            :   arguments to be passed to the compiler linker driver.

        []{#iXlinker(java.lang.String...)}

        -   #### iXlinker

            ``` methodSignature
            public static Iterable<String> iXlinker​(String... args)
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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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

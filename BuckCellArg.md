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
[Package]{.packageLabelInType} [com.facebook.buck.support.cli.args](package-summary.html)
:::

## Class BuckCellArg {#class-buckcellarg .title title="Class BuckCellArg"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.support.cli.args.BuckCellArg

::: description
-   

    ------------------------------------------------------------------------

        public abstract class BuckCellArg
        extends Object

    ::: block
    Helps parse common command line argument formats
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor       Description
          ----------------- -------------
          `BuckCellArg()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `abstract String`     | `getArg()`            |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getBasePath()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstr                | `getCellName()`       |                       |
        | act Optional<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static BuckCellArg`  | `of​(String input)`    | ::: block             |
        |                       |                       | Convenience           |
        |                       |                       | constructor for an    |
        |                       |                       | [`BuckCellArg`](      |
        |                       |                       | BuckCellArg.html "cla |
        |                       |                       | ss in com.facebook.bu |
        |                       |                       | ck.support.cli.args") |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static BuckCellArg`  | `of                   |                       |
        |                       | ​(Optional<String> cel |                       |
        |                       | lName,   String arg)` |                       |
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

        -   #### BuckCellArg

                public BuckCellArg()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getCellName()}

        -   #### getCellName

            ``` methodSignature
            public abstract Optional<String> getCellName()
            ```

        []{#getArg()}

        -   #### getArg

            ``` methodSignature
            public abstract String getArg()
            ```

        []{#getBasePath()}

        -   #### getBasePath

            ``` methodSignature
            @Derived
            public String getBasePath()
            ```

        []{#of(java.lang.String)}

        -   #### of

            ``` methodSignature
            public static BuckCellArg of​(String input)
            ```

            ::: block
            Convenience constructor for an
            [`BuckCellArg`](BuckCellArg.html "class in com.facebook.buck.support.cli.args")
            :::

        []{#of(java.util.Optional,java.lang.String)}

        -   #### of

            ``` methodSignature
            public static BuckCellArg of​(Optional<String> cellName,
                                         String arg)
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

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
[Package]{.packageLabelInType} [com.facebook.buck.core.macros](package-summary.html)
:::

## Class StringMacroCombiner {#class-stringmacrocombiner .title title="Class StringMacroCombiner"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.macros.StringMacroCombiner

::: description
-   

    All Implemented Interfaces:
    :   `MacroCombiner<String>`

    ------------------------------------------------------------------------

        public class StringMacroCombiner
        extends Object
        implements MacroCombiner<String>

    ::: block
    A simple MacroCombiner for `MacroReplacer<String>` that just
    concatenates the strings and expanded macros.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor               Description
          ------------------------- -------------
          `StringMacroCombiner()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `add​(S                | ::: block             |
        |                       | tring expandedMacro)` | Add the expanded form |
        |                       |                       | of a macro.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `ad                   | ::: block             |
        |                       | dString​(String part)` | Add a non-macro       |
        |                       |                       | containing substring. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `build()`             | ::: block             |
        |                       |                       | Returns the combined  |
        |                       |                       | result.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

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

        -   #### StringMacroCombiner

                public StringMacroCombiner()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#build()}

        -   #### build

            ``` methodSignature
            public String build()
            ```

            ::: block
            [Description copied from
            interface: `MacroCombiner`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns the combined result.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `build` in interface `MacroCombiner<String>`

        []{#addString(java.lang.String)}

        -   #### addString

            ``` methodSignature
            public void addString​(String part)
            ```

            ::: block
            [Description copied from
            interface: `MacroCombiner`]{.descfrmTypeLabel}
            :::

            ::: block
            Add a non-macro containing substring.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `addString` in interface `MacroCombiner<String>`

        []{#add(java.lang.String)}

        -   #### add

            ``` methodSignature
            public void add​(String expandedMacro)
            ```

            ::: block
            [Description copied from
            interface: `MacroCombiner`]{.descfrmTypeLabel}
            :::

            ::: block
            Add the expanded form of a macro.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `add` in interface `MacroCombiner<String>`
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

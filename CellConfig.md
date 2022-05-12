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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.core.cell](package-summary.html)
:::

## Class CellConfig {#class-cellconfig .title title="Class CellConfig"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.cell.CellConfig

::: description
-   

    ------------------------------------------------------------------------

        public abstract class CellConfig
        extends Object

    ::: block
    Hierarcical configuration of cell/section/key/value quadruples.
    This class only implements the simple construction/storage/retrieval
    of these values. Other classes like
    [`Config`](../../util/config/Config.html "class in com.facebook.buck.util.config")
    implements accessors that interpret the values as other types.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `CellConfig.Builder`  | ::: block             |
        |                       |                       | A builder for         |
        |                       |                       | [`CellCon             |
        |                       |                       | fig`](CellConfig.html |
        |                       |                       |  "class in com.facebo |
        |                       |                       | ok.buck.core.cell")s. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type     Field              Description
          --------------------- ------------------ -------------
          `static CellConfig`   `EMPTY_INSTANCE`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor      Description
          ---------------- -------------
          `CellConfig()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `stati                | `builder()`           |                       |
        | c CellConfig.Builder` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `RawConfig`           | `getForCel            | ::: block             |
        |                       | l​(CellName cellName)` | Retrieve the          |
        |                       |                       | Cell-view of the raw  |
        |                       |                       | config.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getOv                | ::: block             |
        | n.collect.ImmutableMa | erridesByPath​(com.goo | Translates the \'cell |
        | p<AbsPath,​RawConfig>` | gle.common.collect.Im | name\'-\>override map |
        |                       | mutableMap<CellName,​A | into a                |
        |                       | bsPath> pathMapping)` | \'Path\'-\>override   |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstr                | `getValues()`         |                       |
        | act com.google.common |                       |                       |
        | .collect.ImmutableMap |                       |                       |
        | <CellName,​RawConfig>` |                       |                       |
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
    -   []{#field.detail}

        ### Field Detail

        []{#EMPTY_INSTANCE}

        -   #### EMPTY_INSTANCE

                public static final CellConfig EMPTY_INSTANCE
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### CellConfig

                public CellConfig()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getValues()}

        -   #### getValues

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableMap<CellName,​RawConfig> getValues()
            ```

        []{#getForCell(com.facebook.buck.core.cell.CellName)}

        -   #### getForCell

            ``` methodSignature
            public RawConfig getForCell​(CellName cellName)
            ```

            ::: block
            Retrieve the Cell-view of the raw config.
            :::

            [Returns:]{.returnLabel}
            :   The contents of the raw config with the cell-view filter

        []{#getOverridesByPath(com.google.common.collect.ImmutableMap)}

        -   #### getOverridesByPath

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<AbsPath,​RawConfig> getOverridesByPath​(com.google.common.collect.ImmutableMap<CellName,​AbsPath> pathMapping)
                                                                                               throws InvalidCellOverrideException
            ```

            ::: block
            Translates the \'cell name\'-\>override map into a
            \'Path\'-\>override map.
            :::

            [Parameters:]{.paramLabel}
            :   `pathMapping` - a map containing paths to all of the
                cells we want to query.

            [Returns:]{.returnLabel}
            :   \'Path\'-\>override map

            [Throws:]{.throwsLabel}
            :   `InvalidCellOverrideException`

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static CellConfig.Builder builder()
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
-   [Nested](#nested.class.summary) \| 
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

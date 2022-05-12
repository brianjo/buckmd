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
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.core.model](package-summary.html)
:::

## Class UnconfiguredTargetConfiguration {#class-unconfiguredtargetconfiguration .title title="Class UnconfiguredTargetConfiguration"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.model.TargetConfiguration](TargetConfiguration.html "class in com.facebook.buck.core.model")

    -   -   com.facebook.buck.core.model.UnconfiguredTargetConfiguration

::: description
-   

    All Implemented Interfaces:
    :   `Comparable<TargetConfiguration>`

    ------------------------------------------------------------------------

        public class UnconfiguredTargetConfiguration
        extends TargetConfiguration

    ::: block
    Configuration that resolves to unconfigured platform, which results
    in error on any operations with platforms (like `compatible_with` or
    `select()`
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                          Field        Description
          ------------------------------------------ ------------ -------------
          `static UnconfiguredTargetConfiguration`   `INSTANCE`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `boolean`             | `equals​(Object obj)`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `O                    | `getC                 |                       |
        | ptional<BuildTarget>` | onfigurationTarget()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          | ::: block             |
        |                       |                       | Build target for rule |
        |                       |                       | based build target or |
        |                       |                       | class name otherwise. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.model.TargetConfiguration}

            ### Methods inherited from class com.facebook.buck.core.model.[TargetConfiguration](TargetConfiguration.html "class in com.facebook.buck.core.model")

            `compareTo`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#INSTANCE}

        -   #### INSTANCE

                public static final UnconfiguredTargetConfiguration INSTANCE
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `Object`

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(Object obj)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `Object`

        []{#getConfigurationTarget()}

        -   #### getConfigurationTarget

            ``` methodSignature
            public Optional<BuildTarget> getConfigurationTarget()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getConfigurationTarget` in class `TargetConfiguration`

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            ::: block
            [Description copied from
            class: `TargetConfiguration`]{.descfrmTypeLabel}
            :::

            ::: block
            Build target for rule based build target or class name
            otherwise.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `toString` in class `TargetConfiguration`
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
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
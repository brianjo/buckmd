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
[Package]{.packageLabelInType} [com.facebook.buck.rules.macros](package-summary.html)
:::

## Class LocationMacro {#class-locationmacro .title title="Class LocationMacro"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.rules.macros.BuildTargetMacro](BuildTargetMacro.html "class in com.facebook.buck.rules.macros")

    -   -   [com.facebook.buck.rules.macros.BaseLocationMacro](BaseLocationMacro.html "class in com.facebook.buck.rules.macros")

        -   -   com.facebook.buck.rules.macros.LocationMacro

::: description
-   

    All Implemented Interfaces:
    :   `Macro`, `TargetTranslatable<Macro>`

    ------------------------------------------------------------------------

        public abstract class LocationMacro
        extends BaseLocationMacro

    ::: block
    Macro that resolves to the output location of a build rule.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor         Description
          ------------------- -------------
          `LocationMacro()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Cl                   | `getMacroClass()`     |                       |
        | ass<? extends Macro>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `of​(Buil              | ::: block             |
        | static LocationMacro` | dTarget buildTarget)` | Shorthand for         |
        |                       |                       | constructing a        |
        |                       |                       | LocationMacro         |
        |                       |                       | referring to the main |
        |                       |                       | default output.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `of​(BuildTarge        |                       |
        | static LocationMacro` | tWithOutputs target)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `pro                  | `withTargetW          |                       |
        | tected LocationMacro` | ithOutputs​(BuildTarge |                       |
        |                       | tWithOutputs target)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.rules.macros.BuildTargetMacro}

            ### Methods inherited from class com.facebook.buck.rules.macros.[BuildTargetMacro](BuildTargetMacro.html "class in com.facebook.buck.rules.macros")

            `equals, getTarget, getTargetWithOutputs, hashCode, translateTargets`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### LocationMacro

                public LocationMacro()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getMacroClass()}

        -   #### getMacroClass

            ``` methodSignature
            public Class<? extends Macro> getMacroClass()
            ```

        []{#withTargetWithOutputs(com.facebook.buck.core.model.BuildTargetWithOutputs)}

        -   #### withTargetWithOutputs

            ``` methodSignature
            protected LocationMacro withTargetWithOutputs​(BuildTargetWithOutputs target)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `withTargetWithOutputs` in class `BuildTargetMacro`

            [Returns:]{.returnLabel}
            :   a copy of this
                [`BuildTargetMacro`](BuildTargetMacro.html "class in com.facebook.buck.rules.macros")
                with the given
                [`BuildTargetWithOutputs`](../../core/model/BuildTargetWithOutputs.html "class in com.facebook.buck.core.model").

        []{#of(com.facebook.buck.core.model.BuildTarget)}

        -   #### of

            ``` methodSignature
            public static LocationMacro of​(BuildTarget buildTarget)
            ```

            ::: block
            Shorthand for constructing a LocationMacro referring to the
            main default output.
            :::

        []{#of(com.facebook.buck.core.model.BuildTargetWithOutputs)}

        -   #### of

            ``` methodSignature
            public static LocationMacro of​(BuildTargetWithOutputs target)
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
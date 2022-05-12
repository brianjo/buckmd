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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.platform](package-summary.html)
:::

## Class ThrowingConstraintResolver {#class-throwingconstraintresolver .title title="Class ThrowingConstraintResolver"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.rules.platform.ThrowingConstraintResolver

::: description
-   

    All Implemented Interfaces:
    :   `ConstraintResolver`

    ------------------------------------------------------------------------

        public class ThrowingConstraintResolver
        extends Object
        implements ConstraintResolver

    ::: block
    Constraint resolver that always throws. Can be used in tests or in
    unconfigurable targets.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                      Description
          -------------------------------- -------------
          `ThrowingConstraintResolver()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `ConstraintSetting`   | `getConstraintSe      | ::: block             |
        |                       | tting​(BuildTarget bui | Unconditionally throw |
        |                       | ldTarget,             | :::                   |
        |                       |          DependencySt |                       |
        |                       | ack dependencyStack)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ConstraintValue`     | `getConstrai          | ::: block             |
        |                       | ntValue​(BuildTarget b | Unconditionally throw |
        |                       | uildTarget,           | :::                   |
        |                       |          DependencySt |                       |
        |                       | ack dependencyStack)` |                       |
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

        -   #### ThrowingConstraintResolver

                public ThrowingConstraintResolver()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getConstraintSetting(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.exceptions.DependencyStack)}

        -   #### getConstraintSetting

            ``` methodSignature
            public ConstraintSetting getConstraintSetting​(BuildTarget buildTarget,
                                                          DependencyStack dependencyStack)
            ```

            ::: block
            Unconditionally throw
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getConstraintSetting` in interface `ConstraintResolver`

            [Returns:]{.returnLabel}
            :   [`ConstraintSetting`](../../model/platform/ConstraintSetting.html "class in com.facebook.buck.core.model.platform")
                identified by a given
                [`BuildTarget`](../../model/BuildTarget.html "class in com.facebook.buck.core.model").

        []{#getConstraintValue(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.exceptions.DependencyStack)}

        -   #### getConstraintValue

            ``` methodSignature
            public ConstraintValue getConstraintValue​(BuildTarget buildTarget,
                                                      DependencyStack dependencyStack)
            ```

            ::: block
            Unconditionally throw
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getConstraintValue` in interface `ConstraintResolver`

            [Returns:]{.returnLabel}
            :   [`ConstraintValue`](../../model/platform/ConstraintValue.html "class in com.facebook.buck.core.model.platform")
                identified by a given
                [`BuildTarget`](../../model/BuildTarget.html "class in com.facebook.buck.core.model").
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

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
[Package]{.packageLabelInType} [com.facebook.buck.core.model.platform.impl](package-summary.html)
:::

## Class ConstraintBasedPlatform {#class-constraintbasedplatform .title title="Class ConstraintBasedPlatform"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.model.platform.impl.ConstraintBasedPlatform

::: description
-   

    All Implemented Interfaces:
    :   `NamedPlatform`, `Platform`

    ------------------------------------------------------------------------

        public class ConstraintBasedPlatform
        extends Object
        implements NamedPlatform

    ::: block
    An implementation of a
    [`Platform`](../Platform.html "interface in com.facebook.buck.core.model.platform")
    that has a fixed set of constraints.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                           Description
          ----------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `ConstraintBasedPlatform​(BuildTarget buildTarget,                        com.google.common.collect.ImmutableSet<ConstraintValue> constraintValues)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `BuildTarget`         | `getBuildTarget()`    | ::: block             |
        |                       |                       | Build target used to  |
        |                       |                       | define this platform  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.com       | `g                    |                       |
        | mon.collect.Immutable | etConstraintValues()` |                       |
        | Set<ConstraintValue>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `matchesAll​(Colle     | ::: block             |
        |                       | ction<ConstraintValue | A platform matches    |
        |                       | > constraintValues,   | the given constraints |
        |                       |          DependencySt | when these            |
        |                       | ack dependencyStack)` | constraints are       |
        |                       |                       | present in the        |
        |                       |                       | platform constraints  |
        |                       |                       | (platform constraints |
        |                       |                       | is a superset of the  |
        |                       |                       | provided              |
        |                       |                       | constraints).         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.google.common.collect.ImmutableSet)}

        -   #### ConstraintBasedPlatform

                public ConstraintBasedPlatform​(BuildTarget buildTarget,
                                               com.google.common.collect.ImmutableSet<ConstraintValue> constraintValues)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#matchesAll(java.util.Collection,com.facebook.buck.core.exceptions.DependencyStack)}

        -   #### matchesAll

            ``` methodSignature
            public boolean matchesAll​(Collection<ConstraintValue> constraintValues,
                                      DependencyStack dependencyStack)
            ```

            ::: block
            A platform matches the given constraints when these
            constraints are present in the platform constraints
            (platform constraints is a superset of the provided
            constraints).
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `matchesAll` in interface `Platform`

            [Returns:]{.returnLabel}
            :   `true` if the current platform matches the provided
                constraints.

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

        []{#getBuildTarget()}

        -   #### getBuildTarget

            ``` methodSignature
            public BuildTarget getBuildTarget()
            ```

            ::: block
            [Description copied from
            interface: `NamedPlatform`]{.descfrmTypeLabel}
            :::

            ::: block
            Build target used to define this platform
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildTarget` in interface `NamedPlatform`

            [Returns:]{.returnLabel}
            :   the build target of the `platform` rule where this
                platform is declared.

        []{#getConstraintValues()}

        -   #### getConstraintValues

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<ConstraintValue> getConstraintValues()
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

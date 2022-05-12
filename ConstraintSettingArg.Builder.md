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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.platform](package-summary.html)
:::

## Class ConstraintSettingArg.Builder {#class-constraintsettingarg.builder .title title="Class ConstraintSettingArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.rules.platform.ConstraintSettingArg.Builder

::: description
-   

    Enclosing class:
    :   [ConstraintSettingArg](ConstraintSettingArg.html "class in com.facebook.buck.core.rules.platform")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class ConstraintSettingArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`ConstraintSettingArg`](ConstraintSettingArg.html "class in com.facebook.buck.core.rules.platform").
    Initialize attributes and then invoke the [`build()`](#build())
    method to create an immutable instance.
    *`Builder` is not thread-safe and generally should not be stored in
    a field or collection, but instead used immediately to create
    instances.*
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `                     | `build()`             | ::: block             |
        | ConstraintSettingArg` |                       | Builds a new          |
        |                       |                       | [`ConstraintSetti     |
        |                       |                       | ngArg`](ConstraintSet |
        |                       |                       | tingArg.html "class i |
        |                       |                       | n com.facebook.buck.c |
        |                       |                       | ore.rules.platform"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Constrai             | `from​(Cons            | ::: block             |
        | ntSettingArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Constrai             | `from​(Constraint      | ::: block             |
        | ntSettingArg.Builder` | SettingArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `                     |
        |                       |                       | ConstraintSettingArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Constrai             | `from​(c               | ::: block             |
        | ntSettingArg.Builder` | om.facebook.buck.core | Copy abstract value   |
        |                       | .rules.platform.Const | type                  |
        |                       | raintSettingDescripti | `Abstract             |
        |                       | on.AbstractConstraint | ConstraintSettingArg` |
        |                       | SettingArg instance)` | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Constrai             | `                     | ::: block             |
        | ntSettingArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`n                   |
        |                       |                       | ame`](ConstraintSetti |
        |                       |                       | ngArg.html#getName()) |
        |                       |                       | attribute.            |
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
    -   []{#method.detail}

        ### Method Detail

        []{#from(com.facebook.buck.core.description.arg.ConstructorArg)}

        -   #### from

            ``` methodSignature
            public final ConstraintSettingArg.Builder from​(ConstructorArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.core.description.arg.ConstructorArg`
            instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.rules.platform.ConstraintSettingArg)}

        -   #### from

            ``` methodSignature
            public final ConstraintSettingArg.Builder from​(ConstraintSettingArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `ConstraintSettingArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.rules.platform.ConstraintSettingDescription.AbstractConstraintSettingArg)}

        -   #### from

            ``` methodSignature
            public final ConstraintSettingArg.Builder from​(com.facebook.buck.core.rules.platform.ConstraintSettingDescription.AbstractConstraintSettingArg instance)
            ```

            ::: block
            Copy abstract value type `AbstractConstraintSettingArg`
            instance into builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final ConstraintSettingArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](ConstraintSettingArg.html#getName()) attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public ConstraintSettingArg build()
            ```

            ::: block
            Builds a new
            [`ConstraintSettingArg`](ConstraintSettingArg.html "class in com.facebook.buck.core.rules.platform").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of ConstraintSettingArg

            [Throws:]{.throwsLabel}
            :   `IllegalStateException` - if any required attributes are
                missing
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

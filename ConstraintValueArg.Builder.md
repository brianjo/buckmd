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

## Class ConstraintValueArg.Builder {#class-constraintvaluearg.builder .title title="Class ConstraintValueArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.rules.platform.ConstraintValueArg.Builder

::: description
-   

    Enclosing class:
    :   [ConstraintValueArg](ConstraintValueArg.html "class in com.facebook.buck.core.rules.platform")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class ConstraintValueArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`ConstraintValueArg`](ConstraintValueArg.html "class in com.facebook.buck.core.rules.platform").
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
        | `ConstraintValueArg`  | `build()`             | ::: block             |
        |                       |                       | Builds a new          |
        |                       |                       | [`ConstraintV         |
        |                       |                       | alueArg`](ConstraintV |
        |                       |                       | alueArg.html "class i |
        |                       |                       | n com.facebook.buck.c |
        |                       |                       | ore.rules.platform"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Constr               | `from​(Cons            | ::: block             |
        | aintValueArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Constr               | `from​(Constrai        | ::: block             |
        | aintValueArg.Builder` | ntValueArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `ConstraintValueArg`  |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Constr               | `fr                   | ::: block             |
        | aintValueArg.Builder` | om​(com.facebook.buck. | Copy abstract value   |
        |                       | core.rules.platform.C | type                  |
        |                       | onstraintValueDescrip | `Abstra               |
        |                       | tion.AbstractConstrai | ctConstraintValueArg` |
        |                       | ntValueArg instance)` | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Constr               | `s                    | ::: block             |
        | aintValueArg.Builder` | etConstraintSetting​(U | Initializes the value |
        |                       | nconfiguredBuildTarge | for the               |
        |                       | t constraintSetting)` | [`cons                |
        |                       |                       | traintSetting`](Const |
        |                       |                       | raintValueArg.html#ge |
        |                       |                       | tConstraintSetting()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Constr               | `                     | ::: block             |
        | aintValueArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [                     |
        |                       |                       | `name`](ConstraintVal |
        |                       |                       | ueArg.html#getName()) |
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

        []{#from(com.facebook.buck.core.rules.platform.ConstraintValueArg)}

        -   #### from

            ``` methodSignature
            public final ConstraintValueArg.Builder from​(ConstraintValueArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `ConstraintValueArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.rules.platform.ConstraintValueDescription.AbstractConstraintValueArg)}

        -   #### from

            ``` methodSignature
            public final ConstraintValueArg.Builder from​(com.facebook.buck.core.rules.platform.ConstraintValueDescription.AbstractConstraintValueArg instance)
            ```

            ::: block
            Copy abstract value type `AbstractConstraintValueArg`
            instance into builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.ConstructorArg)}

        -   #### from

            ``` methodSignature
            public final ConstraintValueArg.Builder from​(ConstructorArg instance)
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

        []{#setConstraintSetting(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setConstraintSetting

            ``` methodSignature
            public final ConstraintValueArg.Builder setConstraintSetting​(UnconfiguredBuildTarget constraintSetting)
            ```

            ::: block
            Initializes the value for the
            [`constraintSetting`](ConstraintValueArg.html#getConstraintSetting())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `constraintSetting` - The value for constraintSetting

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final ConstraintValueArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](ConstraintValueArg.html#getName()) attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public ConstraintValueArg build()
            ```

            ::: block
            Builds a new
            [`ConstraintValueArg`](ConstraintValueArg.html "class in com.facebook.buck.core.rules.platform").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of ConstraintValueArg

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

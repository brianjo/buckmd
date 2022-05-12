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

## Class PlatformArg.Builder {#class-platformarg.builder .title title="Class PlatformArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.rules.platform.PlatformArg.Builder

::: description
-   

    Enclosing class:
    :   [PlatformArg](PlatformArg.html "class in com.facebook.buck.core.rules.platform")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class PlatformArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`PlatformArg`](PlatformArg.html "class in com.facebook.buck.core.rules.platform").
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
        | `PlatformArg.Builder` | `addAllConstrai       | ::: block             |
        |                       | ntValues​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`constraintValues    |
        |                       | ildTarget> elements)` | `](PlatformArg.html#g |
        |                       |                       | etConstraintValues()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PlatformArg.Builder` | `ad                   | ::: block             |
        |                       | dAllDeps​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`deps`](Platfo       |
        |                       | ildTarget> elements)` | rmArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PlatformArg.Builder` | `addConstrai          | ::: block             |
        |                       | ntValues​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`constraintValues    |
        |                       |                       | `](PlatformArg.html#g |
        |                       |                       | etConstraintValues()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PlatformArg.Builder` | `addConstraintVa      | ::: block             |
        |                       | lues​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`constraintValues    |
        |                       |                       | `](PlatformArg.html#g |
        |                       |                       | etConstraintValues()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PlatformArg.Builder` | `addDeps​(Unconfigured | ::: block             |
        |                       | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`deps`](Platfo       |
        |                       |                       | rmArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PlatformArg.Builder` | `add                  | ::: block             |
        |                       | Deps​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`deps`](Platfo       |
        |                       |                       | rmArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PlatformArg`         | `build()`             | ::: block             |
        |                       |                       | Builds a new          |
        |                       |                       | [`PlatformArg`](Plat  |
        |                       |                       | formArg.html "class i |
        |                       |                       | n com.facebook.buck.c |
        |                       |                       | ore.rules.platform"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PlatformArg.Builder` | `from​(Cons            | ::: block             |
        |                       | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PlatformArg.Builder` | `from​(P               | ::: block             |
        |                       | latformArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `PlatformArg`         |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PlatformArg.Builder` | `from​(com.            | ::: block             |
        |                       | facebook.buck.core.ru | Copy abstract value   |
        |                       | les.platform.Platform | type                  |
        |                       | Description.AbstractP | `AbstractPlatformArg` |
        |                       | latformArg instance)` | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PlatformArg.Builder` | `setConstrai          | ::: block             |
        |                       | ntValues​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`constraintValues    |
        |                       |                       | `](PlatformArg.html#g |
        |                       |                       | etConstraintValues()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PlatformArg.Builder` | `setDeps​(Iterable<? e | ::: block             |
        |                       | xtends UnconfiguredBu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`deps`](Platfo       |
        |                       |                       | rmArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PlatformArg.Builder` | `                     | ::: block             |
        |                       | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`name`](Platfo       |
        |                       |                       | rmArg.html#getName()) |
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

        []{#from(com.facebook.buck.core.rules.platform.PlatformArg)}

        -   #### from

            ``` methodSignature
            public final PlatformArg.Builder from​(PlatformArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `PlatformArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.rules.platform.PlatformDescription.AbstractPlatformArg)}

        -   #### from

            ``` methodSignature
            public final PlatformArg.Builder from​(com.facebook.buck.core.rules.platform.PlatformDescription.AbstractPlatformArg instance)
            ```

            ::: block
            Copy abstract value type `AbstractPlatformArg` instance into
            builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.ConstructorArg)}

        -   #### from

            ``` methodSignature
            public final PlatformArg.Builder from​(ConstructorArg instance)
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

        []{#addConstraintValues(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### addConstraintValues

            ``` methodSignature
            public final PlatformArg.Builder addConstraintValues​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`constraintValues`](PlatformArg.html#getConstraintValues())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A constraintValues element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addConstraintValues(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addConstraintValues

            ``` methodSignature
            public final PlatformArg.Builder addConstraintValues​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`constraintValues`](PlatformArg.html#getConstraintValues())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of constraintValues elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setConstraintValues(java.lang.Iterable)}

        -   #### setConstraintValues

            ``` methodSignature
            public final PlatformArg.Builder setConstraintValues​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`constraintValues`](PlatformArg.html#getConstraintValues())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of constraintValues elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllConstraintValues(java.lang.Iterable)}

        -   #### addAllConstraintValues

            ``` methodSignature
            public final PlatformArg.Builder addAllConstraintValues​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`constraintValues`](PlatformArg.html#getConstraintValues())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of constraintValues elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### addDeps

            ``` methodSignature
            public final PlatformArg.Builder addDeps​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to [`deps`](PlatformArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A deps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addDeps

            ``` methodSignature
            public final PlatformArg.Builder addDeps​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to [`deps`](PlatformArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDeps(java.lang.Iterable)}

        -   #### setDeps

            ``` methodSignature
            public final PlatformArg.Builder setDeps​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`deps`](PlatformArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllDeps(java.lang.Iterable)}

        -   #### addAllDeps

            ``` methodSignature
            public final PlatformArg.Builder addAllDeps​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to [`deps`](PlatformArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final PlatformArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](PlatformArg.html#getName()) attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public PlatformArg build()
            ```

            ::: block
            Builds a new
            [`PlatformArg`](PlatformArg.html "class in com.facebook.buck.core.rules.platform").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of PlatformArg

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

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
[Package]{.packageLabelInType} [com.facebook.buck.util.types](package-summary.html)
:::

## Class Either\<LEFT,​RIGHT\> {#class-eitherleftright .title title="Class Either"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.types.Either\<LEFT,​RIGHT\>

::: description
-   

    ------------------------------------------------------------------------

        public abstract class Either<LEFT,​RIGHT>
        extends Object

    ::: block
    A discriminated union of two parameters that holds a value of either
    the LEFT or RIGHT type.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `abstract LEFT`       | `getLeft()`           | ::: block             |
        |                       |                       | Returns the left      |
        |                       |                       | value.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abs                  | `getLeftOption()`     | ::: block             |
        | tract Optional<LEFT>` |                       | Left value or empty   |
        |                       |                       | otherwise.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract RIGHT`      | `getRight()`          | ::: block             |
        |                       |                       | Returns the right     |
        |                       |                       | value.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abst                 | `getRightOption()`    | ::: block             |
        | ract Optional<RIGHT>` |                       | Right value or empty  |
        |                       |                       | otherwise.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract boolean`    | `isLeft()`            | ::: block             |
        |                       |                       | Returns whether the   |
        |                       |                       | instance holds a left |
        |                       |                       | value.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract boolean`    | `isRight()`           | ::: block             |
        |                       |                       | Returns whether the   |
        |                       |                       | instance holds a      |
        |                       |                       | right value.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static <LEFT,​RIGH    | `ofLeft​(LEFT value)`  |                       |
        | T>Either<LEFT,​RIGHT>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static <LEFT,​RIGH    | `                     |                       |
        | T>Either<LEFT,​RIGHT>` | ofRight​(RIGHT value)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract <X> X`      | `transform​(java.util  | ::: block             |
        |                       | .function.Function<LE | Apply a function      |
        |                       | FT,​X> lhsTransformer, | based on whether the  |
        |                       |           java.util.f | instance holds a left |
        |                       | unction.Function<RIGH | or right value.       |
        |                       | T,​X> rhsTransformer)` | :::                   |
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
    -   []{#method.detail}

        ### Method Detail

        []{#isLeft()}

        -   #### isLeft

            ``` methodSignature
            public abstract boolean isLeft()
            ```

            ::: block
            Returns whether the instance holds a left value.
            :::

        []{#isRight()}

        -   #### isRight

            ``` methodSignature
            public abstract boolean isRight()
            ```

            ::: block
            Returns whether the instance holds a right value.
            :::

        []{#getLeft()}

        -   #### getLeft

            ``` methodSignature
            public abstract LEFT getLeft()
            ```

            ::: block
            Returns the left value.
            :::

            [Throws:]{.throwsLabel}
            :   `IllegalStateException` - if this instance does not hold
                a left value.

        []{#getRight()}

        -   #### getRight

            ``` methodSignature
            public abstract RIGHT getRight()
            ```

            ::: block
            Returns the right value.
            :::

            [Throws:]{.throwsLabel}
            :   `IllegalStateException` - if this instance does not hold
                a right value.

        []{#getLeftOption()}

        -   #### getLeftOption

            ``` methodSignature
            public abstract Optional<LEFT> getLeftOption()
            ```

            ::: block
            Left value or empty otherwise.
            :::

        []{#getRightOption()}

        -   #### getRightOption

            ``` methodSignature
            public abstract Optional<RIGHT> getRightOption()
            ```

            ::: block
            Right value or empty otherwise.
            :::

        []{#transform(java.util.function.Function,java.util.function.Function)}

        -   #### transform

            ``` methodSignature
            public abstract <X> X transform​(java.util.function.Function<LEFT,​X> lhsTransformer,
                                            java.util.function.Function<RIGHT,​X> rhsTransformer)
            ```

            ::: block
            Apply a function based on whether the instance holds a left
            or right value.
            :::

        []{#ofLeft(java.lang.Object)} []{#ofLeft(LEFT)}

        -   #### ofLeft

            ``` methodSignature
            public static <LEFT,​RIGHT> Either<LEFT,​RIGHT> ofLeft​(LEFT value)
            ```

        []{#ofRight(java.lang.Object)} []{#ofRight(RIGHT)}

        -   #### ofRight

            ``` methodSignature
            public static <LEFT,​RIGHT> Either<LEFT,​RIGHT> ofRight​(RIGHT value)
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

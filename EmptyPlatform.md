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
[Package]{.packageLabelInType} [com.facebook.buck.core.model.platform.impl](package-summary.html)
:::

## Class EmptyPlatform {#class-emptyplatform .title title="Class EmptyPlatform"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.model.platform.impl.EmptyPlatform

::: description
-   

    All Implemented Interfaces:
    :   `Platform`

    ------------------------------------------------------------------------

        public class EmptyPlatform
        extends Object
        implements Platform

    ::: block
    A platform that doesn\'t match any constraints.
    Note that this platform matches an empty list of constraints. The
    behavior of this platform is equivalent to
    [`ConstraintBasedPlatform`](ConstraintBasedPlatform.html "class in com.facebook.buck.core.model.platform.impl")
    with an empty list of constraints.

    Can be used in places when some platform is needed, but
    [`UnconfiguredPlatform`](UnconfiguredPlatform.html "class in com.facebook.buck.core.model.platform.impl")
    does not work because it if effectively prohibits using platforms.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type        Field        Description
          ------------------------ ------------ -------------
          `static EmptyPlatform`   `INSTANCE`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                                  Description
          ------------------- ------------------------------------------------------------------------------------------------------- -------------
          `boolean`           `equals​(Object obj)`                                                                                     
          `int`               `hashCode()`                                                                                             
          `boolean`           `matchesAll​(Collection<ConstraintValue> constraintValues,           DependencyStack dependencyStack)`    
          `String`            `toString()`                                                                                             

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

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

                public static final EmptyPlatform INSTANCE
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
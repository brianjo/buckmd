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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java.lang.model](package-summary.html)
:::

## Class BridgeMethod {#class-bridgemethod .title title="Class BridgeMethod"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.lang.model.BridgeMethod

::: description
-   

    ------------------------------------------------------------------------

        public class BridgeMethod
        extends Object

    ::: block
    A bridge method is used in Java to translate certain language
    constructs (like overriding methods with covariant return types)
    into a form that can be understood by the VM.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Field                 | Description           |
        +=======================+=======================+=======================+
        | `ExecutableElement`   | `from`                | ::: block             |
        |                       |                       | For a normal override |
        |                       |                       | bridge, this is the   |
        |                       |                       | overriding method.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ExecutableElement`   | `to`                  | ::: block             |
        |                       |                       | For a normal override |
        |                       |                       | bridge, this is the   |
        |                       |                       | method being          |
        |                       |                       | overridden.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                Description
          -------------------------------------------------------------------------- -------------
          `BridgeMethod​(ExecutableElement from,             ExecutableElement to)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `boolean`             | `equals​(Object o)`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isA                  | ::: block             |
        |                       | ccessibilityBridge()` | Bridge methods may be |
        |                       |                       | generated for public  |
        |                       |                       | methods of non-public |
        |                       |                       | superclasses to (as   |
        |                       |                       | the compiler source   |
        |                       |                       | puts it) \"work       |
        |                       |                       | around a horrible but |
        |                       |                       | permanent reflection  |
        |                       |                       | design error.\"       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isOverrideBridge()`  | ::: block             |
        |                       |                       | Bridge methods may be |
        |                       |                       | generated when an     |
        |                       |                       | overriding method has |
        |                       |                       | a different erasure   |
        |                       |                       | than the overridden   |
        |                       |                       | method, or a          |
        |                       |                       | different return      |
        |                       |                       | type.                 |
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

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#from}

        -   #### from

                public final ExecutableElement from

            ::: block
            For a normal override bridge, this is the overriding method.
            For an accessibility bridge, this is the same as
            [`to`](#to).
            :::

        []{#to}

        -   #### to

                public final ExecutableElement to

            ::: block
            For a normal override bridge, this is the method being
            overridden. For an accessibility bridge, this is a public
            method in a non-public superclass of the current class.
            :::
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(javax.lang.model.element.ExecutableElement,javax.lang.model.element.ExecutableElement)}

        -   #### BridgeMethod

                public BridgeMethod​(ExecutableElement from,
                                    ExecutableElement to)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(Object o)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `Object`

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `Object`

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

        []{#isAccessibilityBridge()}

        -   #### isAccessibilityBridge

            ``` methodSignature
            public boolean isAccessibilityBridge()
            ```

            ::: block
            Bridge methods may be generated for public methods of
            non-public superclasses to (as the compiler source puts it)
            \"work around a horrible but permanent reflection design
            error.\"
            :::

            [Returns:]{.returnLabel}
            :   true if this is such a bridge method

        []{#isOverrideBridge()}

        -   #### isOverrideBridge

            ``` methodSignature
            public boolean isOverrideBridge()
            ```

            ::: block
            Bridge methods may be generated when an overriding method
            has a different erasure than the overridden method, or a
            different return type. (The VM only sees erased types, and
            at the VM level overloading on return type is legal, so
            these bridge methods are necessary to implement overriding
            as the Java language specifies it.)
            :::

            [Returns:]{.returnLabel}
            :   true if this is such a bridge method
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

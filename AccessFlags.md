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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java.abi](package-summary.html)
:::

## Class AccessFlags {#class-accessflags .title title="Class AccessFlags"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.abi.AccessFlags

::: description
-   

    ------------------------------------------------------------------------

        public final class AccessFlags
        extends Object

    ::: block
    Computes the access flags (see JVMS8 4.1, 4.5, 4.6) for
    [`Element`](http://docs.oracle.com/javase/7/docs/api/javax/lang/model/element/Element.html?is-external=true "class or interface in javax.lang.model.element"){.externalLink}s.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                Description
          ------------------------------------------ -------------
          `AccessFlags​(ElementsExtended elements)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `int`                 | `getAccessF           | ::: block             |
        |                       | lags​(ExecutableElemen | Gets the method       |
        |                       | t executableElement)` | access flags (see     |
        |                       |                       | JVMS8 4.6) for the    |
        |                       |                       | given executable      |
        |                       |                       | element, augmented by |
        |                       |                       | the special ASM       |
        |                       |                       | pseudo-access flag    |
        |                       |                       | for \@Deprecated      |
        |                       |                       | methods.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getAccessFlags​(Type  | ::: block             |
        |                       | Element typeElement)` | Gets the class access |
        |                       |                       | flags (see JVMS8 4.1) |
        |                       |                       | for the given type    |
        |                       |                       | element, augmented by |
        |                       |                       | the special ASM       |
        |                       |                       | pseudo-access flag    |
        |                       |                       | for \@Deprecated      |
        |                       |                       | types.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getAcc               | ::: block             |
        |                       | essFlags​(VariableElem | Gets the field access |
        |                       | ent variableElement)` | flags (see JVMS8 4.5) |
        |                       |                       | for the given         |
        |                       |                       | variable element,     |
        |                       |                       | augmented by the      |
        |                       |                       | special ASM           |
        |                       |                       | pseudo-access flag    |
        |                       |                       | for \@Deprecated      |
        |                       |                       | fields.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `                     | ::: block             |
        |                       | getAccessFlagsForClas | Gets the class access |
        |                       | sNode​(TypeElement e)` | flags (see JVMS8 4.1) |
        |                       |                       | for the given type    |
        |                       |                       | element as they       |
        |                       |                       | should appear in the  |
        |                       |                       | ClassNode of a class  |
        |                       |                       | file.                 |
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.jvm.java.lang.model.ElementsExtended)}

        -   #### AccessFlags

                public AccessFlags​(ElementsExtended elements)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getAccessFlagsForClassNode(javax.lang.model.element.TypeElement)}

        -   #### getAccessFlagsForClassNode

            ``` methodSignature
            public int getAccessFlagsForClassNode​(TypeElement e)
            ```

            ::: block
            Gets the class access flags (see JVMS8 4.1) for the given
            type element as they should appear in the ClassNode of a
            class file. Inner-class specific flags are not allowed in
            that node, presumably for compatibility reasons.
            :::

        []{#getAccessFlags(javax.lang.model.element.TypeElement)}

        -   #### getAccessFlags

            ``` methodSignature
            public int getAccessFlags​(TypeElement typeElement)
            ```

            ::: block
            Gets the class access flags (see JVMS8 4.1) for the given
            type element, augmented by the special ASM pseudo-access
            flag for \@Deprecated types.
            :::

        []{#getAccessFlags(javax.lang.model.element.ExecutableElement)}

        -   #### getAccessFlags

            ``` methodSignature
            public int getAccessFlags​(ExecutableElement executableElement)
            ```

            ::: block
            Gets the method access flags (see JVMS8 4.6) for the given
            executable element, augmented by the special ASM
            pseudo-access flag for \@Deprecated methods.
            :::

        []{#getAccessFlags(javax.lang.model.element.VariableElement)}

        -   #### getAccessFlags

            ``` methodSignature
            public int getAccessFlags​(VariableElement variableElement)
            ```

            ::: block
            Gets the field access flags (see JVMS8 4.5) for the given
            variable element, augmented by the special ASM pseudo-access
            flag for \@Deprecated fields.
            :::
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

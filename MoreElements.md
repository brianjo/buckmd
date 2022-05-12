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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java.lang.model](package-summary.html)
:::

## Class MoreElements {#class-moreelements .title title="Class MoreElements"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.lang.model.MoreElements

::: description
-   

    ------------------------------------------------------------------------

        public final class MoreElements
        extends Object

    ::: block
    More utility functions for working with
    [`Element`](http://docs.oracle.com/javase/7/docs/api/javax/lang/model/element/Element.html?is-external=true "class or interface in javax.lang.model.element"){.externalLink}s,
    along the lines of those found on
    [`Elements`](http://docs.oracle.com/javase/7/docs/api/javax/lang/model/util/Elements.html?is-external=true "class or interface in javax.lang.model.util"){.externalLink}.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `st                   | `getInterfac          |                       |
        | atic java.util.stream | es​(TypeElement type)` |                       |
        | .Stream<TypeElement>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Element`      | `getOuterClass​(       |                       |
        |                       | ExecutableElement e)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `s                    | `getPackageElem       |                       |
        | tatic PackageElement` | ent​(Element element)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `s                    | `getPackageElementE   | ::: block             |
        | tatic PackageElement` | venIfEmpty​(Elements e | Get a package by      |
        |                       | lements,              | name, even if it has  |
        |                       |                 CharS | no members.           |
        |                       | equence packageName)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static TypeElement`  | `getSupercla          |                       |
        |                       | ss​(TypeElement type)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static TypeElement`  | `getTopLevelTypeElem  |                       |
        |                       | ent​(Element element)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `ge                   |                       |
        | atic java.util.stream | tTransitiveSuperclass |                       |
        | .Stream<TypeElement>` | es​(TypeElement type)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static TypeElement`  | `getTypeElem          |                       |
        |                       | ent​(Element element)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `isConstructor​(       |                       |
        |                       | ExecutableElement e)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `isInner              |                       |
        |                       | Class​(TypeElement e)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `isI                  |                       |
        |                       | nnerClassConstructor​( |                       |
        |                       | ExecutableElement e)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `isRunt               |                       |
        |                       | imeRetention​(Annotati |                       |
        |                       | onMirror annotation)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `isSou                |                       |
        |                       | rceRetention​(Annotati |                       |
        |                       | onMirror annotation)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `i                    |                       |
        |                       | sTransitiveMemberClas |                       |
        |                       | s​(TypeElement inner,  |                       |
        |                       |                       |                       |
        |                       |   TypeElement outer)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
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

        []{#getPackageElementEvenIfEmpty(javax.lang.model.util.Elements,java.lang.CharSequence)}

        -   #### getPackageElementEvenIfEmpty

            ``` methodSignature
            public static PackageElement getPackageElementEvenIfEmpty​(Elements elements,
                                                                      CharSequence packageName)
            ```

            ::: block
            Get a package by name, even if it has no members.
            :::

        []{#getSuperclass(javax.lang.model.element.TypeElement)}

        -   #### getSuperclass

            ``` methodSignature
            public static TypeElement getSuperclass​(TypeElement type)
            ```

        []{#getInterfaces(javax.lang.model.element.TypeElement)}

        -   #### getInterfaces

            ``` methodSignature
            public static java.util.stream.Stream<TypeElement> getInterfaces​(TypeElement type)
            ```

        []{#getTransitiveSuperclasses(javax.lang.model.element.TypeElement)}

        -   #### getTransitiveSuperclasses

            ``` methodSignature
            public static java.util.stream.Stream<TypeElement> getTransitiveSuperclasses​(TypeElement type)
            ```

        []{#isTransitiveMemberClass(javax.lang.model.element.TypeElement,javax.lang.model.element.TypeElement)}

        -   #### isTransitiveMemberClass

            ``` methodSignature
            public static boolean isTransitiveMemberClass​(TypeElement inner,
                                                          TypeElement outer)
            ```

        []{#getTypeElement(javax.lang.model.element.Element)}

        -   #### getTypeElement

            ``` methodSignature
            public static TypeElement getTypeElement​(Element element)
            ```

        []{#getTopLevelTypeElement(javax.lang.model.element.Element)}

        -   #### getTopLevelTypeElement

            ``` methodSignature
            public static TypeElement getTopLevelTypeElement​(Element element)
            ```

        []{#getPackageElement(javax.lang.model.element.Element)}

        -   #### getPackageElement

            ``` methodSignature
            public static PackageElement getPackageElement​(Element element)
            ```

        []{#isInnerClassConstructor(javax.lang.model.element.ExecutableElement)}

        -   #### isInnerClassConstructor

            ``` methodSignature
            public static boolean isInnerClassConstructor​(ExecutableElement e)
            ```

        []{#isConstructor(javax.lang.model.element.ExecutableElement)}

        -   #### isConstructor

            ``` methodSignature
            public static boolean isConstructor​(ExecutableElement e)
            ```

        []{#isInnerClass(javax.lang.model.element.TypeElement)}

        -   #### isInnerClass

            ``` methodSignature
            public static boolean isInnerClass​(TypeElement e)
            ```

        []{#getOuterClass(javax.lang.model.element.ExecutableElement)}

        -   #### getOuterClass

            ``` methodSignature
            public static Element getOuterClass​(ExecutableElement e)
            ```

        []{#isRuntimeRetention(javax.lang.model.element.AnnotationMirror)}

        -   #### isRuntimeRetention

            ``` methodSignature
            public static boolean isRuntimeRetention​(AnnotationMirror annotation)
            ```

        []{#isSourceRetention(javax.lang.model.element.AnnotationMirror)}

        -   #### isSourceRetention

            ``` methodSignature
            public static boolean isSourceRetention​(AnnotationMirror annotation)
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

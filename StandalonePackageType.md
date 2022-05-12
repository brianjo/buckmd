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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java.abi.source](package-summary.html)
:::

## Class StandalonePackageType {#class-standalonepackagetype .title title="Class StandalonePackageType"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.abi.source.StandalonePackageType

::: description
-   

    All Implemented Interfaces:
    :   `AnnotatedConstruct`, `NoType`, `TypeMirror`

    ------------------------------------------------------------------------

        public class StandalonePackageType
        extends Object
        implements NoType
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                              Description
          -------------------------------------------------------------------------------------------------------- -------------
          `StandalonePackageType​(com.facebook.buck.jvm.java.abi.source.ArtificialPackageElement packageElement)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                  Method                                            Description
          ------------------------------------------------------------------ ------------------------------------------------- -------------
          `<R,​P>R`                                                           `accept​(TypeVisitor<R,​P> v,       P p)`            
          `com.facebook.buck.jvm.java.abi.source.ArtificialPackageElement`   `asElement()`                                      
          `<A extends Annotation>A`                                          `getAnnotation​(Class<A> annotationType)`           
          `List<? extends AnnotationMirror>`                                 `getAnnotationMirrors()`                           
          `<A extends Annotation>A[]`                                        `getAnnotationsByType​(Class<A> annotationType)`    
          `TypeKind`                                                         `getKind()`                                        
          `String`                                                           `toString()`                                       

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.javax.lang.model.AnnotatedConstruct}

            ### Methods inherited from interface javax.lang.model.[AnnotatedConstruct](http://docs.oracle.com/javase/7/docs/api/javax/lang/model/AnnotatedConstruct.html?is-external=true "class or interface in javax.lang.model"){.externalLink}

            `getAnnotation, getAnnotationMirrors, getAnnotationsByType`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.javax.lang.model.type.TypeMirror}

            ### Methods inherited from interface javax.lang.model.type.[TypeMirror](http://docs.oracle.com/javase/7/docs/api/javax/lang/model/type/TypeMirror.html?is-external=true "class or interface in javax.lang.model.type"){.externalLink}

            `accept, equals, getKind, hashCode`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.jvm.java.abi.source.ArtificialPackageElement)}

        -   #### StandalonePackageType

                public StandalonePackageType​(com.facebook.buck.jvm.java.abi.source.ArtificialPackageElement packageElement)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#asElement()}

        -   #### asElement

            ``` methodSignature
            public com.facebook.buck.jvm.java.abi.source.ArtificialPackageElement asElement()
            ```

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `toString` in interface `TypeMirror`

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

        []{#getKind()}

        -   #### getKind

            ``` methodSignature
            public TypeKind getKind()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getKind` in interface `TypeMirror`

        []{#accept(javax.lang.model.type.TypeVisitor,java.lang.Object)}
        []{#accept(javax.lang.model.type.TypeVisitor,P)}

        -   #### accept

            ``` methodSignature
            public <R,​P> R accept​(TypeVisitor<R,​P> v,
                                        P p)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `accept` in interface `TypeMirror`

        []{#getAnnotationMirrors()}

        -   #### getAnnotationMirrors

            ``` methodSignature
            public List<? extends AnnotationMirror> getAnnotationMirrors()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getAnnotationMirrors` in interface `AnnotatedConstruct`

        []{#getAnnotation(java.lang.Class)}

        -   #### getAnnotation

            ``` methodSignature
            public <A extends Annotation> A getAnnotation​(Class<A> annotationType)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getAnnotation` in interface `AnnotatedConstruct`

        []{#getAnnotationsByType(java.lang.Class)}

        -   #### getAnnotationsByType

            ``` methodSignature
            public <A extends Annotation> A[] getAnnotationsByType​(Class<A> annotationType)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getAnnotationsByType` in interface `AnnotatedConstruct`
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

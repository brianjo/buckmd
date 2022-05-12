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

## Class TypeScanner8\<R,​P\> {#class-typescanner8rp .title title="Class TypeScanner8"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [javax.lang.model.util.AbstractTypeVisitor6](http://docs.oracle.com/javase/7/docs/api/javax/lang/model/util/AbstractTypeVisitor6.html?is-external=true "class or interface in javax.lang.model.util"){.externalLink}\<R,​P\>

    -   -   [javax.lang.model.util.AbstractTypeVisitor7](http://docs.oracle.com/javase/7/docs/api/javax/lang/model/util/AbstractTypeVisitor7.html?is-external=true "class or interface in javax.lang.model.util"){.externalLink}\<R,​P\>

        -   -   [javax.lang.model.util.AbstractTypeVisitor8](http://docs.oracle.com/javase/7/docs/api/javax/lang/model/util/AbstractTypeVisitor8.html?is-external=true "class or interface in javax.lang.model.util"){.externalLink}\<R,​P\>

            -   -   com.facebook.buck.jvm.java.abi.TypeScanner8\<R,​P\>

::: description
-   

    All Implemented Interfaces:
    :   `TypeVisitor<R,​P>`

    ------------------------------------------------------------------------

        public class TypeScanner8<R,​P>
        extends AbstractTypeVisitor8<R,​P>

    ::: block
    A scanning visitor of
    [`TypeMirror`](http://docs.oracle.com/javase/7/docs/api/javax/lang/model/type/TypeMirror.html?is-external=true "class or interface in javax.lang.model.type"){.externalLink}s
    for
    [`SourceVersion.RELEASE_8`](http://docs.oracle.com/javase/7/docs/api/javax/lang/model/SourceVersion.html?is-external=true#RELEASE_8 "class or interface in javax.lang.model"){.externalLink}.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                      Description
          -------------- -------------------------------- -------------
          `protected `   `TypeScanner8()`                  
          `protected `   `TypeScanner8​(R defaultValue)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                          Description
          ------------------- --------------------------------------------------------------- -------------
          `R`                 `scan​(Iterable<? extends TypeMirror> iterable,     P p)`         
          `R`                 `scan​(TypeMirror t)`                                             
          `R`                 `scan​(TypeMirror t,     P p)`                                    
          `R`                 `visitArray​(ArrayType t,           P p)`                         
          `R`                 `visitDeclared​(DeclaredType t,              P p)`                
          `R`                 `visitError​(ErrorType t,           P p)`                         
          `R`                 `visitExecutable​(ExecutableType t,                P p)`          
          `R`                 `visitIntersection​(IntersectionType t,                  P p)`    
          `R`                 `visitNoType​(NoType t,            P p)`                          
          `R`                 `visitNull​(NullType t,          P p)`                            
          `R`                 `visitPrimitive​(PrimitiveType t,               P p)`             
          `R`                 `visitTypeVariable​(TypeVariable t,                  P p)`        
          `R`                 `visitUnion​(UnionType t,           P p)`                         
          `R`                 `visitWildcard​(WildcardType t,              P p)`                

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.javax.lang.model.util.AbstractTypeVisitor6}

            ### Methods inherited from class javax.lang.model.util.[AbstractTypeVisitor6](http://docs.oracle.com/javase/7/docs/api/javax/lang/model/util/AbstractTypeVisitor6.html?is-external=true "class or interface in javax.lang.model.util"){.externalLink}

            `visit, visit, visitUnknown`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### TypeScanner8

                protected TypeScanner8()

        []{#<init>(java.lang.Object)} []{#<init>(R)}

        -   #### TypeScanner8

                protected TypeScanner8​(@Nullable
                                       R defaultValue)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#scan(java.lang.Iterable,java.lang.Object)}
        []{#scan(java.lang.Iterable,P)}

        -   #### scan

            ``` methodSignature
            @Nullable
            public final R scan​(Iterable<? extends TypeMirror> iterable,
                                P p)
            ```

        []{#scan(javax.lang.model.type.TypeMirror,java.lang.Object)}
        []{#scan(javax.lang.model.type.TypeMirror,P)}

        -   #### scan

            ``` methodSignature
            @Nullable
            public R scan​(TypeMirror t,
                          P p)
            ```

        []{#scan(javax.lang.model.type.TypeMirror)}

        -   #### scan

            ``` methodSignature
            @Nullable
            public final R scan​(TypeMirror t)
            ```

        []{#visitPrimitive(javax.lang.model.type.PrimitiveType,java.lang.Object)}
        []{#visitPrimitive(javax.lang.model.type.PrimitiveType,P)}

        -   #### visitPrimitive

            ``` methodSignature
            @Nullable
            public R visitPrimitive​(PrimitiveType t,
                                    P p)
            ```

        []{#visitNull(javax.lang.model.type.NullType,java.lang.Object)}
        []{#visitNull(javax.lang.model.type.NullType,P)}

        -   #### visitNull

            ``` methodSignature
            @Nullable
            public R visitNull​(NullType t,
                               P p)
            ```

        []{#visitArray(javax.lang.model.type.ArrayType,java.lang.Object)}
        []{#visitArray(javax.lang.model.type.ArrayType,P)}

        -   #### visitArray

            ``` methodSignature
            @Nullable
            public R visitArray​(ArrayType t,
                                P p)
            ```

        []{#visitDeclared(javax.lang.model.type.DeclaredType,java.lang.Object)}
        []{#visitDeclared(javax.lang.model.type.DeclaredType,P)}

        -   #### visitDeclared

            ``` methodSignature
            @Nullable
            public R visitDeclared​(DeclaredType t,
                                   P p)
            ```

        []{#visitError(javax.lang.model.type.ErrorType,java.lang.Object)}
        []{#visitError(javax.lang.model.type.ErrorType,P)}

        -   #### visitError

            ``` methodSignature
            @Nullable
            public R visitError​(ErrorType t,
                                P p)
            ```

        []{#visitTypeVariable(javax.lang.model.type.TypeVariable,java.lang.Object)}
        []{#visitTypeVariable(javax.lang.model.type.TypeVariable,P)}

        -   #### visitTypeVariable

            ``` methodSignature
            @Nullable
            public R visitTypeVariable​(TypeVariable t,
                                       P p)
            ```

        []{#visitWildcard(javax.lang.model.type.WildcardType,java.lang.Object)}
        []{#visitWildcard(javax.lang.model.type.WildcardType,P)}

        -   #### visitWildcard

            ``` methodSignature
            @Nullable
            public R visitWildcard​(WildcardType t,
                                   P p)
            ```

        []{#visitExecutable(javax.lang.model.type.ExecutableType,java.lang.Object)}
        []{#visitExecutable(javax.lang.model.type.ExecutableType,P)}

        -   #### visitExecutable

            ``` methodSignature
            @Nullable
            public R visitExecutable​(ExecutableType t,
                                     P p)
            ```

        []{#visitNoType(javax.lang.model.type.NoType,java.lang.Object)}
        []{#visitNoType(javax.lang.model.type.NoType,P)}

        -   #### visitNoType

            ``` methodSignature
            @Nullable
            public R visitNoType​(NoType t,
                                 P p)
            ```

        []{#visitIntersection(javax.lang.model.type.IntersectionType,java.lang.Object)}
        []{#visitIntersection(javax.lang.model.type.IntersectionType,P)}

        -   #### visitIntersection

            ``` methodSignature
            @Nullable
            public R visitIntersection​(IntersectionType t,
                                       P p)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `visitIntersection` in interface `TypeVisitor<R,​P>`

            [Specified by:]{.overrideSpecifyLabel}
            :   `visitIntersection` in class `AbstractTypeVisitor8<R,​P>`

        []{#visitUnion(javax.lang.model.type.UnionType,java.lang.Object)}
        []{#visitUnion(javax.lang.model.type.UnionType,P)}

        -   #### visitUnion

            ``` methodSignature
            @Nullable
            public R visitUnion​(UnionType t,
                                P p)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `visitUnion` in interface `TypeVisitor<R,​P>`

            [Specified by:]{.overrideSpecifyLabel}
            :   `visitUnion` in class `AbstractTypeVisitor7<R,​P>`
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

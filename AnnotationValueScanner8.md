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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java.lang.model](package-summary.html)
:::

## Class AnnotationValueScanner8\<R,​P\> {#class-annotationvaluescanner8rp .title title="Class AnnotationValueScanner8"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [javax.lang.model.util.AbstractAnnotationValueVisitor6](http://docs.oracle.com/javase/7/docs/api/javax/lang/model/util/AbstractAnnotationValueVisitor6.html?is-external=true "class or interface in javax.lang.model.util"){.externalLink}\<R,​P\>

    -   -   [javax.lang.model.util.AbstractAnnotationValueVisitor7](http://docs.oracle.com/javase/7/docs/api/javax/lang/model/util/AbstractAnnotationValueVisitor7.html?is-external=true "class or interface in javax.lang.model.util"){.externalLink}\<R,​P\>

        -   -   [javax.lang.model.util.AbstractAnnotationValueVisitor8](http://docs.oracle.com/javase/7/docs/api/javax/lang/model/util/AbstractAnnotationValueVisitor8.html?is-external=true "class or interface in javax.lang.model.util"){.externalLink}\<R,​P\>

            -   -   com.facebook.buck.jvm.java.lang.model.AnnotationValueScanner8\<R,​P\>

::: description
-   

    All Implemented Interfaces:
    :   `AnnotationValueVisitor<R,​P>`

    ------------------------------------------------------------------------

        public class AnnotationValueScanner8<R,​P>
        extends AbstractAnnotationValueVisitor8<R,​P>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                                 Description
          -------------- ------------------------------------------- -------------
          `protected `   `AnnotationValueScanner8()`                  
          `protected `   `AnnotationValueScanner8​(R defaultValue)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                              Description
          ------------------- ------------------------------------------------------------------- -------------
          `R`                 `scan​(Iterable<? extends AnnotationValue> iterable,     P p)`        
          `R`                 `scan​(AnnotationValue value)`                                        
          `R`                 `scan​(AnnotationValue value,     P p)`                               
          `R`                 `visitAnnotation​(AnnotationMirror a,                P p)`            
          `R`                 `visitArray​(List<? extends AnnotationValue> vals,           P p)`    
          `R`                 `visitBoolean​(boolean b,             P p)`                           
          `R`                 `visitByte​(byte b,          P p)`                                    
          `R`                 `visitChar​(char c,          P p)`                                    
          `R`                 `visitDouble​(double d,            P p)`                              
          `R`                 `visitEnumConstant​(VariableElement c,                  P p)`         
          `R`                 `visitFloat​(float f,           P p)`                                 
          `R`                 `visitInt​(int i,         P p)`                                       
          `R`                 `visitLong​(long i,          P p)`                                    
          `R`                 `visitShort​(short s,           P p)`                                 
          `R`                 `visitString​(String s,            P p)`                              
          `R`                 `visitType​(TypeMirror t,          P p)`                              
          `R`                 `visitUnknown​(AnnotationValue av,             P p)`                  

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.javax.lang.model.util.AbstractAnnotationValueVisitor6}

            ### Methods inherited from class javax.lang.model.util.[AbstractAnnotationValueVisitor6](http://docs.oracle.com/javase/7/docs/api/javax/lang/model/util/AbstractAnnotationValueVisitor6.html?is-external=true "class or interface in javax.lang.model.util"){.externalLink}

            `visit, visit`

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

        -   #### AnnotationValueScanner8

                protected AnnotationValueScanner8()

        []{#<init>(java.lang.Object)} []{#<init>(R)}

        -   #### AnnotationValueScanner8

                protected AnnotationValueScanner8​(R defaultValue)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#scan(java.lang.Iterable,java.lang.Object)}
        []{#scan(java.lang.Iterable,P)}

        -   #### scan

            ``` methodSignature
            public final R scan​(Iterable<? extends AnnotationValue> iterable,
                                P p)
            ```

        []{#scan(javax.lang.model.element.AnnotationValue,java.lang.Object)}
        []{#scan(javax.lang.model.element.AnnotationValue,P)}

        -   #### scan

            ``` methodSignature
            public R scan​(AnnotationValue value,
                          P p)
            ```

        []{#scan(javax.lang.model.element.AnnotationValue)}

        -   #### scan

            ``` methodSignature
            public final R scan​(AnnotationValue value)
            ```

        []{#visitBoolean(boolean,java.lang.Object)}
        []{#visitBoolean(boolean,P)}

        -   #### visitBoolean

            ``` methodSignature
            public R visitBoolean​(boolean b,
                                  P p)
            ```

        []{#visitByte(byte,java.lang.Object)} []{#visitByte(byte,P)}

        -   #### visitByte

            ``` methodSignature
            public R visitByte​(byte b,
                               P p)
            ```

        []{#visitChar(char,java.lang.Object)} []{#visitChar(char,P)}

        -   #### visitChar

            ``` methodSignature
            public R visitChar​(char c,
                               P p)
            ```

        []{#visitDouble(double,java.lang.Object)}
        []{#visitDouble(double,P)}

        -   #### visitDouble

            ``` methodSignature
            public R visitDouble​(double d,
                                 P p)
            ```

        []{#visitFloat(float,java.lang.Object)} []{#visitFloat(float,P)}

        -   #### visitFloat

            ``` methodSignature
            public R visitFloat​(float f,
                                P p)
            ```

        []{#visitInt(int,java.lang.Object)} []{#visitInt(int,P)}

        -   #### visitInt

            ``` methodSignature
            public R visitInt​(int i,
                              P p)
            ```

        []{#visitLong(long,java.lang.Object)} []{#visitLong(long,P)}

        -   #### visitLong

            ``` methodSignature
            public R visitLong​(long i,
                               P p)
            ```

        []{#visitShort(short,java.lang.Object)} []{#visitShort(short,P)}

        -   #### visitShort

            ``` methodSignature
            public R visitShort​(short s,
                                P p)
            ```

        []{#visitString(java.lang.String,java.lang.Object)}
        []{#visitString(java.lang.String,P)}

        -   #### visitString

            ``` methodSignature
            public R visitString​(String s,
                                 P p)
            ```

        []{#visitType(javax.lang.model.type.TypeMirror,java.lang.Object)}
        []{#visitType(javax.lang.model.type.TypeMirror,P)}

        -   #### visitType

            ``` methodSignature
            public R visitType​(TypeMirror t,
                               P p)
            ```

        []{#visitEnumConstant(javax.lang.model.element.VariableElement,java.lang.Object)}
        []{#visitEnumConstant(javax.lang.model.element.VariableElement,P)}

        -   #### visitEnumConstant

            ``` methodSignature
            public R visitEnumConstant​(VariableElement c,
                                       P p)
            ```

        []{#visitAnnotation(javax.lang.model.element.AnnotationMirror,java.lang.Object)}
        []{#visitAnnotation(javax.lang.model.element.AnnotationMirror,P)}

        -   #### visitAnnotation

            ``` methodSignature
            public R visitAnnotation​(AnnotationMirror a,
                                     P p)
            ```

        []{#visitArray(java.util.List,java.lang.Object)}
        []{#visitArray(java.util.List,P)}

        -   #### visitArray

            ``` methodSignature
            public R visitArray​(List<? extends AnnotationValue> vals,
                                P p)
            ```

        []{#visitUnknown(javax.lang.model.element.AnnotationValue,java.lang.Object)}
        []{#visitUnknown(javax.lang.model.element.AnnotationValue,P)}

        -   #### visitUnknown

            ``` methodSignature
            public R visitUnknown​(AnnotationValue av,
                                  P p)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `visitUnknown` in
                interface `AnnotationValueVisitor<R,​P>`

            [Overrides:]{.overrideSpecifyLabel}
            :   `visitUnknown` in
                class `AbstractAnnotationValueVisitor6<R,​P>`
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

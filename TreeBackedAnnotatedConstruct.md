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

## Class TreeBackedAnnotatedConstruct {#class-treebackedannotatedconstruct .title title="Class TreeBackedAnnotatedConstruct"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.abi.source.TreeBackedAnnotatedConstruct

::: description
-   

    All Implemented Interfaces:
    :   `AnnotatedConstruct`

    ------------------------------------------------------------------------

        public class TreeBackedAnnotatedConstruct
        extends Object

    ::: block
    An implementation of
    [`AnnotatedConstruct`](http://docs.oracle.com/javase/7/docs/api/javax/lang/model/AnnotatedConstruct.html?is-external=true "class or interface in javax.lang.model"){.externalLink}
    that uses only the information available from a `Tree`. This results
    in an incomplete implementation; see documentation for individual
    methods and
    [`com.facebook.buck.jvm.java.abi.source`](package-summary.html) for
    more information.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                              Description
          ------------------------------------------------------------------------ -------------
          `TreeBackedAnnotatedConstruct​(AnnotatedConstruct underlyingConstruct)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                                    Method                                            Description
          ------------------------------------------------------------------------------------ ------------------------------------------------- -------------
          `<A extends Annotation>A`                                                            `getAnnotation​(Class<A> annotationType)`           
          `List<? extends com.facebook.buck.jvm.java.abi.source.ArtificialAnnotationMirror>`   `getAnnotationMirrors()`                           
          `<A extends Annotation>A[]`                                                          `getAnnotationsByType​(Class<A> annotationType)`    

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

        []{#<init>(javax.lang.model.AnnotatedConstruct)}

        -   #### TreeBackedAnnotatedConstruct

                public TreeBackedAnnotatedConstruct​(AnnotatedConstruct underlyingConstruct)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getAnnotationMirrors()}

        -   #### getAnnotationMirrors

            ``` methodSignature
            public List<? extends com.facebook.buck.jvm.java.abi.source.ArtificialAnnotationMirror> getAnnotationMirrors()
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

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

## Class TreeBackedAnnotationFactory {#class-treebackedannotationfactory .title title="Class TreeBackedAnnotationFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.abi.source.TreeBackedAnnotationFactory

::: description
-   

    ------------------------------------------------------------------------

        public class TreeBackedAnnotationFactory
        extends Object

    ::: block
    Support for \@{link TreeBackedAnnotatedConstruct#getAnnotation}.
    `getAnnotation` can throw unexpected exceptions when building
    source-only ABIs, due to some of the classes it tries to load being
    unavailable. We try to return our own implementations of the
    annotations instead, bypassing javac\'s support altogether. However,
    if the annotation processor requests a field that we can\'t fake, we
    have to fall back to the underlying annotation.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                       Description
          --------------------------------- -------------
          `TreeBackedAnnotationFactory()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                  Method                                                                                                                                                                                Description
          ---------------------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `static <A extends Annotation>A`   `createOrGetUnderlying​(TreeBackedAnnotatedConstruct annotatedConstruct,                      AnnotatedConstruct underlyingConstruct,                      Class<A> annotationType)`    

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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### TreeBackedAnnotationFactory

                public TreeBackedAnnotationFactory()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#createOrGetUnderlying(com.facebook.buck.jvm.java.abi.source.TreeBackedAnnotatedConstruct,javax.lang.model.AnnotatedConstruct,java.lang.Class)}

        -   #### createOrGetUnderlying

            ``` methodSignature
            public static <A extends Annotation> A createOrGetUnderlying​(TreeBackedAnnotatedConstruct annotatedConstruct,
                                                                         AnnotatedConstruct underlyingConstruct,
                                                                         Class<A> annotationType)
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

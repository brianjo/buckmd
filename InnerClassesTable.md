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

## Class InnerClassesTable {#class-innerclassestable .title title="Class InnerClassesTable"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.abi.InnerClassesTable

::: description
-   

    ------------------------------------------------------------------------

        public class InnerClassesTable
        extends Object

    ::: block
    Aids in constructing a table of `InnerClassNode`s when generating
    bytecode for a
    [`TypeElement`](http://docs.oracle.com/javase/7/docs/api/javax/lang/model/element/TypeElement.html?is-external=true "class or interface in javax.lang.model.element"){.externalLink}.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                   Description
          ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `InnerClassesTable​(com.facebook.buck.jvm.java.abi.DescriptorFactory descriptorFactory,                  AccessFlags accessFlagsUtils,                  Element topElement)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                    Description
          ------------------- ------------------------------------------------------------------------- -------------
          `void`              `addTypeReferences​(List<? extends AnnotationMirror> annotationMirrors)`    
          `void`              `addTypeReferences​(Element element)`                                       
          `void`              `addTypeReferences​(TypeMirror type)`                                       
          `void`              `reportInnerClassReferences​(org.objectweb.asm.ClassVisitor visitor)`       

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

        []{#<init>(com.facebook.buck.jvm.java.abi.DescriptorFactory,com.facebook.buck.jvm.java.abi.AccessFlags,javax.lang.model.element.Element)}

        -   #### InnerClassesTable

                public InnerClassesTable​(com.facebook.buck.jvm.java.abi.DescriptorFactory descriptorFactory,
                                         AccessFlags accessFlagsUtils,
                                         Element topElement)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#addTypeReferences(javax.lang.model.element.Element)}

        -   #### addTypeReferences

            ``` methodSignature
            public void addTypeReferences​(Element element)
            ```

        []{#addTypeReferences(javax.lang.model.type.TypeMirror)}

        -   #### addTypeReferences

            ``` methodSignature
            public void addTypeReferences​(TypeMirror type)
            ```

        []{#addTypeReferences(java.util.List)}

        -   #### addTypeReferences

            ``` methodSignature
            public void addTypeReferences​(List<? extends AnnotationMirror> annotationMirrors)
            ```

        []{#reportInnerClassReferences(org.objectweb.asm.ClassVisitor)}

        -   #### reportInnerClassReferences

            ``` methodSignature
            public void reportInnerClassReferences​(org.objectweb.asm.ClassVisitor visitor)
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

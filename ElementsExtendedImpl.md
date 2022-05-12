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
-   [Nested](#nested.class.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java.plugin.adapter](package-summary.html)
:::

## Class ElementsExtendedImpl {#class-elementsextendedimpl .title title="Class ElementsExtendedImpl"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.plugin.adapter.ElementsExtendedImpl

::: description
-   

    All Implemented Interfaces:
    :   `ElementsExtended`, `Elements`

    ------------------------------------------------------------------------

        public class ElementsExtendedImpl
        extends Object
        implements ElementsExtended

    ::: block
    Wraps and extends
    [`Elements`](http://docs.oracle.com/javase/7/docs/api/javax/lang/model/util/Elements.html?is-external=true "class or interface in javax.lang.model.util"){.externalLink}
    with methods that cannot be added as pure extension methods on
    [`MoreElements`](../../lang/model/MoreElements.html "class in com.facebook.buck.jvm.java.lang.model")
    because they require per-instance state.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.javax.lang.model.util.Elements}

            ### Nested classes/interfaces inherited from interface javax.lang.model.util.[Elements](http://docs.oracle.com/javase/7/docs/api/javax/lang/model/util/Elements.html?is-external=true "class or interface in javax.lang.model.util"){.externalLink}

            `Elements.Origin`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                    Description
          ------------------------------------------------------------------------------------------------------------------------------ -------------
          `ElementsExtendedImpl​(Elements inner,                     Types types,                     com.sun.source.util.Trees trees)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                              Method                                                                                                       Description
          -------------------------------------------------------------- ------------------------------------------------------------------------------------------------------------ -------------
          `List<? extends AnnotationMirror>`                             `getAllAnnotationMirrors​(Element e)`                                                                          
          `List<BridgeMethod>`                                           `getAllBridgeMethods​(TypeElement type)`                                                                       
          `List<? extends Element>`                                      `getAllMembers​(TypeElement type)`                                                                             
          `List<ExecutableElement>`                                      `getAllMethods​(TypeElement owner,              CharSequence name)`                                            
          `Set<? extends ModuleElement>`                                 `getAllModuleElements()`                                                                                      
          `Set<? extends PackageElement>`                                `getAllPackageElements​(CharSequence name)`                                                                    
          `TypeElement`                                                  `getBinaryImplementationOwner​(ExecutableElement method,                             TypeElement inType)`      
          `Name`                                                         `getBinaryName​(TypeElement type)`                                                                             
          `List<BridgeMethod>`                                           `getBridgeMethods​(TypeElement owner,                 CharSequence name)`                                      
          `String`                                                       `getConstantExpression​(Object value)`                                                                         
          `List<ExecutableElement>`                                      `getDeclaredMethods​(TypeElement owner,                   CharSequence name)`                                  
          `String`                                                       `getDocComment​(Element e)`                                                                                    
          `Map<? extends ExecutableElement,​? extends AnnotationValue>`   `getElementValuesWithDefaults​(AnnotationMirror a)`                                                            
          `ExecutableElement`                                            `getImplementation​(ExecutableElement baseMethod,                  TypeElement inType)`                        
          `ModuleElement`                                                `getModuleElement​(CharSequence name)`                                                                         
          `Name`                                                         `getName​(CharSequence cs)`                                                                                    
          `PackageElement`                                               `getPackageElement​(CharSequence name)`                                                                        
          `PackageElement`                                               `getPackageElement​(ModuleElement module,                  CharSequence name)`                                 
          `PackageElement`                                               `getPackageOf​(Element type)`                                                                                  
          `TypeElement`                                                  `getTypeElement​(CharSequence name)`                                                                           
          `boolean`                                                      `hides​(Element hider,      Element hidden)`                                                                   
          `boolean`                                                      `isCompiledInCurrentRun​(Element element)`                                                                     
          `boolean`                                                      `isDeprecated​(Element e)`                                                                                     
          `boolean`                                                      `isFunctionalInterface​(TypeElement type)`                                                                     
          `boolean`                                                      `overrides​(ExecutableElement overrider,          ExecutableElement overridden,          TypeElement type)`    
          `void`                                                         `printElements​(Writer w,              Element... elements)`                                                   

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.javax.lang.model.util.Elements}

            ### Methods inherited from interface javax.lang.model.util.[Elements](http://docs.oracle.com/javase/7/docs/api/javax/lang/model/util/Elements.html?is-external=true "class or interface in javax.lang.model.util"){.externalLink}

            `getAllAnnotationMirrors, getAllMembers, getAllModuleElements, getAllPackageElements, getAllTypeElements, getBinaryName, getConstantExpression, getDocComment, getElementValuesWithDefaults, getModuleElement, getModuleOf, getName, getOrigin, getOrigin, getOrigin, getPackageElement, getPackageElement, getPackageOf, getTypeElement, getTypeElement, hides, isBridge, isDeprecated, isFunctionalInterface, overrides, printElements`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(javax.lang.model.util.Elements,javax.lang.model.util.Types,com.sun.source.util.Trees)}

        -   #### ElementsExtendedImpl

                public ElementsExtendedImpl​(Elements inner,
                                            Types types,
                                            com.sun.source.util.Trees trees)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getDeclaredMethods(javax.lang.model.element.TypeElement,java.lang.CharSequence)}

        -   #### getDeclaredMethods

            ``` methodSignature
            public List<ExecutableElement> getDeclaredMethods​(TypeElement owner,
                                                              CharSequence name)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDeclaredMethods` in interface `ElementsExtended`

        []{#getAllMethods(javax.lang.model.element.TypeElement,java.lang.CharSequence)}

        -   #### getAllMethods

            ``` methodSignature
            public List<ExecutableElement> getAllMethods​(TypeElement owner,
                                                         CharSequence name)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getAllMethods` in interface `ElementsExtended`

        []{#getBridgeMethods(javax.lang.model.element.TypeElement,java.lang.CharSequence)}

        -   #### getBridgeMethods

            ``` methodSignature
            public List<BridgeMethod> getBridgeMethods​(TypeElement owner,
                                                       CharSequence name)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBridgeMethods` in interface `ElementsExtended`

        []{#getImplementation(javax.lang.model.element.ExecutableElement,javax.lang.model.element.TypeElement)}

        -   #### getImplementation

            ``` methodSignature
            public ExecutableElement getImplementation​(ExecutableElement baseMethod,
                                                       TypeElement inType)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getImplementation` in interface `ElementsExtended`

        []{#getBinaryImplementationOwner(javax.lang.model.element.ExecutableElement,javax.lang.model.element.TypeElement)}

        -   #### getBinaryImplementationOwner

            ``` methodSignature
            public TypeElement getBinaryImplementationOwner​(ExecutableElement method,
                                                            TypeElement inType)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBinaryImplementationOwner` in
                interface `ElementsExtended`

        []{#getAllBridgeMethods(javax.lang.model.element.TypeElement)}

        -   #### getAllBridgeMethods

            ``` methodSignature
            public List<BridgeMethod> getAllBridgeMethods​(TypeElement type)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getAllBridgeMethods` in interface `ElementsExtended`

        []{#isCompiledInCurrentRun(javax.lang.model.element.Element)}

        -   #### isCompiledInCurrentRun

            ``` methodSignature
            public boolean isCompiledInCurrentRun​(Element element)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isCompiledInCurrentRun` in interface `ElementsExtended`

        []{#getPackageElement(java.lang.CharSequence)}

        -   #### getPackageElement

            ``` methodSignature
            public PackageElement getPackageElement​(CharSequence name)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPackageElement` in interface `Elements`

        []{#getPackageElement(javax.lang.model.element.ModuleElement,java.lang.CharSequence)}

        -   #### getPackageElement

            ``` methodSignature
            public PackageElement getPackageElement​(ModuleElement module,
                                                    CharSequence name)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPackageElement` in interface `Elements`

        []{#getAllPackageElements(java.lang.CharSequence)}

        -   #### getAllPackageElements

            ``` methodSignature
            public Set<? extends PackageElement> getAllPackageElements​(CharSequence name)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getAllPackageElements` in interface `Elements`

        []{#getTypeElement(java.lang.CharSequence)}

        -   #### getTypeElement

            ``` methodSignature
            public TypeElement getTypeElement​(CharSequence name)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTypeElement` in interface `Elements`

        []{#getModuleElement(java.lang.CharSequence)}

        -   #### getModuleElement

            ``` methodSignature
            public ModuleElement getModuleElement​(CharSequence name)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getModuleElement` in interface `Elements`

        []{#getAllModuleElements()}

        -   #### getAllModuleElements

            ``` methodSignature
            public Set<? extends ModuleElement> getAllModuleElements()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getAllModuleElements` in interface `Elements`

        []{#getElementValuesWithDefaults(javax.lang.model.element.AnnotationMirror)}

        -   #### getElementValuesWithDefaults

            ``` methodSignature
            public Map<? extends ExecutableElement,​? extends AnnotationValue> getElementValuesWithDefaults​(AnnotationMirror a)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getElementValuesWithDefaults` in interface `Elements`

        []{#getDocComment(javax.lang.model.element.Element)}

        -   #### getDocComment

            ``` methodSignature
            public String getDocComment​(Element e)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDocComment` in interface `Elements`

        []{#isDeprecated(javax.lang.model.element.Element)}

        -   #### isDeprecated

            ``` methodSignature
            public boolean isDeprecated​(Element e)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isDeprecated` in interface `Elements`

        []{#getBinaryName(javax.lang.model.element.TypeElement)}

        -   #### getBinaryName

            ``` methodSignature
            public Name getBinaryName​(TypeElement type)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBinaryName` in interface `Elements`

        []{#getPackageOf(javax.lang.model.element.Element)}

        -   #### getPackageOf

            ``` methodSignature
            public PackageElement getPackageOf​(Element type)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPackageOf` in interface `Elements`

        []{#getAllMembers(javax.lang.model.element.TypeElement)}

        -   #### getAllMembers

            ``` methodSignature
            public List<? extends Element> getAllMembers​(TypeElement type)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getAllMembers` in interface `Elements`

        []{#getAllAnnotationMirrors(javax.lang.model.element.Element)}

        -   #### getAllAnnotationMirrors

            ``` methodSignature
            public List<? extends AnnotationMirror> getAllAnnotationMirrors​(Element e)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getAllAnnotationMirrors` in interface `Elements`

        []{#hides(javax.lang.model.element.Element,javax.lang.model.element.Element)}

        -   #### hides

            ``` methodSignature
            public boolean hides​(Element hider,
                                 Element hidden)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `hides` in interface `Elements`

        []{#overrides(javax.lang.model.element.ExecutableElement,javax.lang.model.element.ExecutableElement,javax.lang.model.element.TypeElement)}

        -   #### overrides

            ``` methodSignature
            public boolean overrides​(ExecutableElement overrider,
                                     ExecutableElement overridden,
                                     TypeElement type)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `overrides` in interface `Elements`

        []{#getConstantExpression(java.lang.Object)}

        -   #### getConstantExpression

            ``` methodSignature
            public String getConstantExpression​(Object value)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getConstantExpression` in interface `Elements`

        []{#printElements(java.io.Writer,javax.lang.model.element.Element...)}

        -   #### printElements

            ``` methodSignature
            public void printElements​(Writer w,
                                      Element... elements)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `printElements` in interface `Elements`

        []{#getName(java.lang.CharSequence)}

        -   #### getName

            ``` methodSignature
            public Name getName​(CharSequence cs)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getName` in interface `Elements`

        []{#isFunctionalInterface(javax.lang.model.element.TypeElement)}

        -   #### isFunctionalInterface

            ``` methodSignature
            public boolean isFunctionalInterface​(TypeElement type)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isFunctionalInterface` in interface `Elements`
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
-   [Nested](#nested.class.summary) \| 
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

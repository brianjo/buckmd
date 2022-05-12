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

## Interface ElementsExtended {#interface-elementsextended .title title="Interface ElementsExtended"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `Elements`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `ElementsExtendedImpl`

    ------------------------------------------------------------------------

        public interface ElementsExtended
        extends Elements

    ::: block
    Wraps and extends
    [`Elements`](http://docs.oracle.com/javase/7/docs/api/javax/lang/model/util/Elements.html?is-external=true "class or interface in javax.lang.model.util"){.externalLink}
    with methods that cannot be added as pure extension methods on
    [`MoreElements`](MoreElements.html "class in com.facebook.buck.jvm.java.lang.model")
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
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type           Method                                                                                                     Description
          --------------------------- ---------------------------------------------------------------------------------------------------------- -------------
          `List<BridgeMethod>`        `getAllBridgeMethods​(TypeElement type)`                                                                     
          `List<ExecutableElement>`   `getAllMethods​(TypeElement owner,              CharSequence name)`                                          
          `TypeElement`               `getBinaryImplementationOwner​(ExecutableElement method,                             TypeElement inType)`    
          `List<BridgeMethod>`        `getBridgeMethods​(TypeElement owner,                 CharSequence name)`                                    
          `List<ExecutableElement>`   `getDeclaredMethods​(TypeElement owner,                   CharSequence name)`                                
          `ExecutableElement`         `getImplementation​(ExecutableElement method,                  TypeElement inType)`                          
          `boolean`                   `isCompiledInCurrentRun​(Element element)`                                                                   

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

        -   []{#methods.inherited.from.class.javax.lang.model.util.Elements}

            ### Methods inherited from interface javax.lang.model.util.[Elements](http://docs.oracle.com/javase/7/docs/api/javax/lang/model/util/Elements.html?is-external=true "class or interface in javax.lang.model.util"){.externalLink}

            `getAllAnnotationMirrors, getAllMembers, getAllModuleElements, getAllPackageElements, getAllTypeElements, getBinaryName, getConstantExpression, getDocComment, getElementValuesWithDefaults, getModuleElement, getModuleOf, getName, getOrigin, getOrigin, getOrigin, getPackageElement, getPackageElement, getPackageOf, getTypeElement, getTypeElement, hides, isBridge, isDeprecated, isFunctionalInterface, overrides, printElements`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getDeclaredMethods(javax.lang.model.element.TypeElement,java.lang.CharSequence)}

        -   #### getDeclaredMethods

            ``` methodSignature
            List<ExecutableElement> getDeclaredMethods​(TypeElement owner,
                                                       CharSequence name)
            ```

        []{#getAllMethods(javax.lang.model.element.TypeElement,java.lang.CharSequence)}

        -   #### getAllMethods

            ``` methodSignature
            List<ExecutableElement> getAllMethods​(TypeElement owner,
                                                  CharSequence name)
            ```

        []{#getBridgeMethods(javax.lang.model.element.TypeElement,java.lang.CharSequence)}

        -   #### getBridgeMethods

            ``` methodSignature
            List<BridgeMethod> getBridgeMethods​(TypeElement owner,
                                                CharSequence name)
            ```

        []{#getAllBridgeMethods(javax.lang.model.element.TypeElement)}

        -   #### getAllBridgeMethods

            ``` methodSignature
            List<BridgeMethod> getAllBridgeMethods​(TypeElement type)
            ```

        []{#getImplementation(javax.lang.model.element.ExecutableElement,javax.lang.model.element.TypeElement)}

        -   #### getImplementation

            ``` methodSignature
            ExecutableElement getImplementation​(ExecutableElement method,
                                                TypeElement inType)
            ```

        []{#getBinaryImplementationOwner(javax.lang.model.element.ExecutableElement,javax.lang.model.element.TypeElement)}

        -   #### getBinaryImplementationOwner

            ``` methodSignature
            TypeElement getBinaryImplementationOwner​(ExecutableElement method,
                                                     TypeElement inType)
            ```

        []{#isCompiledInCurrentRun(javax.lang.model.element.Element)}

        -   #### isCompiledInCurrentRun

            ``` methodSignature
            boolean isCompiledInCurrentRun​(Element element)
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
-   [Nested](#nested.class.summary) \| 
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

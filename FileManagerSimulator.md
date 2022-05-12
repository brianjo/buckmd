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

## Class FileManagerSimulator {#class-filemanagersimulator .title title="Class FileManagerSimulator"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.abi.source.FileManagerSimulator

::: description
-   

    ------------------------------------------------------------------------

        public class FileManagerSimulator
        extends Object

    ::: block
    Simulates the behavior of `javac`\'s file manager for source-only
    ABI classpaths.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                       Description
          --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `FileManagerSimulator​(Elements elements,                     com.sun.source.util.Trees trees,                     SourceOnlyAbiRuleInfoFactory.SourceOnlyAbiRuleInfo ruleInfo)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                              Description
          ------------------- --------------------------------------------------- -------------
          `String`            `getOwningTarget​(Element element)`                   
          `boolean`           `isCompiledInCurrentRun​(TypeElement typeElement)`    
          `boolean`           `typeWillBeAvailable​(TypeElement type)`              

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

        []{#<init>(javax.lang.model.util.Elements,com.sun.source.util.Trees,com.facebook.buck.jvm.java.abi.source.api.SourceOnlyAbiRuleInfoFactory.SourceOnlyAbiRuleInfo)}

        -   #### FileManagerSimulator

                public FileManagerSimulator​(Elements elements,
                                            com.sun.source.util.Trees trees,
                                            SourceOnlyAbiRuleInfoFactory.SourceOnlyAbiRuleInfo ruleInfo)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getOwningTarget(javax.lang.model.element.Element)}

        -   #### getOwningTarget

            ``` methodSignature
            public String getOwningTarget​(Element element)
            ```

        []{#typeWillBeAvailable(javax.lang.model.element.TypeElement)}

        -   #### typeWillBeAvailable

            ``` methodSignature
            public boolean typeWillBeAvailable​(TypeElement type)
            ```

        []{#isCompiledInCurrentRun(javax.lang.model.element.TypeElement)}

        -   #### isCompiledInCurrentRun

            ``` methodSignature
            public boolean isCompiledInCurrentRun​(TypeElement typeElement)
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

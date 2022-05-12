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
[Package]{.packageLabelInType} [com.facebook.buck.rules.modern.impl](package-summary.html)
:::

## Class OutputPathVisitor {#class-outputpathvisitor .title title="Class OutputPathVisitor"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.rules.modern.impl.AbstractValueVisitor](AbstractValueVisitor.html "class in com.facebook.buck.rules.modern.impl")\<[RuntimeException](http://docs.oracle.com/javase/7/docs/api/java/lang/RuntimeException.html?is-external=true "class or interface in java.lang"){.externalLink}\>

    -   -   com.facebook.buck.rules.modern.impl.OutputPathVisitor

::: description
-   

    All Implemented Interfaces:
    :   `ValueVisitor<RuntimeException>`

    ------------------------------------------------------------------------

        public class OutputPathVisitor
        extends AbstractValueVisitor<RuntimeException>

    ::: block
    Visits all the referenced OutputPaths.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                             Description
          ----------------------------------------------------------------------- -------------
          `OutputPathVisitor​(java.util.function.Consumer<OutputPath> consumer)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                Description
          ------------------- ------------------------------------- -------------
          `void`              `visitOutputPath​(OutputPath value)`    
          `void`              `visitPath​(Path path)`                 
          `void`              `visitSimple​(Object value)`            
          `void`              `visitSourcePath​(SourcePath value)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.rules.modern.impl.AbstractValueVisitor}

            ### Methods inherited from class com.facebook.buck.rules.modern.impl.[AbstractValueVisitor](AbstractValueVisitor.html "class in com.facebook.buck.rules.modern.impl")

            `visitBoolean, visitByte, visitCharacter, visitDouble, visitDynamic, visitField, visitFloat, visitInteger, visitList, visitLong, visitMap, visitNullable, visitOptional, visitSet, visitShort, visitSortedMap, visitSortedSet, visitString, visitTargetConfiguration`

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

        []{#<init>(java.util.function.Consumer)}

        -   #### OutputPathVisitor

                public OutputPathVisitor​(java.util.function.Consumer<OutputPath> consumer)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#visitOutputPath(com.facebook.buck.rules.modern.OutputPath)}

        -   #### visitOutputPath

            ``` methodSignature
            public void visitOutputPath​(OutputPath value)
            ```

        []{#visitSourcePath(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### visitSourcePath

            ``` methodSignature
            public void visitSourcePath​(SourcePath value)
            ```

        []{#visitSimple(java.lang.Object)}

        -   #### visitSimple

            ``` methodSignature
            public void visitSimple​(Object value)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `visitSimple` in
                class `AbstractValueVisitor<RuntimeException>`

        []{#visitPath(java.nio.file.Path)}

        -   #### visitPath

            ``` methodSignature
            public void visitPath​(Path path)
                           throws RuntimeException
            ```

            [Throws:]{.throwsLabel}
            :   `RuntimeException`
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

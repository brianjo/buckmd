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

## Class StubJar {#class-stubjar .title title="Class StubJar"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.abi.StubJar

::: description
-   

    ------------------------------------------------------------------------

        public class StubJar
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                  Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `StubJar​(Path toMirror)`                                                                                                                                                                                      
          `StubJar​(SourceVersion targetVersion,        ElementsExtended elements,        Types types,        Messager messager,        Iterable<Element> topLevelElements,        boolean includeParameterMetadata)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `StubJar`             | `setCompatibility     | ::: block             |
        |                       | Mode​(AbiGenerationMod | Filters the stub jar  |
        |                       | e compatibilityMode)` | through               |
        |                       |                       | [                     |
        |                       |                       | `SourceAbiCompatibleV |
        |                       |                       | isitor`](SourceAbiCom |
        |                       |                       | patibleVisitor.html " |
        |                       |                       | class in com.facebook |
        |                       |                       | .buck.jvm.java.abi"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `writeTo​(Projec       |                       |
        |                       | tFilesystem filesyste |                       |
        |                       | m,        Path path)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `writeTo​(Ja           |                       |
        |                       | rBuilder jarBuilder)` |                       |
        +-----------------------+-----------------------+-----------------------+

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

        []{#<init>(java.nio.file.Path)}

        -   #### StubJar

                public StubJar​(Path toMirror)

        []{#<init>(javax.lang.model.SourceVersion,com.facebook.buck.jvm.java.lang.model.ElementsExtended,javax.lang.model.util.Types,javax.annotation.processing.Messager,java.lang.Iterable,boolean)}

        -   #### StubJar

                public StubJar​(SourceVersion targetVersion,
                               ElementsExtended elements,
                               Types types,
                               Messager messager,
                               Iterable<Element> topLevelElements,
                               boolean includeParameterMetadata)

            [Parameters:]{.paramLabel}
            :   `targetVersion` - the class file version to output,
                expressed as the corresponding Java source version
            :   `types` -
            :   `messager` -
            :   `includeParameterMetadata` -
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#setCompatibilityMode(com.facebook.buck.jvm.java.abi.AbiGenerationMode)}

        -   #### setCompatibilityMode

            ``` methodSignature
            public StubJar setCompatibilityMode​(AbiGenerationMode compatibilityMode)
            ```

            ::: block
            Filters the stub jar through
            [`SourceAbiCompatibleVisitor`](SourceAbiCompatibleVisitor.html "class in com.facebook.buck.jvm.java.abi").
            See that class for details.
            :::

            [Parameters:]{.paramLabel}
            :   `compatibilityMode` -

        []{#writeTo(com.facebook.buck.io.filesystem.ProjectFilesystem,java.nio.file.Path)}

        -   #### writeTo

            ``` methodSignature
            public void writeTo​(ProjectFilesystem filesystem,
                                Path path)
                         throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#writeTo(com.facebook.buck.util.zip.JarBuilder)}

        -   #### writeTo

            ``` methodSignature
            public void writeTo​(JarBuilder jarBuilder)
                         throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`
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

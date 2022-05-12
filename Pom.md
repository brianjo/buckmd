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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.maven](package-summary.html)
:::

## Class Pom {#class-pom .title title="Class Pom"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.maven.Pom

::: description
-   

    ------------------------------------------------------------------------

        public class Pom
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                  Description
          -------------------------------------------------------------------------------------------- -------------
          `Pom​(SourcePathResolverAdapter pathResolver,    Path path,    MavenPublishable buildRule)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                Method                                                                                            Description
          -------------------------------- ------------------------------------------------------------------------------------------------- -------------
          `void`                           `flushToFile()`                                                                                    
          `static Path`                    `generatePomFile​(SourcePathResolverAdapter pathResolver,                MavenPublishable rule)`    
          `org.apache.maven.model.Model`   `getModel()`                                                                                       
          `Path`                           `getPath()`                                                                                        

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
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

        []{#<init>(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,java.nio.file.Path,com.facebook.buck.jvm.java.MavenPublishable)}

        -   #### Pom

                public Pom​(SourcePathResolverAdapter pathResolver,
                           Path path,
                           MavenPublishable buildRule)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#generatePomFile(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,com.facebook.buck.jvm.java.MavenPublishable)}

        -   #### generatePomFile

            ``` methodSignature
            public static Path generatePomFile​(SourcePathResolverAdapter pathResolver,
                                               MavenPublishable rule)
                                        throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#flushToFile()}

        -   #### flushToFile

            ``` methodSignature
            public void flushToFile()
                             throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getModel()}

        -   #### getModel

            ``` methodSignature
            public org.apache.maven.model.Model getModel()
            ```

        []{#getPath()}

        -   #### getPath

            ``` methodSignature
            public Path getPath()
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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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

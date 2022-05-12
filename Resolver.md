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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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

## Class Resolver {#class-resolver .title title="Class Resolver"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.maven.Resolver

::: description
-   

    ------------------------------------------------------------------------

        public class Resolver
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                               Description
          ------------------- ----------------------------------- -------------
          `static String`     `ARTIFACT_FILE_NAME_FORMAT`          
          `static String`     `ARTIFACT_FILE_NAME_REGEX_FORMAT`    
          `static String`     `VERSION_REGEX_GROUP`                

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                         Description
          ----------------------------------- -------------
          `Resolver​(ArtifactConfig config)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                    Description
          ------------------- ----------------------------------------- -------------
          `static void`       `main​(String[] args)`                      
          `void`              `resolve​(Collection<String> artifacts)`    

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
    -   []{#field.detail}

        ### Field Detail

        []{#ARTIFACT_FILE_NAME_FORMAT}

        -   #### ARTIFACT_FILE_NAME_FORMAT

                public static final String ARTIFACT_FILE_NAME_FORMAT

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.maven.Resolver.ARTIFACT_FILE_NAME_FORMAT)

        []{#ARTIFACT_FILE_NAME_REGEX_FORMAT}

        -   #### ARTIFACT_FILE_NAME_REGEX_FORMAT

                public static final String ARTIFACT_FILE_NAME_REGEX_FORMAT

        []{#VERSION_REGEX_GROUP}

        -   #### VERSION_REGEX_GROUP

                public static final String VERSION_REGEX_GROUP

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.maven.Resolver.VERSION_REGEX_GROUP)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.maven.ArtifactConfig)}

        -   #### Resolver

                public Resolver​(ArtifactConfig config)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#resolve(java.util.Collection)}

        -   #### resolve

            ``` methodSignature
            public void resolve​(Collection<String> artifacts)
                         throws org.eclipse.aether.RepositoryException,
                                ExecutionException,
                                InterruptedException,
                                IOException
            ```

            [Throws:]{.throwsLabel}
            :   `org.eclipse.aether.RepositoryException`
            :   `ExecutionException`
            :   `InterruptedException`
            :   `IOException`

        []{#main(java.lang.String[])}

        -   #### main

            ``` methodSignature
            public static void main​(String[] args)
                             throws org.kohsuke.args4j.CmdLineException,
                                    org.eclipse.aether.RepositoryException,
                                    IOException,
                                    ExecutionException,
                                    InterruptedException
            ```

            [Throws:]{.throwsLabel}
            :   `org.kohsuke.args4j.CmdLineException`
            :   `org.eclipse.aether.RepositoryException`
            :   `IOException`
            :   `ExecutionException`
            :   `InterruptedException`
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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

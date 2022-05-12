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

## Class ArtifactConfig {#class-artifactconfig .title title="Class ArtifactConfig"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.maven.ArtifactConfig

::: description
-   

    ------------------------------------------------------------------------

        public class ArtifactConfig
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type    Field              Description
          -------------------- ------------------ -------------
          `List<String>`       `artifacts`         
          `String`             `buckRepoRoot`      
          `String`             `mavenLocalRepo`    
          `List<Repository>`   `repositories`      
          `String`             `thirdParty`        
          `List<String>`       `visibility`        

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor          Description
          -------------------- -------------
          `ArtifactConfig()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type         Method                                                                        Description
          ------------------------- ----------------------------------------------------------------------------- -------------
          `static ArtifactConfig`   `fromCommandLineArgs​(String[] args)`                                           
          `ArtifactConfig`          `mergeCmdLineArgs​(com.facebook.buck.maven.ArtifactConfig.CmdLineArgs args)`    

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

        []{#repositories}

        -   #### repositories

                public List<Repository> repositories

        []{#artifacts}

        -   #### artifacts

                public List<String> artifacts

        []{#buckRepoRoot}

        -   #### buckRepoRoot

                public String buckRepoRoot

        []{#thirdParty}

        -   #### thirdParty

                public String thirdParty

        []{#mavenLocalRepo}

        -   #### mavenLocalRepo

                public String mavenLocalRepo

        []{#visibility}

        -   #### visibility

                public List<String> visibility
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### ArtifactConfig

                public ArtifactConfig()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#mergeCmdLineArgs(com.facebook.buck.maven.ArtifactConfig.CmdLineArgs)}

        -   #### mergeCmdLineArgs

            ``` methodSignature
            public ArtifactConfig mergeCmdLineArgs​(com.facebook.buck.maven.ArtifactConfig.CmdLineArgs args)
            ```

        []{#fromCommandLineArgs(java.lang.String[])}

        -   #### fromCommandLineArgs

            ``` methodSignature
            public static ArtifactConfig fromCommandLineArgs​(String[] args)
                                                      throws org.kohsuke.args4j.CmdLineException,
                                                             IOException
            ```

            [Throws:]{.throwsLabel}
            :   `org.kohsuke.args4j.CmdLineException`
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

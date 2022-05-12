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

## Class Publisher {#class-publisher .title title="Class Publisher"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.maven.Publisher

::: description
-   

    ------------------------------------------------------------------------

        public class Publisher
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                 Description
          ------------------- --------------------- -------------
          `static URL`        `MAVEN_CENTRAL`        
          `static String`     `MAVEN_CENTRAL_URL`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                    Description
          -------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `Publisher​(Path localRepoPath,          URL remoteRepoUrl,          Optional<String> username,          Optional<String> password,          boolean dryRun)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                                      Method                                                                                                                            Description
          -------------------------------------------------------------------------------------- --------------------------------------------------------------------------------------------------------------------------------- -------------
          `com.google.common.collect.ImmutableSet<org.eclipse.aether.deployment.DeployResult>`   `publish​(SourcePathResolverAdapter pathResolver,        com.google.common.collect.ImmutableSet<MavenPublishable> publishables)`    
          `org.eclipse.aether.deployment.DeployResult`                                           `publish​(String groupId,        String artifactId,        String version,        List<File> toPublish)`                            
          `org.eclipse.aether.deployment.DeployResult`                                           `publish​(List<org.eclipse.aether.artifact.Artifact> toPublish)`                                                                    
          `org.eclipse.aether.deployment.DeployResult`                                           `publish​(org.eclipse.aether.artifact.Artifact descriptor,        List<File> toPublish)`                                            

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
    -   []{#field.detail}

        ### Field Detail

        []{#MAVEN_CENTRAL_URL}

        -   #### MAVEN_CENTRAL_URL

                public static final String MAVEN_CENTRAL_URL

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.maven.Publisher.MAVEN_CENTRAL_URL)

        []{#MAVEN_CENTRAL}

        -   #### MAVEN_CENTRAL

                public static final URL MAVEN_CENTRAL
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.nio.file.Path,java.net.URL,java.util.Optional,java.util.Optional,boolean)}

        -   #### Publisher

                public Publisher​(Path localRepoPath,
                                 URL remoteRepoUrl,
                                 Optional<String> username,
                                 Optional<String> password,
                                 boolean dryRun)

            [Parameters:]{.paramLabel}
            :   `localRepoPath` - Typically obtained as
                [`ProjectFilesystem.getRootPath()`](../io/filesystem/ProjectFilesystem.html#getRootPath())
            :   `remoteRepoUrl` - Canonically
                [`MAVEN_CENTRAL_URL`](#MAVEN_CENTRAL_URL)
            :   `dryRun` - if true, a dummy `DeployResult` will be
                returned, with the fully constructed `DeployRequest`. No
                actual publishing will happen
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#publish(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,com.google.common.collect.ImmutableSet)}

        -   #### publish

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<org.eclipse.aether.deployment.DeployResult> publish​(SourcePathResolverAdapter pathResolver,
                                                                                                              com.google.common.collect.ImmutableSet<MavenPublishable> publishables)
                                                                                                       throws org.eclipse.aether.deployment.DeploymentException
            ```

            [Throws:]{.throwsLabel}
            :   `org.eclipse.aether.deployment.DeploymentException`

        []{#publish(java.lang.String,java.lang.String,java.lang.String,java.util.List)}

        -   #### publish

            ``` methodSignature
            public org.eclipse.aether.deployment.DeployResult publish​(String groupId,
                                                                      String artifactId,
                                                                      String version,
                                                                      List<File> toPublish)
                                                               throws org.eclipse.aether.deployment.DeploymentException
            ```

            [Throws:]{.throwsLabel}
            :   `org.eclipse.aether.deployment.DeploymentException`

        []{#publish(org.eclipse.aether.artifact.Artifact,java.util.List)}

        -   #### publish

            ``` methodSignature
            public org.eclipse.aether.deployment.DeployResult publish​(org.eclipse.aether.artifact.Artifact descriptor,
                                                                      List<File> toPublish)
                                                               throws org.eclipse.aether.deployment.DeploymentException
            ```

            [Parameters:]{.paramLabel}
            :   `descriptor` - an `Artifact`, holding the maven
                coordinates for the published files less the extension
                that is to be derived from the files. The `descriptor`
                itself will not be published as is, and the
                [`File`](http://docs.oracle.com/javase/7/docs/api/java/io/File.html?is-external=true "class or interface in java.io"){.externalLink}
                attached to it (if any) will be ignored.
            :   `toPublish` -
                [`File`](http://docs.oracle.com/javase/7/docs/api/java/io/File.html?is-external=true "class or interface in java.io"){.externalLink}(s)
                to be published using the given coordinates. The
                filename extension of each given file will be used as a
                maven \"extension\" coordinate

            [Throws:]{.throwsLabel}
            :   `org.eclipse.aether.deployment.DeploymentException`

        []{#publish(java.util.List)}

        -   #### publish

            ``` methodSignature
            public org.eclipse.aether.deployment.DeployResult publish​(List<org.eclipse.aether.artifact.Artifact> toPublish)
                                                               throws org.eclipse.aether.deployment.DeploymentException
            ```

            [Parameters:]{.paramLabel}
            :   `toPublish` - each `Artifact` must contain a file, that
                will be published under maven coordinates in the
                corresponding `Artifact`.

            [Throws:]{.throwsLabel}
            :   `org.eclipse.aether.deployment.DeploymentException`

            [See Also:]{.seeLabel}
            :   `Artifact.setFile(java.io.File)`
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

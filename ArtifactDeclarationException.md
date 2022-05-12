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

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../deprecated-list.html)
-   [Index](../../../../../index-all.html)
-   [Help](../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../allclasses.html)

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
-   Method

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
[Package]{.packageLabelInType} [com.facebook.buck.core.artifact](package-summary.html)
:::

## Class ArtifactDeclarationException {#class-artifactdeclarationexception .title title="Class ArtifactDeclarationException"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Throwable](http://docs.oracle.com/javase/7/docs/api/java/lang/Throwable.html?is-external=true "class or interface in java.lang"){.externalLink}

    -   -   [java.lang.Exception](http://docs.oracle.com/javase/7/docs/api/java/lang/Exception.html?is-external=true "class or interface in java.lang"){.externalLink}

        -   -   [java.lang.RuntimeException](http://docs.oracle.com/javase/7/docs/api/java/lang/RuntimeException.html?is-external=true "class or interface in java.lang"){.externalLink}

            -   -   [com.facebook.buck.core.exceptions.HumanReadableException](../exceptions/HumanReadableException.html "class in com.facebook.buck.core.exceptions")

                -   -   com.facebook.buck.core.artifact.ArtifactDeclarationException

::: description
-   

    All Implemented Interfaces:
    :   `ExceptionWithHumanReadableMessage`, `Serializable`

    ------------------------------------------------------------------------

        public class ArtifactDeclarationException
        extends HumanReadableException

    ::: block
    Represents a failure to declare an
    [`Artifact`](Artifact.html "interface in com.facebook.buck.core.artifact")
    :::

    [See Also:]{.seeLabel}
    :   [Serialized
        Form](../../../../../serialized-form.html#com.facebook.buck.core.artifact.ArtifactDeclarationException)
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                Description
          ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `ArtifactDeclarationException​(com.facebook.buck.core.artifact.ArtifactDeclarationException.Reason reason,                             BuildTarget buildTarget,                             String path)`    
          `ArtifactDeclarationException​(com.facebook.buck.core.artifact.ArtifactDeclarationException.Reason reason,                             BuildTarget buildTarget,                             Path path)`      

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        -   []{#methods.inherited.from.class.com.facebook.buck.core.exceptions.HumanReadableException}

            ### Methods inherited from class com.facebook.buck.core.exceptions.[HumanReadableException](../exceptions/HumanReadableException.html "class in com.facebook.buck.core.exceptions")

            `getDependencyStack, getHumanReadableErrorMessage`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Throwable}

            ### Methods inherited from class java.lang.[Throwable](http://docs.oracle.com/javase/7/docs/api/java/lang/Throwable.html?is-external=true "class or interface in java.lang"){.externalLink}

            `addSuppressed, fillInStackTrace, getCause, getLocalizedMessage, getMessage, getStackTrace, getSuppressed, initCause, printStackTrace, printStackTrace, printStackTrace, setStackTrace, toString`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.artifact.ArtifactDeclarationException.Reason,com.facebook.buck.core.model.BuildTarget,java.nio.file.Path)}

        -   #### ArtifactDeclarationException

                public ArtifactDeclarationException​(com.facebook.buck.core.artifact.ArtifactDeclarationException.Reason reason,
                                                    BuildTarget buildTarget,
                                                    Path path)

        []{#<init>(com.facebook.buck.core.artifact.ArtifactDeclarationException.Reason,com.facebook.buck.core.model.BuildTarget,java.lang.String)}

        -   #### ArtifactDeclarationException

                public ArtifactDeclarationException​(com.facebook.buck.core.artifact.ArtifactDeclarationException.Reason reason,
                                                    BuildTarget buildTarget,
                                                    String path)
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

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../deprecated-list.html)
-   [Index](../../../../../index-all.html)
-   [Help](../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../allclasses.html)

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
-   Method

</div>

[]{#skip.navbar.bottom}
:::

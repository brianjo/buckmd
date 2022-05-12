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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.common](package-summary.html)
:::

## Class RecordArtifactVerifier {#class-recordartifactverifier .title title="Class RecordArtifactVerifier"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.rules.common.RecordArtifactVerifier

::: description
-   

    All Implemented Interfaces:
    :   `BuildableContext`

    ------------------------------------------------------------------------

        public class RecordArtifactVerifier
        extends Object
        implements BuildableContext

    ::: block
    RecordArtifactVerifier can be used to ease the migration to
    ModernBuildRule. It will record a fixed set of artifacts and then
    act as a BuildableContext and verify that any further recorded
    artifacts are in the initial set (or children of an item in the
    set). This can be used at the top-level getBuildSteps() call to
    replace the BuildableContext.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                               Description
          --------------------------------------------------------------------------------------------------------- -------------
          `RecordArtifactVerifier​(Collection<Path> allowedPaths,                       BuildableContext context)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                  Description
          ------------------- --------------------------------------- -------------
          `Iterable<Path>`    `getPaths()`                             
          `void`              `recordArtifact​(Path pathToArtifact)`    

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

        []{#<init>(java.util.Collection,com.facebook.buck.core.build.buildable.context.BuildableContext)}

        -   #### RecordArtifactVerifier

                public RecordArtifactVerifier​(Collection<Path> allowedPaths,
                                              BuildableContext context)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#recordArtifact(java.nio.file.Path)}

        -   #### recordArtifact

            ``` methodSignature
            public void recordArtifact​(Path pathToArtifact)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `recordArtifact` in interface `BuildableContext`

            [See Also:]{.seeLabel}
            :   [`BuildInfoRecorder.recordArtifact(Path)`](../../build/engine/buildinfo/BuildInfoRecorder.html#recordArtifact(java.nio.file.Path))

        []{#getPaths()}

        -   #### getPaths

            ``` methodSignature
            public Iterable<Path> getPaths()
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

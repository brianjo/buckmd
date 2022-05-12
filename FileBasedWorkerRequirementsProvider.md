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
[Package]{.packageLabelInType} [com.facebook.buck.remoteexecution](package-summary.html)
:::

## Class FileBasedWorkerRequirementsProvider {#class-filebasedworkerrequirementsprovider .title title="Class FileBasedWorkerRequirementsProvider"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.remoteexecution.FileBasedWorkerRequirementsProvider

::: description
-   

    All Implemented Interfaces:
    :   `WorkerRequirementsProvider`

    ------------------------------------------------------------------------

        public final class FileBasedWorkerRequirementsProvider
        extends Object
        implements WorkerRequirementsProvider

    ::: block
    Provides rule\'s RE worker requirements based on JSON file
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                                                     Field                         Description
          --------------------------------------------------------------------- ----------------------------- -------------
          `static com.facebook.buck.remoteexecution.proto.WorkerRequirements`   `DONT_RETRY_ON_OOM_DEFAULT`    
          `static com.facebook.buck.remoteexecution.proto.WorkerRequirements`   `RETRY_ON_OOM_DEFAULT`         

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                           Description
          --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `FileBasedWorkerRequirementsProvider​(ProjectFilesystem projectFilesystem,                                    String workerRequirementsFilename,                                    boolean tryLargerWorkerOnOom,                                    int cacheSize)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.facebook.buck    | `r                    | ::: block             |
        | .remoteexecution.prot | esolveRequirements​(Bu | Resolve rule\'s       |
        | o.WorkerRequirements` | ildTarget target,     | worker requirements.  |
        |                       |                 Strin | :::                   |
        |                       | g auxiliaryBuildTag)` |                       |
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
    -   []{#field.detail}

        ### Field Detail

        []{#RETRY_ON_OOM_DEFAULT}

        -   #### RETRY_ON_OOM_DEFAULT

                public static final com.facebook.buck.remoteexecution.proto.WorkerRequirements RETRY_ON_OOM_DEFAULT

        []{#DONT_RETRY_ON_OOM_DEFAULT}

        -   #### DONT_RETRY_ON_OOM_DEFAULT

                public static final com.facebook.buck.remoteexecution.proto.WorkerRequirements DONT_RETRY_ON_OOM_DEFAULT
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.io.filesystem.ProjectFilesystem,java.lang.String,boolean,int)}

        -   #### FileBasedWorkerRequirementsProvider

                public FileBasedWorkerRequirementsProvider​(ProjectFilesystem projectFilesystem,
                                                           String workerRequirementsFilename,
                                                           boolean tryLargerWorkerOnOom,
                                                           int cacheSize)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#resolveRequirements(com.facebook.buck.core.model.BuildTarget,java.lang.String)}

        -   #### resolveRequirements

            ``` methodSignature
            public com.facebook.buck.remoteexecution.proto.WorkerRequirements resolveRequirements​(BuildTarget target,
                                                                                                  String auxiliaryBuildTag)
            ```

            ::: block
            Resolve rule\'s worker requirements.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `resolveRequirements` in
                interface `WorkerRequirementsProvider`

            [Parameters:]{.paramLabel}
            :   `target` - build target
            :   `auxiliaryBuildTag` - auxiliary tag capturing any custom
                configurations

            [Returns:]{.returnLabel}\
            [See Also:]{.seeLabel}
            :   `based on JSON file,      otherwise @see      com.facebook.buck.remoteexecution.FileBasedWorkerRequirementsProvider.DEFAULT`
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

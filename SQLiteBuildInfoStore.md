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
[Package]{.packageLabelInType} [com.facebook.buck.core.build.engine.buildinfo](package-summary.html)
:::

## Class SQLiteBuildInfoStore {#class-sqlitebuildinfostore .title title="Class SQLiteBuildInfoStore"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.build.engine.buildinfo.SQLiteBuildInfoStore

::: description
-   

    All Implemented Interfaces:
    :   `BuildInfoStore`, `Closeable`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class SQLiteBuildInfoStore
        extends Object
        implements BuildInfoStore
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                            Description
          ------------------------------------------------------ -------------
          `SQLiteBuildInfoStore​(ProjectFilesystem filesystem)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                         Method                                                                                 Description
          --------------------------------------------------------- -------------------------------------------------------------------------------------- -------------
          `void`                                                    `close()`                                                                               
          `void`                                                    `deleteMetadata​(BuildTarget buildTarget)`                                               
          `com.google.common.collect.ImmutableMap<String,​String>`   `getAllMetadata​(BuildTarget buildTarget)`                                               
          `Optional<String>`                                        `readMetadata​(BuildTarget buildTarget,             String key)`                         
          `void`                                                    `updateMetadata​(BuildTarget buildTarget,               Map<String,​String> metadata)`    

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

        []{#<init>(com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### SQLiteBuildInfoStore

                public SQLiteBuildInfoStore​(ProjectFilesystem filesystem)
                                     throws IOException

            [Throws:]{.throwsLabel}
            :   `IOException`
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#close()}

        -   #### close

            ``` methodSignature
            public void close()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `BuildInfoStore`

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `Closeable`

        []{#readMetadata(com.facebook.buck.core.model.BuildTarget,java.lang.String)}

        -   #### readMetadata

            ``` methodSignature
            public Optional<String> readMetadata​(BuildTarget buildTarget,
                                                 String key)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `readMetadata` in interface `BuildInfoStore`

        []{#getAllMetadata(com.facebook.buck.core.model.BuildTarget)}

        -   #### getAllMetadata

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​String> getAllMetadata​(BuildTarget buildTarget)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getAllMetadata` in interface `BuildInfoStore`

        []{#updateMetadata(com.facebook.buck.core.model.BuildTarget,java.util.Map)}

        -   #### updateMetadata

            ``` methodSignature
            public void updateMetadata​(BuildTarget buildTarget,
                                       Map<String,​String> metadata)
                                throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `updateMetadata` in interface `BuildInfoStore`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#deleteMetadata(com.facebook.buck.core.model.BuildTarget)}

        -   #### deleteMetadata

            ``` methodSignature
            public void deleteMetadata​(BuildTarget buildTarget)
                                throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `deleteMetadata` in interface `BuildInfoStore`

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

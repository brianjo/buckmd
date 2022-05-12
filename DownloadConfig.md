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
[Package]{.packageLabelInType} [com.facebook.buck.file.downloader.impl](package-summary.html)
:::

## Class DownloadConfig {#class-downloadconfig .title title="Class DownloadConfig"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.file.downloader.impl.DownloadConfig

::: description
-   

    ------------------------------------------------------------------------

        public class DownloadConfig
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                             Description
          --------------------------------------- -------------
          `DownloadConfig​(BuckConfig delegate)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                         Method                              Description
          --------------------------------------------------------- ----------------------------------- -------------
          `com.google.common.collect.ImmutableMap<String,​String>`   `getAllMavenRepos()`                 
          `Optional<String>`                                        `getMavenRepo()`                     
          `OptionalInt`                                             `getMaxNumberOfRetries()`            
          `Optional<Proxy>`                                         `getProxy()`                         
          `Optional<PasswordAuthentication>`                        `getRepoCredentials​(String repo)`    
          `boolean`                                                 `isDownloadAtRuntimeOk()`            

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

        []{#<init>(com.facebook.buck.core.config.BuckConfig)}

        -   #### DownloadConfig

                public DownloadConfig​(BuckConfig delegate)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getProxy()}

        -   #### getProxy

            ``` methodSignature
            public Optional<Proxy> getProxy()
            ```

        []{#getMavenRepo()}

        -   #### getMavenRepo

            ``` methodSignature
            public Optional<String> getMavenRepo()
            ```

        []{#getAllMavenRepos()}

        -   #### getAllMavenRepos

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​String> getAllMavenRepos()
            ```

        []{#isDownloadAtRuntimeOk()}

        -   #### isDownloadAtRuntimeOk

            ``` methodSignature
            public boolean isDownloadAtRuntimeOk()
            ```

        []{#getRepoCredentials(java.lang.String)}

        -   #### getRepoCredentials

            ``` methodSignature
            public Optional<PasswordAuthentication> getRepoCredentials​(String repo)
            ```

        []{#getMaxNumberOfRetries()}

        -   #### getMaxNumberOfRetries

            ``` methodSignature
            public OptionalInt getMaxNumberOfRetries()
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

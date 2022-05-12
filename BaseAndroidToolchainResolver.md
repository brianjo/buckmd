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
[Package]{.packageLabelInType} [com.facebook.buck.android.toolchain.common](package-summary.html)
:::

## Class BaseAndroidToolchainResolver {#class-baseandroidtoolchainresolver .title title="Class BaseAndroidToolchainResolver"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.toolchain.common.BaseAndroidToolchainResolver

::: description
-   

    Direct Known Subclasses:
    :   `AndroidNdkResolver`, `AndroidSdkDirectoryResolver`

    ------------------------------------------------------------------------

        public class BaseAndroidToolchainResolver
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                                                   Field                                  Description
          ------------------------------------------------------------------- -------------------------------------- -------------
          `protected com.google.common.collect.ImmutableMap<String,​String>`   `environment`                           
          `protected FileSystem`                                              `fileSystem`                            
          `static String`                                                     `INVALID_DIRECTORY_MESSAGE_TEMPLATE`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                                                                                                                                            Description
          -------------- ------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `protected `   `BaseAndroidToolchainResolver​(FileSystem fileSystem,                             com.google.common.collect.ImmutableMap<String,​String> environment)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                           Method                                                                                                       Description
          ------------------------------------------- ------------------------------------------------------------------------------------------------------------ -------------
          `protected Optional<Path>`                  `findFirstDirectory​(com.google.common.collect.ImmutableList<Pair<String,​Optional<String>>> possiblePaths)`    
          `protected Pair<String,​Optional<String>>`   `getEnvironmentVariable​(String key)`                                                                          

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

        []{#INVALID_DIRECTORY_MESSAGE_TEMPLATE}

        -   #### INVALID_DIRECTORY_MESSAGE_TEMPLATE

                public static final String INVALID_DIRECTORY_MESSAGE_TEMPLATE

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.android.toolchain.common.BaseAndroidToolchainResolver.INVALID_DIRECTORY_MESSAGE_TEMPLATE)

        []{#fileSystem}

        -   #### fileSystem

                protected final FileSystem fileSystem

        []{#environment}

        -   #### environment

                protected final com.google.common.collect.ImmutableMap<String,​String> environment
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.nio.file.FileSystem,com.google.common.collect.ImmutableMap)}

        -   #### BaseAndroidToolchainResolver

                protected BaseAndroidToolchainResolver​(FileSystem fileSystem,
                                                       com.google.common.collect.ImmutableMap<String,​String> environment)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#findFirstDirectory(com.google.common.collect.ImmutableList)}

        -   #### findFirstDirectory

            ``` methodSignature
            protected Optional<Path> findFirstDirectory​(com.google.common.collect.ImmutableList<Pair<String,​Optional<String>>> possiblePaths)
            ```

        []{#getEnvironmentVariable(java.lang.String)}

        -   #### getEnvironmentVariable

            ``` methodSignature
            protected Pair<String,​Optional<String>> getEnvironmentVariable​(String key)
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

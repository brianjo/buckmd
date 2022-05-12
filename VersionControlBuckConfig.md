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
[Package]{.packageLabelInType} [com.facebook.buck.util.versioncontrol](package-summary.html)
:::

## Class VersionControlBuckConfig {#class-versioncontrolbuckconfig .title title="Class VersionControlBuckConfig"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.versioncontrol.VersionControlBuckConfig

::: description
-   

    ------------------------------------------------------------------------

        public class VersionControlBuckConfig
        extends Object

    ::: block
    \* Provides simplified access to settings from the version_control
    section of a .buckconfig file.
    Available keys:

    generate_statistics: - Enable or disable the generation of version
    control statistics - Default value is false. - Currently only
    Mercurial is supported. hg_cmd: - Override the default Mercurial
    command used when generating statistics. - Default value is hg

    Example config section:

    \[version_control\] hg_cmd = hg3 generate_statistics = true
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                       Description
          ------------------------------------------------- -------------
          `VersionControlBuckConfig​(BuckConfig delegate)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                           Method                                   Description
          --------------------------------------------------------------------------- ---------------------------------------- -------------
          `String`                                                                    `getHgCmd()`                              
          `Optional<com.facebook.buck.util.versioncontrol.FastVersionControlStats>`   `getPregeneratedVersionControlStats()`    
          `boolean`                                                                   `shouldGenerateStatistics()`              

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

        -   #### VersionControlBuckConfig

                public VersionControlBuckConfig​(BuckConfig delegate)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getHgCmd()}

        -   #### getHgCmd

            ``` methodSignature
            public String getHgCmd()
            ```

        []{#shouldGenerateStatistics()}

        -   #### shouldGenerateStatistics

            ``` methodSignature
            public boolean shouldGenerateStatistics()
            ```

        []{#getPregeneratedVersionControlStats()}

        -   #### getPregeneratedVersionControlStats

            ``` methodSignature
            public Optional<com.facebook.buck.util.versioncontrol.FastVersionControlStats> getPregeneratedVersionControlStats()
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
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

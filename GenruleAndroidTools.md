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
[Package]{.packageLabelInType} [com.facebook.buck.shell](package-summary.html)
:::

## Class GenruleAndroidTools {#class-genruleandroidtools .title title="Class GenruleAndroidTools"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.shell.GenruleAndroidTools

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`

    ------------------------------------------------------------------------

        public abstract class GenruleAndroidTools
        extends Object
        implements AddsToRuleKey

    ::: block
    Immutable class for holding Android paths and tools, for use in
    [`GenruleBuildable`](GenruleBuildable.html "class in com.facebook.buck.shell").
    Note that, despite implementing AddsToRuleKey, GenruleAndroidTools
    does not actually contribute to rule keys. The reason for this is
    that all of the Path objects contained in this object are paths
    outside of the repository. GenruleAndroidTools is never serialized
    due to other logic in
    [`GenruleBuildable`](GenruleBuildable.html "class in com.facebook.buck.shell")
    that prevents it from happening; it is a logic error to serialize
    this class across a
    [`ModernBuildRule`](../rules/modern/ModernBuildRule.html "class in com.facebook.buck.rules.modern")
    boundary.

    This class still must implement AddsToRuleKey because
    ModernBuildRule requires that all fields in a
    [`Buildable`](../rules/modern/Buildable.html "interface in com.facebook.buck.rules.modern")
    must implement AddsToRuleKey so that a serializer can be derived.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor               Description
          ------------------------- -------------
          `GenruleAndroidTools()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `abstract Tool`       | `getAapt2Tool()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Tool`       | `getAaptTool()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abs                  | `get                  |                       |
        | tract Optional<Path>` | AndroidNdkLocation()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Path`       | `                     |                       |
        |                       | getAndroidPathToDx()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Path`       | `getAnd               |                       |
        |                       | roidPathToZipalign()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Path`       | `get                  |                       |
        |                       | AndroidSdkLocation()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `of​(AndroidTools      | ::: block             |
        |  GenruleAndroidTools` | tools,   BuildTarget  | Extracts a set of     |
        |                       | target,   BuildRuleRe | Android tools for a   |
        |                       | solver ruleResolver)` | particular build      |
        |                       |                       | using that build\'s   |
        |                       |                       | target and rule       |
        |                       |                       | resolver.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
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

        []{#<init>()}

        -   #### GenruleAndroidTools

                public GenruleAndroidTools()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getAndroidSdkLocation()}

        -   #### getAndroidSdkLocation

            ``` methodSignature
            public abstract Path getAndroidSdkLocation()
            ```

        []{#getAndroidPathToDx()}

        -   #### getAndroidPathToDx

            ``` methodSignature
            public abstract Path getAndroidPathToDx()
            ```

        []{#getAndroidPathToZipalign()}

        -   #### getAndroidPathToZipalign

            ``` methodSignature
            public abstract Path getAndroidPathToZipalign()
            ```

        []{#getAaptTool()}

        -   #### getAaptTool

            ``` methodSignature
            public abstract Tool getAaptTool()
            ```

        []{#getAapt2Tool()}

        -   #### getAapt2Tool

            ``` methodSignature
            public abstract Tool getAapt2Tool()
            ```

        []{#getAndroidNdkLocation()}

        -   #### getAndroidNdkLocation

            ``` methodSignature
            public abstract Optional<Path> getAndroidNdkLocation()
            ```

        []{#of(com.facebook.buck.android.toolchain.AndroidTools,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### of

            ``` methodSignature
            public static GenruleAndroidTools of​(AndroidTools tools,
                                                 BuildTarget target,
                                                 BuildRuleResolver ruleResolver)
            ```

            ::: block
            Extracts a set of Android tools for a particular build using
            that build\'s target and rule resolver. This is done here is
            instead of within the GenruleBuildable because Buildables
            don\'t have access to rule resolvers, and one is used here
            to look up the Tool for aapt2. In general Genrule probably
            shouldn\'t know about Android, but for the moment it does.
            :::

            [Parameters:]{.paramLabel}
            :   `tools` - Tools reference for Android
            :   `target` - The BuildTarget to retrieve tools for
            :   `ruleResolver` - Rule resolver for resolving tool
                referenves
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

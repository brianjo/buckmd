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
[Package]{.packageLabelInType} [com.facebook.buck.skylark.parser](package-summary.html)
:::

## Class ParseResult {#class-parseresult .title title="Class ParseResult"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.skylark.parser.ParseResult

::: description
-   

    ------------------------------------------------------------------------

        public abstract class ParseResult
        extends Object

    ::: block
    Parse result containing build/package rules and package defined in
    build or package files and supporting metadata.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor       Description
          ----------------- -------------
          `ParseResult()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `abstra               | `getGlob              |                       |
        | ct com.google.common. | ManifestWithResult()` |                       |
        | collect.ImmutableList |                       |                       |
        | <GlobSpecWithResult>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract com.g       | `getLoadedPaths()`    | ::: block             |
        | oogle.common.collect. |                       | Returns a set of      |
        | ImmutableSet<String>` |                       | extension paths that  |
        |                       |                       | were loaded           |
        |                       |                       | explicitly or         |
        |                       |                       | transitively when     |
        |                       |                       | parsing current build |
        |                       |                       | or package file.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abst                 | `getPackage()`        | ::: block             |
        | ract PackageMetadata` |                       | Contains the package  |
        |                       |                       | defined in a package  |
        |                       |                       | file.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract com         | `getRawRules()`       | ::: block             |
        | .google.common.collec |                       | Returns rules         |
        | t.ImmutableMap<String |                       | organized in a map    |
        | ,​Map<String,​Object>>` |                       | where a key is a rule |
        |                       |                       | name and the value is |
        |                       |                       | a map with keys       |
        |                       |                       | representing rule     |
        |                       |                       | parameters and values |
        |                       |                       | representing rule     |
        |                       |                       | arguments.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract com.go      | `getReadCo            | ::: block             |
        | ogle.common.collect.I | nfigurationOptions()` | Returns all           |
        | mmutableMap<String,​co |                       | configuration options |
        | m.google.common.colle |                       | accessed during       |
        | ct.ImmutableMap<Strin |                       | parsing of the build  |
        | g,​Optional<String>>>` |                       | or package file.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

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

        -   #### ParseResult

                public ParseResult()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getPackage()}

        -   #### getPackage

            ``` methodSignature
            public abstract PackageMetadata getPackage()
            ```

            ::: block
            Contains the package defined in a package file.
            :::

        []{#getRawRules()}

        -   #### getRawRules

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableMap<String,​Map<String,​Object>> getRawRules()
            ```

            ::: block
            Returns rules organized in a map where a key is a rule name
            and the value is a map with keys representing rule
            parameters and values representing rule arguments.
            For example {\"name\": \"my_rule\", \...}
            :::

        []{#getLoadedPaths()}

        -   #### getLoadedPaths

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSet<String> getLoadedPaths()
            ```

            ::: block
            Returns a set of extension paths that were loaded explicitly
            or transitively when parsing current build or package file.
            :::

        []{#getReadConfigurationOptions()}

        -   #### getReadConfigurationOptions

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableMap<String,​com.google.common.collect.ImmutableMap<String,​Optional<String>>> getReadConfigurationOptions()
            ```

            ::: block
            Returns all configuration options accessed during parsing of
            the build or package file.
            The schema is section-\>key-\>value
            :::

        []{#getGlobManifestWithResult()}

        -   #### getGlobManifestWithResult

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<GlobSpecWithResult> getGlobManifestWithResult()
            ```

            [Returns:]{.returnLabel}
            :   A list of
                [`GlobSpec`](../io/GlobSpec.html "class in com.facebook.buck.skylark.io")
                with the corresponding set of expanded paths.
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

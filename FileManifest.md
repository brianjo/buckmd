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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.parser.api](package-summary.html)
:::

## Interface FileManifest {#interface-filemanifest .title title="Interface FileManifest"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `BuildFileManifest`, `PackageFileManifest`

    ------------------------------------------------------------------------

        public interface FileManifest

    ::: block
    The
    [`FileManifest`](FileManifest.html "interface in com.facebook.buck.parser.api")
    output as a result of parsing a file with a
    [`FileParser`](FileParser.html "interface in com.facebook.buck.parser.api").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                             Method            Description
          ----------------------------------------------------------------------------- ----------------- -------------
          `com.google.common.collect.ImmutableMap<String,​Object>`                       `getConfigs()`     
          `Optional<com.google.common.collect.ImmutableMap<String,​Optional<String>>>`   `getEnv()`         
          `com.google.common.collect.ImmutableList<ParsingError>`                       `getErrors()`      
          `com.google.common.collect.ImmutableSortedSet<String>`                        `getIncludes()`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getIncludes()}

        -   #### getIncludes

            ``` methodSignature
            com.google.common.collect.ImmutableSortedSet<String> getIncludes()
            ```

            [Returns:]{.returnLabel}
            :   a set of extension files read during parsing.

        []{#getConfigs()}

        -   #### getConfigs

            ``` methodSignature
            com.google.common.collect.ImmutableMap<String,​Object> getConfigs()
            ```

            [Returns:]{.returnLabel}
            :   a map from configuration section to configuration key to
                the value returned during parsing.

        []{#getEnv()}

        -   #### getEnv

            ``` methodSignature
            Optional<com.google.common.collect.ImmutableMap<String,​Optional<String>>> getEnv()
            ```

            [Returns:]{.returnLabel}
            :   an optional map from environment variable to a value
                read during parsing (if any).

        []{#getErrors()}

        -   #### getErrors

            ``` methodSignature
            com.google.common.collect.ImmutableList<ParsingError> getErrors()
            ```

            [Returns:]{.returnLabel}
            :   A list of fatal errors occurred during parsing a file,
                i.e. errors that might render manifest incomplete. It is
                up for the parser to decide if still wants to fill this
                object with unaffected targets
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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

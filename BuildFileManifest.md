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
[Package]{.packageLabelInType} [com.facebook.buck.parser.api](package-summary.html)
:::

## Class BuildFileManifest {#class-buildfilemanifest .title title="Class BuildFileManifest"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.parser.api.BuildFileManifest

::: description
-   

    All Implemented Interfaces:
    :   `ComputeResult`, `FileManifest`

    ------------------------------------------------------------------------

        public abstract class BuildFileManifest
        extends Object
        implements ComputeResult, FileManifest

    ::: block
    Describes the content of a build file, which includes defined
    targets and their metadata.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor             Description
          ----------------------- -------------
          `BuildFileManifest()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                                                                 Method                                                                                                                                                                                                                                                                                                                                                                                                                                                                              Description
          ----------------------------------------------------------------------------------------------------------------- ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `abstract com.google.common.collect.ImmutableMap<String,​Object>`                                                  `getConfigs()`                                                                                                                                                                                                                                                                                                                                                                                                                                                                       
          `abstract Optional<com.google.common.collect.ImmutableMap<String,​Optional<String>>>`                              `getEnv()`                                                                                                                                                                                                                                                                                                                                                                                                                                                                           
          `abstract com.google.common.collect.ImmutableList<ParsingError>`                                                  `getErrors()`                                                                                                                                                                                                                                                                                                                                                                                                                                                                        
          `abstract com.google.common.collect.ImmutableList<GlobSpecWithResult>`                                            `getGlobManifest()`                                                                                                                                                                                                                                                                                                                                                                                                                                                                  
          `abstract com.google.common.collect.ImmutableSortedSet<String>`                                                   `getIncludes()`                                                                                                                                                                                                                                                                                                                                                                                                                                                                      
          `abstract com.google.common.collect.ImmutableMap<String,​com.google.common.collect.ImmutableMap<String,​Object>>`   `getTargets()`                                                                                                                                                                                                                                                                                                                                                                                                                                                                       
          `static BuildFileManifest`                                                                                        `of​(com.google.common.collect.ImmutableMap<String,​com.google.common.collect.ImmutableMap<String,​Object>> targets,   com.google.common.collect.ImmutableSortedSet<String> includes,   com.google.common.collect.ImmutableMap<String,​Object> configs,   Optional<com.google.common.collect.ImmutableMap<String,​Optional<String>>> env,   com.google.common.collect.ImmutableList<GlobSpecWithResult> globManifest,   com.google.common.collect.ImmutableList<ParsingError> errors)`    

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

        -   #### BuildFileManifest

                public BuildFileManifest()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getTargets()}

        -   #### getTargets

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableMap<String,​com.google.common.collect.ImmutableMap<String,​Object>> getTargets()
            ```

            [Returns:]{.returnLabel}
            :   a list of targets defined in the build file.

        []{#getIncludes()}

        -   #### getIncludes

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSortedSet<String> getIncludes()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getIncludes` in interface `FileManifest`

            [Returns:]{.returnLabel}
            :   a set of extension files read during parsing.

        []{#getConfigs()}

        -   #### getConfigs

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableMap<String,​Object> getConfigs()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getConfigs` in interface `FileManifest`

            [Returns:]{.returnLabel}
            :   a map from configuration section to configuration key to
                the value returned during parsing.

        []{#getEnv()}

        -   #### getEnv

            ``` methodSignature
            public abstract Optional<com.google.common.collect.ImmutableMap<String,​Optional<String>>> getEnv()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getEnv` in interface `FileManifest`

            [Returns:]{.returnLabel}
            :   an optional map from environment variable to a value
                read during parsing (if any).

        []{#getGlobManifest()}

        -   #### getGlobManifest

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<GlobSpecWithResult> getGlobManifest()
            ```

            [Returns:]{.returnLabel}
            :   A list of the glob operations performed with their
                results.

        []{#getErrors()}

        -   #### getErrors

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<ParsingError> getErrors()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getErrors` in interface `FileManifest`

            [Returns:]{.returnLabel}
            :   A list of fatal errors occurred during parsing a file,
                i.e. errors that might render manifest incomplete. It is
                up for the parser to decide if still wants to fill this
                object with unaffected targets

        []{#of(com.google.common.collect.ImmutableMap,com.google.common.collect.ImmutableSortedSet,com.google.common.collect.ImmutableMap,java.util.Optional,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableList)}

        -   #### of

            ``` methodSignature
            public static BuildFileManifest of​(com.google.common.collect.ImmutableMap<String,​com.google.common.collect.ImmutableMap<String,​Object>> targets,
                                               com.google.common.collect.ImmutableSortedSet<String> includes,
                                               com.google.common.collect.ImmutableMap<String,​Object> configs,
                                               Optional<com.google.common.collect.ImmutableMap<String,​Optional<String>>> env,
                                               com.google.common.collect.ImmutableList<GlobSpecWithResult> globManifest,
                                               com.google.common.collect.ImmutableList<ParsingError> errors)
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

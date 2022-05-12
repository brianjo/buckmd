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
[Package]{.packageLabelInType} [com.facebook.buck.parser.api](package-summary.html)
:::

## Class PackageFileManifest {#class-packagefilemanifest .title title="Class PackageFileManifest"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.parser.api.PackageFileManifest

::: description
-   

    All Implemented Interfaces:
    :   `ComputeResult`, `FileManifest`

    ------------------------------------------------------------------------

        public abstract class PackageFileManifest
        extends Object
        implements ComputeResult, FileManifest

    ::: block
    Describes the content of a package file, which includes a package
    definition and their metadata.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Field                 | Description           |
        +=======================+=======================+=======================+
        | `static               | `EMPTY_SINGLETON`     | ::: block             |
        |  PackageFileManifest` |                       | A singleton instance  |
        |                       |                       | of a manifest with an |
        |                       |                       | empty package         |
        |                       |                       | metadata.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor               Description
          ------------------------- -------------
          `PackageFileManifest()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `                     | `getConfigs()`        |                       |
        | abstract com.google.c |                       |                       |
        | ommon.collect.Immutab |                       |                       |
        | leMap<String,​Object>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Optional<co | `getEnv()`            |                       |
        | m.google.common.colle |                       |                       |
        | ct.ImmutableMap<Strin |                       |                       |
        | g,​Optional<String>>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getErrors()`         |                       |
        | abstract com.google.c |                       |                       |
        | ommon.collect.Immutab |                       |                       |
        | leList<ParsingError>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract com.google. | `getIncludes()`       |                       |
        | common.collect.Immuta |                       |                       |
        | bleSortedSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abst                 | `getPackage()`        | ::: block             |
        | ract PackageMetadata` |                       | Contains the package  |
        |                       |                       | defined in the build  |
        |                       |                       | file.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `of​(PackageMe         |                       |
        |  PackageFileManifest` | tadata getPackage,    |                       |
        |                       | com.google.common.col |                       |
        |                       | lect.ImmutableSortedS |                       |
        |                       | et<String> includes,  |                       |
        |                       |   com.google.common.c |                       |
        |                       | ollect.ImmutableMap<S |                       |
        |                       | tring,​Object> configs |                       |
        |                       | ,   Optional<com.goog |                       |
        |                       | le.common.collect.Imm |                       |
        |                       | utableMap<String,​Opti |                       |
        |                       | onal<String>>> env,   |                       |
        |                       |  com.google.common.co |                       |
        |                       | llect.ImmutableList<P |                       |
        |                       | arsingError> errors)` |                       |
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
    -   []{#field.detail}

        ### Field Detail

        []{#EMPTY_SINGLETON}

        -   #### EMPTY_SINGLETON

                public static final PackageFileManifest EMPTY_SINGLETON

            ::: block
            A singleton instance of a manifest with an empty package
            metadata.
            :::
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### PackageFileManifest

                public PackageFileManifest()
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
            Contains the package defined in the build file.
            :::

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

        []{#of(com.facebook.buck.parser.api.PackageMetadata,com.google.common.collect.ImmutableSortedSet,com.google.common.collect.ImmutableMap,java.util.Optional,com.google.common.collect.ImmutableList)}

        -   #### of

            ``` methodSignature
            public static PackageFileManifest of​(PackageMetadata getPackage,
                                                 com.google.common.collect.ImmutableSortedSet<String> includes,
                                                 com.google.common.collect.ImmutableMap<String,​Object> configs,
                                                 Optional<com.google.common.collect.ImmutableMap<String,​Optional<String>>> env,
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

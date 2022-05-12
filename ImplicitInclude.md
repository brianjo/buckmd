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
[Package]{.packageLabelInType} [com.facebook.buck.parser.implicit](package-summary.html)
:::

## Class ImplicitInclude {#class-implicitinclude .title title="Class ImplicitInclude"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.parser.implicit.ImplicitInclude

::: description
-   

    ------------------------------------------------------------------------

        public abstract class ImplicitInclude
        extends Object

    ::: block
    Represents a load path and symbols that should be implicitly
    included in a build file
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor           Description
          --------------------- -------------
          `ImplicitInclude()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `st                   | `fromConfig           | ::: block             |
        | atic ImplicitInclude` | urationString​(String  | Constructs a          |
        |                       | configurationString)` | `Abs                  |
        |                       |                       | tractImplicitInclude` |
        |                       |                       | from a configuration  |
        |                       |                       | string in the form of |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getImportString()`   |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `getLoadPath()`       | ::: block             |
        | e.devtools.build.lib. |                       | Returns the load path |
        | syntax.SkylarkImport` |                       | for the given path.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getSymbols()`        |                       |
        | abstract com.google.c |                       |                       |
        | ommon.collect.Immutab |                       |                       |
        | leMap<String,​String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `of​(                  |                       |
        | atic ImplicitInclude` | String rawImportLabel |                       |
        |                       | ,   Map<String,​? exte |                       |
        |                       | nds String> symbols)` |                       |
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

        -   #### ImplicitInclude

                public ImplicitInclude()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getSymbols()}

        -   #### getSymbols

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableMap<String,​String> getSymbols()
            ```

        []{#getImportString()}

        -   #### getImportString

            ``` methodSignature
            @Derived
            public String getImportString()
            ```

        []{#getLoadPath()}

        -   #### getLoadPath

            ``` methodSignature
            @Derived
            public com.google.devtools.build.lib.syntax.SkylarkImport getLoadPath()
            ```

            ::: block
            Returns the load path for the given path. SkylarkImport is
            used to eagerly compute fewer objects up front and
            centralize error handling
            :::

        []{#fromConfigurationString(java.lang.String)}

        -   #### fromConfigurationString

            ``` methodSignature
            public static ImplicitInclude fromConfigurationString​(String configurationString)
            ```

            ::: block
            Constructs a `AbstractImplicitInclude` from a configuration
            string in the form of
            //path/to:bzl_file.bzl::symbol_to_import::second_symbol_to_import
            :::

            [Parameters:]{.paramLabel}
            :   `configurationString` - The string used in configuration

            [Returns:]{.returnLabel}
            :   A parsed `AbstractImplicitInclude` object

        []{#of(java.lang.String,java.util.Map)}

        -   #### of

            ``` methodSignature
            public static ImplicitInclude of​(String rawImportLabel,
                                             Map<String,​? extends String> symbols)
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

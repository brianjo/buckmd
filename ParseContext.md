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
[Package]{.packageLabelInType} [com.facebook.buck.skylark.parser.context](package-summary.html)
:::

## Class ParseContext {#class-parsecontext .title title="Class ParseContext"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.skylark.parser.context.ParseContext

::: description
-   

    ------------------------------------------------------------------------

        public class ParseContext
        extends Object

    ::: block
    Tracks parse context.
    This class provides API to record information retrieved while
    parsing a build or package file like parsed rules or a package
    definition.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                     Description
          ----------------------------------------------- -------------
          `ParseContext​(PackageContext packageContext)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.go               | `getAccessedCo        |                       |
        | ogle.common.collect.I | nfigurationOptions()` |                       |
        | mmutableMap<String,​co |                       |                       |
        | m.google.common.colle |                       |                       |
        | ct.ImmutableMap<Strin |                       |                       |
        | g,​Optional<String>>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `PackageMetadata`     | `getPackage()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `PackageContext`      | `getPackageContext()` | ::: block             |
        |                       |                       | Returns a context of  |
        |                       |                       | the package currently |
        |                       |                       | being parsed.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static ParseContext` | `getParseContext​(com  | ::: block             |
        |                       | .google.devtools.buil | Get the               |
        |                       | d.lib.syntax.Environm | [`P                   |
        |                       | ent env,              | arseContext`](ParseCo |
        |                       |    com.google.devtool | ntext.html "class in  |
        |                       | s.build.lib.syntax.Fu | com.facebook.buck.sky |
        |                       | ncallExpression ast)` | lark.parser.context") |
        |                       |                       | by looking up in the  |
        |                       |                       | environment.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common    | `getRecordedRules()`  |                       |
        | .collect.ImmutableMap |                       |                       |
        | <String,​com.google.co |                       |                       |
        | mmon.collect.Immutabl |                       |                       |
        | eMap<String,​Object>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `                     |                       |
        |                       | hasRule​(String name)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `rec                  | ::: block             |
        |                       | ordPackage​(PackageMet | Records the parsed    |
        |                       | adata pkg,            | `rawPackage`.         |
        |                       |    com.google.devtool | :::                   |
        |                       | s.build.lib.syntax.Fu |                       |
        |                       | ncallExpression ast)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `reco                 | ::: block             |
        |                       | rdReadConfigurationOp | Records an accessed   |
        |                       | tion​(String section,  | `section.key`         |
        |                       |                       | configuration and its |
        |                       |         String key,   | returned `value`.     |
        |                       |                       | :::                   |
        |                       |        String value)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `recordRule​(com.goo   | ::: block             |
        |                       | gle.common.collect.Im | Records the parsed    |
        |                       | mutableMap<String,​Obj | `rawRule`.            |
        |                       | ect> rawRule,         | :::                   |
        |                       |    com.google.devtool |                       |
        |                       | s.build.lib.syntax.Fu |                       |
        |                       | ncallExpression ast)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `setup​(com.google.d   |                       |
        |                       | evtools.build.lib.syn |                       |
        |                       | tax.Environment env)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
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

        []{#<init>(com.facebook.buck.skylark.packages.PackageContext)}

        -   #### ParseContext

                public ParseContext​(PackageContext packageContext)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#recordPackage(com.facebook.buck.parser.api.PackageMetadata,com.google.devtools.build.lib.syntax.FuncallExpression)}

        -   #### recordPackage

            ``` methodSignature
            public void recordPackage​(PackageMetadata pkg,
                                      com.google.devtools.build.lib.syntax.FuncallExpression ast)
                               throws com.google.devtools.build.lib.syntax.EvalException
            ```

            ::: block
            Records the parsed `rawPackage`.
            :::

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`

        []{#recordRule(com.google.common.collect.ImmutableMap,com.google.devtools.build.lib.syntax.FuncallExpression)}

        -   #### recordRule

            ``` methodSignature
            public void recordRule​(com.google.common.collect.ImmutableMap<String,​Object> rawRule,
                                   com.google.devtools.build.lib.syntax.FuncallExpression ast)
                            throws com.google.devtools.build.lib.syntax.EvalException
            ```

            ::: block
            Records the parsed `rawRule`.
            :::

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`

        []{#recordReadConfigurationOption(java.lang.String,java.lang.String,java.lang.String)}

        -   #### recordReadConfigurationOption

            ``` methodSignature
            public void recordReadConfigurationOption​(String section,
                                                      String key,
                                                      @Nullable
                                                      String value)
            ```

            ::: block
            Records an accessed `section.key` configuration and its
            returned `value`.
            It\'s safe to not have to override existing values because
            configuration options are frozen for the duration of build
            file parsing.
            :::

        []{#getPackage()}

        -   #### getPackage

            ``` methodSignature
            public PackageMetadata getPackage()
            ```

            [Returns:]{.returnLabel}
            :   The package in the parsed package file if defined.

        []{#getRecordedRules()}

        -   #### getRecordedRules

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​com.google.common.collect.ImmutableMap<String,​Object>> getRecordedRules()
            ```

            [Returns:]{.returnLabel}
            :   The list of raw build rules discovered in parsed build
                file. Raw rule is presented as a map with attributes as
                keys and parameters as values.

        []{#hasRule(java.lang.String)}

        -   #### hasRule

            ``` methodSignature
            public boolean hasRule​(String name)
            ```

            [Returns:]{.returnLabel}
            :   `true` if the rule with provided name exists, `false`
                otherwise.

        []{#getAccessedConfigurationOptions()}

        -   #### getAccessedConfigurationOptions

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​com.google.common.collect.ImmutableMap<String,​Optional<String>>> getAccessedConfigurationOptions()
            ```

        []{#getPackageContext()}

        -   #### getPackageContext

            ``` methodSignature
            public PackageContext getPackageContext()
            ```

            ::: block
            Returns a context of the package currently being parsed.
            :::

        []{#getParseContext(com.google.devtools.build.lib.syntax.Environment,com.google.devtools.build.lib.syntax.FuncallExpression)}

        -   #### getParseContext

            ``` methodSignature
            public static ParseContext getParseContext​(com.google.devtools.build.lib.syntax.Environment env,
                                                       com.google.devtools.build.lib.syntax.FuncallExpression ast)
                                                throws com.google.devtools.build.lib.syntax.EvalException
            ```

            ::: block
            Get the
            [`ParseContext`](ParseContext.html "class in com.facebook.buck.skylark.parser.context")
            by looking up in the environment.
            :::

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`

        []{#setup(com.google.devtools.build.lib.syntax.Environment)}

        -   #### setup

            ``` methodSignature
            public void setup​(com.google.devtools.build.lib.syntax.Environment env)
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

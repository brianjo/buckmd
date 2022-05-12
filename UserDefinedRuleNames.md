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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.starlark.rule.names](package-summary.html)
:::

## Class UserDefinedRuleNames {#class-userdefinedrulenames .title title="Class UserDefinedRuleNames"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.starlark.rule.names.UserDefinedRuleNames

::: description
-   

    ------------------------------------------------------------------------

        public class UserDefinedRuleNames
        extends Object

    ::: block
    Helper methods to create, validate, and parse the identifier used by
    the parser for the `  buck.type` attribute on targets of user
    defined rules.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `s                    | `fromIdentifie        | ::: block             |
        | tatic Pair<com.google | r​(String identifier)` | Parses the extension  |
        | .devtools.build.lib.c |                       | label and the rule    |
        | mdline.Label,​String>` |                       | name from an          |
        |                       |                       | identifier            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `get                  | ::: block             |
        |                       | Identifier​(com.google | Creates an identifier |
        |                       | .devtools.build.lib.c | that can be used in   |
        |                       | mdline.Label extensio | `buck.type` in the    |
        |                       | nLabel,               | parser                |
        |                       | String exportedName)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static com.googl     | `importFromIdentifie  | ::: block             |
        | e.devtools.build.lib. | r​(String identifier)` | Convert a             |
        | syntax.SkylarkImport` |                       | \'buck.type\' string  |
        |                       |                       | into a SkylarkImport  |
        |                       |                       | object                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `isUse                | ::: block             |
        |                       | rDefinedRuleIdentifie | Determines whether    |
        |                       | r​(String identifier)` | the given identifier  |
        |                       |                       | is for a user defined |
        |                       |                       | rule                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getIdentifier(com.google.devtools.build.lib.cmdline.Label,java.lang.String)}

        -   #### getIdentifier

            ``` methodSignature
            public static String getIdentifier​(com.google.devtools.build.lib.cmdline.Label extensionLabel,
                                               String exportedName)
            ```

            ::: block
            Creates an identifier that can be used in `buck.type` in the
            parser
            :::

            [Parameters:]{.paramLabel}
            :   `extensionLabel` - the label of the extension file that
                this rule was defined in
            :   `exportedName` - the name of the rule in the extension
                file

            [Returns:]{.returnLabel}
            :   An identifier of the form
                `cell//package:extension.bzl:extension_name`

        []{#isUserDefinedRuleIdentifier(java.lang.String)}

        -   #### isUserDefinedRuleIdentifier

            ``` methodSignature
            public static boolean isUserDefinedRuleIdentifier​(String identifier)
            ```

            ::: block
            Determines whether the given identifier is for a user
            defined rule
            :::

            [Parameters:]{.paramLabel}
            :   `identifier` - the identifier from `buck.type`

            [Returns:]{.returnLabel}
            :   Whether this looks like an identifier for a user defined
                rule

        []{#fromIdentifier(java.lang.String)}

        -   #### fromIdentifier

            ``` methodSignature
            @Nullable
            public static Pair<com.google.devtools.build.lib.cmdline.Label,​String> fromIdentifier​(String identifier)
            ```

            ::: block
            Parses the extension label and the rule name from an
            identifier
            :::

            [Parameters:]{.paramLabel}
            :   `identifier` - the identifier from `buck.type`

            [Returns:]{.returnLabel}
            :   a pair of the label of the extension file that contains
                this rule, and the rule\'s name. If the identifier could
                not be parsed, `null` is returned.

        []{#importFromIdentifier(java.lang.String)}

        -   #### importFromIdentifier

            ``` methodSignature
            @Nullable
            public static com.google.devtools.build.lib.syntax.SkylarkImport importFromIdentifier​(String identifier)
            ```

            ::: block
            Convert a \'buck.type\' string into a SkylarkImport object
            :::

            [Parameters:]{.paramLabel}
            :   `identifier` - the result from buck.type

            [Returns:]{.returnLabel}
            :   A `SkylarkImport` object if `identifier` is parsable as
                a UDR identifier, else `null`
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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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

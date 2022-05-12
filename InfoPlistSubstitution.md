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
[Package]{.packageLabelInType} [com.facebook.buck.apple](package-summary.html)
:::

## Class InfoPlistSubstitution {#class-infoplistsubstitution .title title="Class InfoPlistSubstitution"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.InfoPlistSubstitution

::: description
-   

    ------------------------------------------------------------------------

        public class InfoPlistSubstitution
        extends Object

    ::: block
    Utility class to substitute Xcode Info.plist variables in the forms:
    `  ${FOO}  $(FOO)  ${FOO:modifier}  $(FOO:modifier)  ` with
    specified string values.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static j             | `createV              |                       |
        | ava.util.function.Fun | ariableExpansionFunct |                       |
        | ction<String,​String>` | ion​(Map<String,​String |                       |
        |                       | > variablesToExpand)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `g                    | ::: block             |
        | tic Optional<String>` | etVariableExpansionFo | Returns a variable    |
        |                       | rPlatform​(String keyN | expansion for keys    |
        |                       | ame,                  | which may depend on   |
        |                       |                String | platform name, trying |
        |                       |  platformName,        | from most to least    |
        |                       |                       | specific.             |
        |                       |     Map<String,​String | :::                   |
        |                       | > variablesToExpand)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `replaceVariablesI    |                       |
        |                       | nString​(String input, |                       |
        |                       |                       |                       |
        |                       |     Map<String,​String |                       |
        |                       | > variablesToExpand)` |                       |
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

        []{#getVariableExpansionForPlatform(java.lang.String,java.lang.String,java.util.Map)}

        -   #### getVariableExpansionForPlatform

            ``` methodSignature
            public static Optional<String> getVariableExpansionForPlatform​(String keyName,
                                                                           String platformName,
                                                                           Map<String,​String> variablesToExpand)
            ```

            ::: block
            Returns a variable expansion for keys which may depend on
            platform name, trying from most to least specific. While it
            doesn\'t capture all arbitrary wildcard expansions, it
            should handle everything likely to occur in practice.
            e.g.`VALID_ARCHS[sdk=iphoneos*]`
            :::

            [Parameters:]{.paramLabel}
            :   `keyName` - The name of the parent key. e.g.
                \"VALID_ARCHS\"
            :   `platformName` - The name of the platform. e.g.
                \"iphoneos\"
            :   `variablesToExpand` - The mapping of variable keys to
                values.

            [Returns:]{.returnLabel}
            :   Optional containing the string value if found, or
                absent.

        []{#replaceVariablesInString(java.lang.String,java.util.Map)}

        -   #### replaceVariablesInString

            ``` methodSignature
            public static String replaceVariablesInString​(String input,
                                                          Map<String,​String> variablesToExpand)
            ```

        []{#createVariableExpansionFunction(java.util.Map)}

        -   #### createVariableExpansionFunction

            ``` methodSignature
            public static java.util.function.Function<String,​String> createVariableExpansionFunction​(Map<String,​String> variablesToExpand)
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

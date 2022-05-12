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
[Package]{.packageLabelInType} [com.facebook.buck.core.starlark.rule](package-summary.html)
:::

## Class SkylarkRuleContextAttr {#class-skylarkrulecontextattr .title title="Class SkylarkRuleContextAttr"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.starlark.rule.SkylarkRuleContextAttr

::: description
-   

    All Implemented Interfaces:
    :   `com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable`,
        `com.google.devtools.build.lib.skylarkinterface.SkylarkValue`,
        `com.google.devtools.build.lib.syntax.ClassObject`

    ------------------------------------------------------------------------

        public class SkylarkRuleContextAttr
        extends Object
        implements com.google.devtools.build.lib.syntax.ClassObject, com.google.devtools.build.lib.skylarkinterface.SkylarkValue

    ::: block
    The struct representing the \'attr\' property of the \'ctx\' struct
    passed to a user defined rule\'s implementation function
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                         Method                                                                          Description
          --------------------------------------------------------- ------------------------------------------------------------------------------- -------------
          `String`                                                  `getErrorMessageForUnknownField​(String field)`                                   
          `com.google.common.collect.ImmutableCollection<String>`   `getFieldNames()`                                                                
          `Object`                                                  `getValue​(String name)`                                                          
          `void`                                                    `repr​(com.google.devtools.build.lib.skylarkinterface.SkylarkPrinter printer)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable}

            ### Methods inherited from interface com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable

            `debugPrint, str`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.google.devtools.build.lib.skylarkinterface.SkylarkValue}

            ### Methods inherited from interface com.google.devtools.build.lib.skylarkinterface.SkylarkValue

            `isHashable, isImmutable`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getValue(java.lang.String)}

        -   #### getValue

            ``` methodSignature
            @Nullable
            public Object getValue​(String name)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getValue` in
                interface `com.google.devtools.build.lib.syntax.ClassObject`

        []{#getFieldNames()}

        -   #### getFieldNames

            ``` methodSignature
            public com.google.common.collect.ImmutableCollection<String> getFieldNames()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFieldNames` in
                interface `com.google.devtools.build.lib.syntax.ClassObject`

        []{#getErrorMessageForUnknownField(java.lang.String)}

        -   #### getErrorMessageForUnknownField

            ``` methodSignature
            @Nullable
            public String getErrorMessageForUnknownField​(String field)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getErrorMessageForUnknownField` in
                interface `com.google.devtools.build.lib.syntax.ClassObject`

        []{#repr(com.google.devtools.build.lib.skylarkinterface.SkylarkPrinter)}

        -   #### repr

            ``` methodSignature
            public void repr​(com.google.devtools.build.lib.skylarkinterface.SkylarkPrinter printer)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `repr` in
                interface `com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable`
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

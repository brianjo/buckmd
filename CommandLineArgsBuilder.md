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
[Package]{.packageLabelInType} [com.facebook.buck.core.starlark.rule.args](package-summary.html)
:::

## Class CommandLineArgsBuilder {#class-commandlineargsbuilder .title title="Class CommandLineArgsBuilder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.starlark.rule.args.CommandLineArgsBuilder

::: description
-   

    All Implemented Interfaces:
    :   `CommandLineArgsBuilderApi`,
        `com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable`,
        `com.google.devtools.build.lib.skylarkinterface.SkylarkValue`

    ------------------------------------------------------------------------

        public class CommandLineArgsBuilder
        extends Object
        implements CommandLineArgsBuilderApi

    ::: block
    Struct exposed to skylark to create
    [`CommandLineArgs`](../../../rules/actions/lib/args/CommandLineArgs.html "interface in com.facebook.buck.core.rules.actions.lib.args")
    instances.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                  Description
          ---------------------------- -------------
          `CommandLineArgsBuilder()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type          Method                                                                                                                                                          Description
          -------------------------- --------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `CommandLineArgsBuilder`   `add​(Object argNameOrValue,    Object value,    String formatString,    com.google.devtools.build.lib.events.Location location)`                                 
          `CommandLineArgsBuilder`   `addAll​(com.google.devtools.build.lib.syntax.SkylarkList<?> values,       String formatString,       com.google.devtools.build.lib.events.Location location)`    
          `CommandLineArgs`          `build()`                                                                                                                                                        
          `void`                     `repr​(com.google.devtools.build.lib.skylarkinterface.SkylarkPrinter printer)`                                                                                    

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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### CommandLineArgsBuilder

                public CommandLineArgsBuilder()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#build()}

        -   #### build

            ``` methodSignature
            public CommandLineArgs build()
            ```

        []{#add(java.lang.Object,java.lang.Object,java.lang.String,com.google.devtools.build.lib.events.Location)}

        -   #### add

            ``` methodSignature
            public CommandLineArgsBuilder add​(Object argNameOrValue,
                                              Object value,
                                              String formatString,
                                              com.google.devtools.build.lib.events.Location location)
                                       throws com.google.devtools.build.lib.syntax.EvalException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `add` in interface `CommandLineArgsBuilderApi`

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`

        []{#addAll(com.google.devtools.build.lib.syntax.SkylarkList,java.lang.String,com.google.devtools.build.lib.events.Location)}

        -   #### addAll

            ``` methodSignature
            public CommandLineArgsBuilder addAll​(com.google.devtools.build.lib.syntax.SkylarkList<?> values,
                                                 String formatString,
                                                 com.google.devtools.build.lib.events.Location location)
                                          throws com.google.devtools.build.lib.syntax.EvalException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `addAll` in interface `CommandLineArgsBuilderApi`

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`

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

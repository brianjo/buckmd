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

## Interface SkylarkRuleContextActionsApi {#interface-skylarkrulecontextactionsapi .title title="Interface SkylarkRuleContextActionsApi"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `SkylarkRuleContextActions`

    ------------------------------------------------------------------------

        public interface SkylarkRuleContextActionsApi

    ::: block
    Struct containing methods that create actions within the
    implementation function of a user defined rule
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type             Method                                                                                                                                                                         Description
          ----------------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `CommandLineArgsBuilderApi`   `args​(Object args,     String formatString,     com.google.devtools.build.lib.events.Location location)`                                                                        
          `Artifact`                    `copyFile​(Artifact src,         Object dest,         com.google.devtools.build.lib.events.Location location)`                                                                   
          `Artifact`                    `declareFile​(String path,            com.google.devtools.build.lib.events.Location location)`                                                                                   
          `void`                        `run​(com.google.devtools.build.lib.syntax.SkylarkList<Object> arguments,    Object shortName,    Object userEnv,    com.google.devtools.build.lib.events.Location location)`    
          `Artifact`                    `write​(Object output,      Object content,      boolean isExecutable,      com.google.devtools.build.lib.events.Location location)`                                             

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

        []{#declareFile(java.lang.String,com.google.devtools.build.lib.events.Location)}

        -   #### declareFile

            ``` methodSignature
            Artifact declareFile​(String path,
                                 com.google.devtools.build.lib.events.Location location)
                          throws com.google.devtools.build.lib.syntax.EvalException
            ```

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`

        []{#copyFile(com.facebook.buck.core.artifact.Artifact,java.lang.Object,com.google.devtools.build.lib.events.Location)}

        -   #### copyFile

            ``` methodSignature
            Artifact copyFile​(Artifact src,
                              Object dest,
                              com.google.devtools.build.lib.events.Location location)
                       throws com.google.devtools.build.lib.syntax.EvalException
            ```

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`

        []{#write(java.lang.Object,java.lang.Object,boolean,com.google.devtools.build.lib.events.Location)}

        -   #### write

            ``` methodSignature
            Artifact write​(Object output,
                           Object content,
                           boolean isExecutable,
                           com.google.devtools.build.lib.events.Location location)
                    throws com.google.devtools.build.lib.syntax.EvalException
            ```

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`

        []{#args(java.lang.Object,java.lang.String,com.google.devtools.build.lib.events.Location)}

        -   #### args

            ``` methodSignature
            CommandLineArgsBuilderApi args​(Object args,
                                           String formatString,
                                           com.google.devtools.build.lib.events.Location location)
                                    throws com.google.devtools.build.lib.syntax.EvalException
            ```

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`

        []{#run(com.google.devtools.build.lib.syntax.SkylarkList,java.lang.Object,java.lang.Object,com.google.devtools.build.lib.events.Location)}

        -   #### run

            ``` methodSignature
            void run​(com.google.devtools.build.lib.syntax.SkylarkList<Object> arguments,
                     Object shortName,
                     Object userEnv,
                     com.google.devtools.build.lib.events.Location location)
              throws com.google.devtools.build.lib.syntax.EvalException
            ```

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`
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

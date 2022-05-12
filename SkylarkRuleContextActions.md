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
[Package]{.packageLabelInType} [com.facebook.buck.core.starlark.rule](package-summary.html)
:::

## Class SkylarkRuleContextActions {#class-skylarkrulecontextactions .title title="Class SkylarkRuleContextActions"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.starlark.rule.SkylarkRuleContextActions

::: description
-   

    All Implemented Interfaces:
    :   `SkylarkRuleContextActionsApi`

    ------------------------------------------------------------------------

        public class SkylarkRuleContextActions
        extends Object
        implements SkylarkRuleContextActionsApi

    ::: block
    Container for all methods that create actions within the
    implementation function of a user defined rule
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                            Description
          ------------------------------------------------------ -------------
          `SkylarkRuleContextActions​(ActionRegistry registry)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
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

        []{#<init>(com.facebook.buck.core.rules.actions.ActionRegistry)}

        -   #### SkylarkRuleContextActions

                public SkylarkRuleContextActions​(ActionRegistry registry)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#declareFile(java.lang.String,com.google.devtools.build.lib.events.Location)}

        -   #### declareFile

            ``` methodSignature
            public Artifact declareFile​(String path,
                                        com.google.devtools.build.lib.events.Location location)
                                 throws com.google.devtools.build.lib.syntax.EvalException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `declareFile` in
                interface `SkylarkRuleContextActionsApi`

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`

        []{#copyFile(com.facebook.buck.core.artifact.Artifact,java.lang.Object,com.google.devtools.build.lib.events.Location)}

        -   #### copyFile

            ``` methodSignature
            public Artifact copyFile​(Artifact src,
                                     Object dest,
                                     com.google.devtools.build.lib.events.Location location)
                              throws com.google.devtools.build.lib.syntax.EvalException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `copyFile` in interface `SkylarkRuleContextActionsApi`

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`

        []{#write(java.lang.Object,java.lang.Object,boolean,com.google.devtools.build.lib.events.Location)}

        -   #### write

            ``` methodSignature
            public Artifact write​(Object output,
                                  Object content,
                                  boolean isExecutable,
                                  com.google.devtools.build.lib.events.Location location)
                           throws com.google.devtools.build.lib.syntax.EvalException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `write` in interface `SkylarkRuleContextActionsApi`

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`

        []{#args(java.lang.Object,java.lang.String,com.google.devtools.build.lib.events.Location)}

        -   #### args

            ``` methodSignature
            public CommandLineArgsBuilderApi args​(Object args,
                                                  String formatString,
                                                  com.google.devtools.build.lib.events.Location location)
                                           throws com.google.devtools.build.lib.syntax.EvalException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `args` in interface `SkylarkRuleContextActionsApi`

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`

        []{#run(com.google.devtools.build.lib.syntax.SkylarkList,java.lang.Object,java.lang.Object,com.google.devtools.build.lib.events.Location)}

        -   #### run

            ``` methodSignature
            public void run​(com.google.devtools.build.lib.syntax.SkylarkList<Object> arguments,
                            Object shortName,
                            Object userEnv,
                            com.google.devtools.build.lib.events.Location location)
                     throws com.google.devtools.build.lib.syntax.EvalException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `run` in interface `SkylarkRuleContextActionsApi`

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

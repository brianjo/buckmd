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
[Package]{.packageLabelInType} [com.facebook.buck.skylark.function](package-summary.html)
:::

## Class SkylarkBuildModule {#class-skylarkbuildmodule .title title="Class SkylarkBuildModule"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.skylark.function.AbstractSkylarkFunctions](AbstractSkylarkFunctions.html "class in com.facebook.buck.skylark.function")

    -   -   com.facebook.buck.skylark.function.SkylarkBuildModule

::: description
-   

    All Implemented Interfaces:
    :   `SkylarkFunctionModule`

    ------------------------------------------------------------------------

        public class SkylarkBuildModule
        extends AbstractSkylarkFunctions
        implements SkylarkFunctionModule

    ::: block
    A class for the Skylark native module providing functions for
    parsing build files. It includes all functions provided natively by
    Buck and are available using `native.foo` in build file extensions
    and just `foo` in build files.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type             Field            Description
          ----------------------------- ---------------- -------------
          `static SkylarkBuildModule`   `BUILD_MODULE`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor              Description
          ------------------------ -------------
          `SkylarkBuildModule()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                            Method                                                                                                                                                                                                                                                                                                     Description
          ------------------------------------------------------------ ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `com.google.devtools.build.lib.syntax.SkylarkList<String>`   `glob​(com.google.devtools.build.lib.syntax.SkylarkList<String> include,     com.google.devtools.build.lib.syntax.SkylarkList<String> exclude,     Boolean excludeDirectories,     com.google.devtools.build.lib.syntax.FuncallExpression ast,     com.google.devtools.build.lib.syntax.Environment env)`    
          `com.google.devtools.build.lib.packages.Info`                `hostInfo()`                                                                                                                                                                                                                                                                                                
          `Object`                                                     `implicitPackageSymbol​(String symbol,                      Object defaultValue,                      com.google.devtools.build.lib.syntax.FuncallExpression ast,                      com.google.devtools.build.lib.syntax.Environment env)`                                                                
          `String`                                                     `packageName​(com.google.devtools.build.lib.syntax.FuncallExpression ast,            com.google.devtools.build.lib.syntax.Environment env)`                                                                                                                                                                  
          `String`                                                     `repositoryName​(com.google.devtools.build.lib.events.Location location,               com.google.devtools.build.lib.syntax.FuncallExpression ast,               com.google.devtools.build.lib.syntax.Environment env)`                                                                                      
          `Boolean`                                                    `ruleExists​(String name,           com.google.devtools.build.lib.syntax.FuncallExpression ast,           com.google.devtools.build.lib.syntax.Environment env)`                                                                                                                                             

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.skylark.function.AbstractSkylarkFunctions}

            ### Methods inherited from class com.facebook.buck.skylark.function.[AbstractSkylarkFunctions](AbstractSkylarkFunctions.html "class in com.facebook.buck.skylark.function")

            `readConfig`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#BUILD_MODULE}

        -   #### BUILD_MODULE

                public static final SkylarkBuildModule BUILD_MODULE
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### SkylarkBuildModule

                public SkylarkBuildModule()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#packageName(com.google.devtools.build.lib.syntax.FuncallExpression,com.google.devtools.build.lib.syntax.Environment)}

        -   #### packageName

            ``` methodSignature
            public String packageName​(com.google.devtools.build.lib.syntax.FuncallExpression ast,
                                      com.google.devtools.build.lib.syntax.Environment env)
                               throws com.google.devtools.build.lib.syntax.EvalException
            ```

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`

        []{#repositoryName(com.google.devtools.build.lib.events.Location,com.google.devtools.build.lib.syntax.FuncallExpression,com.google.devtools.build.lib.syntax.Environment)}

        -   #### repositoryName

            ``` methodSignature
            public String repositoryName​(com.google.devtools.build.lib.events.Location location,
                                         com.google.devtools.build.lib.syntax.FuncallExpression ast,
                                         com.google.devtools.build.lib.syntax.Environment env)
                                  throws com.google.devtools.build.lib.syntax.EvalException
            ```

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`

        []{#ruleExists(java.lang.String,com.google.devtools.build.lib.syntax.FuncallExpression,com.google.devtools.build.lib.syntax.Environment)}

        -   #### ruleExists

            ``` methodSignature
            public Boolean ruleExists​(String name,
                                      com.google.devtools.build.lib.syntax.FuncallExpression ast,
                                      com.google.devtools.build.lib.syntax.Environment env)
                               throws com.google.devtools.build.lib.syntax.EvalException
            ```

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`

        []{#glob(com.google.devtools.build.lib.syntax.SkylarkList,com.google.devtools.build.lib.syntax.SkylarkList,java.lang.Boolean,com.google.devtools.build.lib.syntax.FuncallExpression,com.google.devtools.build.lib.syntax.Environment)}

        -   #### glob

            ``` methodSignature
            public com.google.devtools.build.lib.syntax.SkylarkList<String> glob​(com.google.devtools.build.lib.syntax.SkylarkList<String> include,
                                                                                 com.google.devtools.build.lib.syntax.SkylarkList<String> exclude,
                                                                                 Boolean excludeDirectories,
                                                                                 com.google.devtools.build.lib.syntax.FuncallExpression ast,
                                                                                 com.google.devtools.build.lib.syntax.Environment env)
                                                                          throws com.google.devtools.build.lib.syntax.EvalException,
                                                                                 IOException,
                                                                                 InterruptedException
            ```

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`
            :   `IOException`
            :   `InterruptedException`

        []{#hostInfo()}

        -   #### hostInfo

            ``` methodSignature
            public com.google.devtools.build.lib.packages.Info hostInfo()
            ```

        []{#implicitPackageSymbol(java.lang.String,java.lang.Object,com.google.devtools.build.lib.syntax.FuncallExpression,com.google.devtools.build.lib.syntax.Environment)}

        -   #### implicitPackageSymbol

            ``` methodSignature
            @Nullable
            public Object implicitPackageSymbol​(String symbol,
                                                Object defaultValue,
                                                com.google.devtools.build.lib.syntax.FuncallExpression ast,
                                                com.google.devtools.build.lib.syntax.Environment env)
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

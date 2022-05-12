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

## Class SkylarkPackageModule {#class-skylarkpackagemodule .title title="Class SkylarkPackageModule"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.skylark.function.AbstractSkylarkFunctions](AbstractSkylarkFunctions.html "class in com.facebook.buck.skylark.function")

    -   -   com.facebook.buck.skylark.function.SkylarkPackageModule

::: description
-   

    All Implemented Interfaces:
    :   `SkylarkFunctionModule`

    ------------------------------------------------------------------------

        public class SkylarkPackageModule
        extends AbstractSkylarkFunctions
        implements SkylarkFunctionModule

    ::: block
    A class for the Skylark native module providing functions for
    parsing package files. It provides package() and other shared
    functions that are available also using `native.foo` in build file
    extensions and just `foo` in package files.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type               Field              Description
          ------------------------------- ------------------ -------------
          `static SkylarkPackageModule`   `PACKAGE_MODULE`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                Description
          -------------------------- -------------
          `SkylarkPackageModule()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                                                                                                                                                                                                                                                        Description
          ------------------- ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `void`              `packageFunction​(com.google.devtools.build.lib.syntax.SkylarkList<String> visibility,                com.google.devtools.build.lib.syntax.SkylarkList<String> within_view,                com.google.devtools.build.lib.syntax.FuncallExpression ast,                com.google.devtools.build.lib.syntax.Environment env)`    

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

        []{#PACKAGE_MODULE}

        -   #### PACKAGE_MODULE

                public static final SkylarkPackageModule PACKAGE_MODULE
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### SkylarkPackageModule

                public SkylarkPackageModule()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#packageFunction(com.google.devtools.build.lib.syntax.SkylarkList,com.google.devtools.build.lib.syntax.SkylarkList,com.google.devtools.build.lib.syntax.FuncallExpression,com.google.devtools.build.lib.syntax.Environment)}

        -   #### packageFunction

            ``` methodSignature
            public void packageFunction​(com.google.devtools.build.lib.syntax.SkylarkList<String> visibility,
                                        com.google.devtools.build.lib.syntax.SkylarkList<String> within_view,
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

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
[Package]{.packageLabelInType} [com.facebook.buck.skylark.function](package-summary.html)
:::

## Class AbstractSkylarkFunctions {#class-abstractskylarkfunctions .title title="Class AbstractSkylarkFunctions"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.skylark.function.AbstractSkylarkFunctions

::: description
-   

    Direct Known Subclasses:
    :   `SkylarkBuildModule`, `SkylarkPackageModule`

    ------------------------------------------------------------------------

        public abstract class AbstractSkylarkFunctions
        extends Object

    ::: block
    Abstract class containing function definitions shared by
    [`SkylarkBuildModule`](SkylarkBuildModule.html "class in com.facebook.buck.skylark.function")
    and
    [`SkylarkPackageModule`](SkylarkPackageModule.html "class in com.facebook.buck.skylark.function").
    Note: \@SkylarkModule does not support having the same name for
    multiple classes in
    `Runtime.setupSkylarkLibrary(com.google.common.collect.ImmutableMap.Builder<java.lang.String, java.lang.Object>, java.lang.Object)`
    and since we want the shared functions to also be under \"native\",
    we must subclass.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                    Description
          ------------------------------ -------------
          `AbstractSkylarkFunctions()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Object`              | `readCo               | ::: block             |
        |                       | nfig​(String section,  | Exposes a             |
        |                       |           String fiel | `read_config` for     |
        |                       | d,           Object d | Skylark parser.       |
        |                       | efaultValue,          | :::                   |
        |                       |   com.google.devtools |                       |
        |                       | .build.lib.syntax.Fun |                       |
        |                       | callExpression ast,   |                       |
        |                       |          com.google.d |                       |
        |                       | evtools.build.lib.syn |                       |
        |                       | tax.Environment env)` |                       |
        +-----------------------+-----------------------+-----------------------+

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

        []{#<init>()}

        -   #### AbstractSkylarkFunctions

                public AbstractSkylarkFunctions()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#readConfig(java.lang.String,java.lang.String,java.lang.Object,com.google.devtools.build.lib.syntax.FuncallExpression,com.google.devtools.build.lib.syntax.Environment)}

        -   #### readConfig

            ``` methodSignature
            public Object readConfig​(String section,
                                     String field,
                                     Object defaultValue,
                                     com.google.devtools.build.lib.syntax.FuncallExpression ast,
                                     com.google.devtools.build.lib.syntax.Environment env)
                              throws com.google.devtools.build.lib.syntax.EvalException
            ```

            ::: block
            Exposes a `read_config` for Skylark parser.
            This is a temporary solution to simplify migration from
            Python DSL to Skylark and allows clients to query values
            from `.buckconfig` files and `--config` command line
            arguments.

            Example, when buck is invoked with
            `--config user.value=my_value` an invocation of
            `read_config("user", "value", "default_value")` will return
            `my_value`.
            :::

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

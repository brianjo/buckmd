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
[Package]{.packageLabelInType} [com.facebook.buck.core.starlark.compatible](package-summary.html)
:::

## Class BuckStarlarkFunction {#class-buckstarlarkfunction .title title="Class BuckStarlarkFunction"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.starlark.compatible.BuckStarlarkFunction

::: description
-   

    All Implemented Interfaces:
    :   `com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable`,
        `com.google.devtools.build.lib.skylarkinterface.SkylarkValue`,
        `com.google.devtools.build.lib.syntax.StarlarkFunction`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `BuiltInProvider`

    ------------------------------------------------------------------------

        public abstract class BuckStarlarkFunction
        extends Object
        implements com.google.devtools.build.lib.syntax.StarlarkFunction

    ::: block
    Marker class that makes some method exposable to skylark.
    This class currently doesn\'t handle optionals and other
    java/skylark object coercing.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `BuckSt                           | ::: block                         |
        | arlarkFunction​(String methodName, | Creates a new skylark callable    |
        |                      Constructor< | function of the given name that   |
        | ?> constructor,                   | invokes the method handle.        |
        |    List<String> namedParams,      | :::                               |
        |                 List<String> defa |                                   |
        | ultSkylarkValues,                 |                                   |
        |      Set<String> noneableParams)` |                                   |
        +-----------------------------------+-----------------------------------+
        | `BuckStarlarkFunction​(Strin       | ::: block                         |
        | g methodName,                     | Creates a new skylark callable    |
        |  Method method,                   | function of the given name that   |
        |    List<String> namedParams,      | invokes the method handle.        |
        |                 List<String> defa | :::                               |
        | ultSkylarkValues,                 |                                   |
        |      Set<String> noneableParams)` |                                   |
        +-----------------------------------+-----------------------------------+

        : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                                                                                                                       Description
          ------------------- -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `Object`            `call​(List<Object> args,     Map<String,​Object> kwargs,     com.google.devtools.build.lib.syntax.FuncallExpression nullableAst,     com.google.devtools.build.lib.syntax.Environment env)`    
          `String`            `getName()`                                                                                                                                                                                   
          `void`              `repr​(com.google.devtools.build.lib.skylarkinterface.SkylarkPrinter printer)`                                                                                                                 

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

        []{#<init>(java.lang.String,java.lang.reflect.Constructor,java.util.List,java.util.List,java.util.Set)}

        -   #### BuckStarlarkFunction

                public BuckStarlarkFunction​(String methodName,
                                            Constructor<?> constructor,
                                            List<String> namedParams,
                                            List<String> defaultSkylarkValues,
                                            Set<String> noneableParams)

            ::: block
            Creates a new skylark callable function of the given name
            that invokes the method handle. The named parameters for
            skylark is the list of namedParams, which is mapped in order
            to the end of the parameter list for the method handle.
            :::

            [Parameters:]{.paramLabel}
            :   `methodName` - the function name exposed to skylark
            :   `constructor` - the constructor that we will call as a
                method
            :   `namedParams` - a list of named parameters for skylark.
                The names are mapped in order to the parameters of
                `constructor`
            :   `defaultSkylarkValues` - a list of default values for
                parameters in skylark. The names are mapped in order to
                the parameters of `constructor`

        []{#<init>(java.lang.String,java.lang.reflect.Method,java.util.List,java.util.List,java.util.Set)}

        -   #### BuckStarlarkFunction

                public BuckStarlarkFunction​(String methodName,
                                            Method method,
                                            List<String> namedParams,
                                            List<String> defaultSkylarkValues,
                                            Set<String> noneableParams)

            ::: block
            Creates a new skylark callable function of the given name
            that invokes the method handle. The named parameters for
            skylark is the list of namedParams, which is mapped in order
            to the end of the parameter list for the method handle.
            :::

            [Parameters:]{.paramLabel}
            :   `methodName` - the function name exposed to skylark
            :   `method` - a method that will eventually be called in
                [`call(List, Map,      FuncallExpression, Environment)`](#call(java.util.List,java.util.Map,com.google.devtools.build.lib.syntax.FuncallExpression,com.google.devtools.build.lib.syntax.Environment))
            :   `namedParams` - a list of named parameters for skylark.
                The names are mapped in order to the parameters of
                `method`
            :   `defaultSkylarkValues` - a list of default values for
                parameters in skylark. The values are mapped in order to
                the parameters of `method`
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#call(java.util.List,java.util.Map,com.google.devtools.build.lib.syntax.FuncallExpression,com.google.devtools.build.lib.syntax.Environment)}

        -   #### call

            ``` methodSignature
            public Object call​(List<Object> args,
                               @Nullable
                               Map<String,​Object> kwargs,
                               @Nullable
                               com.google.devtools.build.lib.syntax.FuncallExpression nullableAst,
                               com.google.devtools.build.lib.syntax.Environment env)
                        throws com.google.devtools.build.lib.syntax.EvalException,
                               InterruptedException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `call` in
                interface `com.google.devtools.build.lib.syntax.StarlarkFunction`

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`
            :   `InterruptedException`

        []{#repr(com.google.devtools.build.lib.skylarkinterface.SkylarkPrinter)}

        -   #### repr

            ``` methodSignature
            public void repr​(com.google.devtools.build.lib.skylarkinterface.SkylarkPrinter printer)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `repr` in
                interface `com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable`

        []{#getName()}

        -   #### getName

            ``` methodSignature
            public String getName()
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

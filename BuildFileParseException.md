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
[Package]{.packageLabelInType} [com.facebook.buck.parser.exceptions](package-summary.html)
:::

## Class BuildFileParseException {#class-buildfileparseexception .title title="Class BuildFileParseException"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Throwable](http://docs.oracle.com/javase/7/docs/api/java/lang/Throwable.html?is-external=true "class or interface in java.lang"){.externalLink}

    -   -   [java.lang.Exception](http://docs.oracle.com/javase/7/docs/api/java/lang/Exception.html?is-external=true "class or interface in java.lang"){.externalLink}

        -   -   [java.lang.RuntimeException](http://docs.oracle.com/javase/7/docs/api/java/lang/RuntimeException.html?is-external=true "class or interface in java.lang"){.externalLink}

            -   -   [com.facebook.buck.core.exceptions.HumanReadableException](../../core/exceptions/HumanReadableException.html "class in com.facebook.buck.core.exceptions")

                -   -   com.facebook.buck.parser.exceptions.BuildFileParseException

::: description
-   

    All Implemented Interfaces:
    :   `ExceptionWithHumanReadableMessage`, `Serializable`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `BuildTargetException`

    ------------------------------------------------------------------------

        public class BuildFileParseException
        extends HumanReadableException

    ::: block
    Thrown if we encounter an unexpected, fatal condition while
    interacting with the build file parser.
    :::

    [See Also:]{.seeLabel}
    :   [Serialized
        Form](../../../../../serialized-form.html#com.facebook.buck.parser.exceptions.BuildFileParseException)
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                                                                        Description
          -------------- ---------------------------------------------------------------------------------- -------------
          `protected `   `BuildFileParseException​(String message,                        Object... args)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                  Method                                                                                          Description
          ---------------------------------- ----------------------------------------------------------------------------------------------- -------------
          `static BuildFileParseException`   `createForBuildFileParseError​(Path buildFile,                             IOException cause)`    
          `static BuildFileParseException`   `createForUnknownParseError​(String message,                           Object... args)`           
          `String`                           `getHumanReadableErrorMessage()`                                                                 

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.exceptions.HumanReadableException}

            ### Methods inherited from class com.facebook.buck.core.exceptions.[HumanReadableException](../../core/exceptions/HumanReadableException.html "class in com.facebook.buck.core.exceptions")

            `getDependencyStack`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Throwable}

            ### Methods inherited from class java.lang.[Throwable](http://docs.oracle.com/javase/7/docs/api/java/lang/Throwable.html?is-external=true "class or interface in java.lang"){.externalLink}

            `addSuppressed, fillInStackTrace, getCause, getLocalizedMessage, getMessage, getStackTrace, getSuppressed, initCause, printStackTrace, printStackTrace, printStackTrace, setStackTrace, toString`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.lang.String,java.lang.Object...)}

        -   #### BuildFileParseException

                protected BuildFileParseException​(String message,
                                                  Object... args)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#createForUnknownParseError(java.lang.String,java.lang.Object...)}

        -   #### createForUnknownParseError

            ``` methodSignature
            public static BuildFileParseException createForUnknownParseError​(String message,
                                                                             Object... args)
            ```

        []{#createForBuildFileParseError(java.nio.file.Path,java.io.IOException)}

        -   #### createForBuildFileParseError

            ``` methodSignature
            public static BuildFileParseException createForBuildFileParseError​(Path buildFile,
                                                                               @Nullable
                                                                               IOException cause)
            ```

        []{#getHumanReadableErrorMessage()}

        -   #### getHumanReadableErrorMessage

            ``` methodSignature
            public String getHumanReadableErrorMessage()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getHumanReadableErrorMessage` in
                interface `ExceptionWithHumanReadableMessage`

            [Overrides:]{.overrideSpecifyLabel}
            :   `getHumanReadableErrorMessage` in
                class `HumanReadableException`

            [Returns:]{.returnLabel}
            :   a human-readable error message
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

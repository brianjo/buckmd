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
[Package]{.packageLabelInType} [com.facebook.buck.core.exceptions](package-summary.html)
:::

## Class BuckUncheckedExecutionException {#class-buckuncheckedexecutionexception .title title="Class BuckUncheckedExecutionException"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Throwable](http://docs.oracle.com/javase/7/docs/api/java/lang/Throwable.html?is-external=true "class or interface in java.lang"){.externalLink}

    -   -   [java.lang.Exception](http://docs.oracle.com/javase/7/docs/api/java/lang/Exception.html?is-external=true "class or interface in java.lang"){.externalLink}

        -   -   [java.lang.RuntimeException](http://docs.oracle.com/javase/7/docs/api/java/lang/RuntimeException.html?is-external=true "class or interface in java.lang"){.externalLink}

            -   -   com.facebook.buck.core.exceptions.BuckUncheckedExecutionException

::: description
-   

    All Implemented Interfaces:
    :   `ExceptionWithContext`, `WrapsException`, `Serializable`

    ------------------------------------------------------------------------

        public class BuckUncheckedExecutionException
        extends RuntimeException
        implements ExceptionWithContext, WrapsException

    ::: block
    Allows wrapping a checked exception into an unchecked exception in a
    way that Buck understands.
    Users should prefer
    `throw new BuckUncheckedExecutionException(exception);` to
    `  throw new RuntimeException(exception);` for throwing arbitrary
    checked exceptions as unchecked. Even better would be to specify
    that the function throws BuckExecutionException.
    :::

    [See Also:]{.seeLabel}
    :   [Serialized
        Form](../../../../../serialized-form.html#com.facebook.buck.core.exceptions.BuckUncheckedExecutionException)
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                        Description
          -------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `BuckUncheckedExecutionException​(String message)`                                                                                                   
          `BuckUncheckedExecutionException​(String message,                                String context)`                                                    
          `BuckUncheckedExecutionException​(String message,                                Throwable cause,                                String context)`    
          `BuckUncheckedExecutionException​(Throwable cause)`                                                                                                  
          `BuckUncheckedExecutionException​(Throwable cause,                                String context)`                                                   
          `BuckUncheckedExecutionException​(Throwable cause,                                String format,                                Object... args)`     

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type    Method           Description
          -------------------- ---------------- -------------
          `Optional<String>`   `getContext()`    
          `String`             `getMessage()`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Throwable}

            ### Methods inherited from class java.lang.[Throwable](http://docs.oracle.com/javase/7/docs/api/java/lang/Throwable.html?is-external=true "class or interface in java.lang"){.externalLink}

            `addSuppressed, fillInStackTrace, getCause, getLocalizedMessage, getStackTrace, getSuppressed, initCause, printStackTrace, printStackTrace, printStackTrace, setStackTrace, toString`

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

        []{#<init>(java.lang.String)}

        -   #### BuckUncheckedExecutionException

                public BuckUncheckedExecutionException​(String message)

        []{#<init>(java.lang.String,java.lang.String)}

        -   #### BuckUncheckedExecutionException

                public BuckUncheckedExecutionException​(String message,
                                                       @Nullable
                                                       String context)

        []{#<init>(java.lang.String,java.lang.Throwable,java.lang.String)}

        -   #### BuckUncheckedExecutionException

                public BuckUncheckedExecutionException​(String message,
                                                       @Nullable
                                                       Throwable cause,
                                                       @Nullable
                                                       String context)

        []{#<init>(java.lang.Throwable)}

        -   #### BuckUncheckedExecutionException

                public BuckUncheckedExecutionException​(Throwable cause)

        []{#<init>(java.lang.Throwable,java.lang.String)}

        -   #### BuckUncheckedExecutionException

                public BuckUncheckedExecutionException​(Throwable cause,
                                                       @Nullable
                                                       String context)

        []{#<init>(java.lang.Throwable,java.lang.String,java.lang.Object...)}

        -   #### BuckUncheckedExecutionException

                public BuckUncheckedExecutionException​(Throwable cause,
                                                       String format,
                                                       Object... args)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getMessage()}

        -   #### getMessage

            ``` methodSignature
            public String getMessage()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `getMessage` in class `Throwable`

        []{#getContext()}

        -   #### getContext

            ``` methodSignature
            public Optional<String> getContext()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getContext` in interface `ExceptionWithContext`
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
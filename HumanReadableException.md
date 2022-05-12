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

## Class HumanReadableException {#class-humanreadableexception .title title="Class HumanReadableException"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Throwable](http://docs.oracle.com/javase/7/docs/api/java/lang/Throwable.html?is-external=true "class or interface in java.lang"){.externalLink}

    -   -   [java.lang.Exception](http://docs.oracle.com/javase/7/docs/api/java/lang/Exception.html?is-external=true "class or interface in java.lang"){.externalLink}

        -   -   [java.lang.RuntimeException](http://docs.oracle.com/javase/7/docs/api/java/lang/RuntimeException.html?is-external=true "class or interface in java.lang"){.externalLink}

            -   -   com.facebook.buck.core.exceptions.HumanReadableException

::: description
-   

    All Implemented Interfaces:
    :   `ExceptionWithHumanReadableMessage`, `Serializable`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `ActionCreationException`, `ArtifactDeclarationException`,
        `BuildFileParseException`, `BuildTargetParseException`,
        `CommandAlias.UnsupportedPlatformException`,
        `CommandLineArgException`, `CommandLineException`,
        `FlavorDomainException`, `LogDaemonException`,
        `ProcessExecutionFailedException`, `RuleAnalysisException`,
        `ToolchainInstantiationException`, `UnexpectedFlavorException`,
        `UnknownCellException`

    ------------------------------------------------------------------------

        public class HumanReadableException
        extends RuntimeException
        implements ExceptionWithHumanReadableMessage

    ::: block
    Exception with an error message that can sensibly be displayed to
    the user without a stacktrace. This exception is meant only to be
    caught at the top level of the application.
    :::

    [See Also:]{.seeLabel}
    :   [Serialized
        Form](../../../../../serialized-form.html#com.facebook.buck.core.exceptions.HumanReadableException)
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                      Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `HumanReadableException​(DependencyStack dependencyStack,                       String humanReadableErrorMessage)`                                                                                 
          `HumanReadableException​(DependencyStack dependencyStack,                       String humanReadableFormatString,                       Object... args)`                                           
          `HumanReadableException​(ExceptionWithHumanReadableMessage e)`                                                                                                                                     
          `HumanReadableException​(String humanReadableErrorMessage)`                                                                                                                                        
          `HumanReadableException​(String humanReadableFormatString,                       Object... args)`                                                                                                  
          `HumanReadableException​(Throwable cause,                       DependencyStack dependencyStack,                       String humanReadableErrorMessage)`                                          
          `HumanReadableException​(Throwable cause,                       DependencyStack dependencyStack,                       String humanReadableFormatString,                       Object... args)`    
          `HumanReadableException​(Throwable cause,                       String humanReadableErrorMessage)`                                                                                                 
          `HumanReadableException​(Throwable cause,                       String humanReadableFormatString,                       Object... args)`                                                           

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `DependencyStack`     | `                     | ::: block             |
        |                       | getDependencyStack()` | Get the dependency    |
        |                       |                       | stack associated with |
        |                       |                       | this error            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getHumanRe           |                       |
        |                       | adableErrorMessage()` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

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

        []{#<init>(com.facebook.buck.core.exceptions.DependencyStack,java.lang.String,java.lang.Object...)}

        -   #### HumanReadableException

                public HumanReadableException​(DependencyStack dependencyStack,
                                              String humanReadableFormatString,
                                              Object... args)

        []{#<init>(com.facebook.buck.core.exceptions.DependencyStack,java.lang.String)}

        -   #### HumanReadableException

                public HumanReadableException​(DependencyStack dependencyStack,
                                              String humanReadableErrorMessage)

        []{#<init>(java.lang.Throwable,com.facebook.buck.core.exceptions.DependencyStack,java.lang.String)}

        -   #### HumanReadableException

                public HumanReadableException​(@Nullable
                                              Throwable cause,
                                              DependencyStack dependencyStack,
                                              String humanReadableErrorMessage)

        []{#<init>(java.lang.Throwable,com.facebook.buck.core.exceptions.DependencyStack,java.lang.String,java.lang.Object...)}

        -   #### HumanReadableException

                public HumanReadableException​(@Nullable
                                              Throwable cause,
                                              DependencyStack dependencyStack,
                                              String humanReadableFormatString,
                                              Object... args)

        []{#<init>(java.lang.String,java.lang.Object...)}

        -   #### HumanReadableException

                public HumanReadableException​(String humanReadableFormatString,
                                              Object... args)

        []{#<init>(java.lang.String)}

        -   #### HumanReadableException

                public HumanReadableException​(String humanReadableErrorMessage)

        []{#<init>(java.lang.Throwable,java.lang.String)}

        -   #### HumanReadableException

                public HumanReadableException​(@Nullable
                                              Throwable cause,
                                              String humanReadableErrorMessage)

        []{#<init>(java.lang.Throwable,java.lang.String,java.lang.Object...)}

        -   #### HumanReadableException

                public HumanReadableException​(@Nullable
                                              Throwable cause,
                                              String humanReadableFormatString,
                                              Object... args)

        []{#<init>(com.facebook.buck.core.exceptions.ExceptionWithHumanReadableMessage)}

        -   #### HumanReadableException

                public HumanReadableException​(ExceptionWithHumanReadableMessage e)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getHumanReadableErrorMessage()}

        -   #### getHumanReadableErrorMessage

            ``` methodSignature
            public String getHumanReadableErrorMessage()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getHumanReadableErrorMessage` in
                interface `ExceptionWithHumanReadableMessage`

            [Returns:]{.returnLabel}
            :   a human-readable error message

        []{#getDependencyStack()}

        -   #### getDependencyStack

            ``` methodSignature
            public DependencyStack getDependencyStack()
            ```

            ::: block
            [Description copied from
            interface: `ExceptionWithHumanReadableMessage`]{.descfrmTypeLabel}
            :::

            ::: block
            Get the dependency stack associated with this error
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDependencyStack` in
                interface `ExceptionWithHumanReadableMessage`
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

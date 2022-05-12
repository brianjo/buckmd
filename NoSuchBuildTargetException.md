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

## Class NoSuchBuildTargetException {#class-nosuchbuildtargetexception .title title="Class NoSuchBuildTargetException"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Throwable](http://docs.oracle.com/javase/7/docs/api/java/lang/Throwable.html?is-external=true "class or interface in java.lang"){.externalLink}

    -   -   [java.lang.Exception](http://docs.oracle.com/javase/7/docs/api/java/lang/Exception.html?is-external=true "class or interface in java.lang"){.externalLink}

        -   -   [java.lang.RuntimeException](http://docs.oracle.com/javase/7/docs/api/java/lang/RuntimeException.html?is-external=true "class or interface in java.lang"){.externalLink}

            -   -   [com.facebook.buck.core.exceptions.HumanReadableException](../../core/exceptions/HumanReadableException.html "class in com.facebook.buck.core.exceptions")

                -   -   [com.facebook.buck.parser.exceptions.BuildFileParseException](BuildFileParseException.html "class in com.facebook.buck.parser.exceptions")

                    -   -   [com.facebook.buck.parser.exceptions.BuildTargetException](BuildTargetException.html "class in com.facebook.buck.parser.exceptions")

                        -   -   com.facebook.buck.parser.exceptions.NoSuchBuildTargetException

::: description
-   

    All Implemented Interfaces:
    :   `ExceptionWithHumanReadableMessage`, `Serializable`

    ------------------------------------------------------------------------

        public class NoSuchBuildTargetException
        extends BuildTargetException

    ::: block
    Thrown when build target definition is missing in corresponding
    build file
    :::

    [See Also:]{.seeLabel}
    :   [Serialized
        Form](../../../../../serialized-form.html#com.facebook.buck.parser.exceptions.NoSuchBuildTargetException)
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                    Description
          -------------------------------------------------------------- -------------
          `NoSuchBuildTargetException​(BuildTarget target)`                
          `NoSuchBuildTargetException​(UnconfiguredBuildTarget target)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                     Method                                                                                                                                                                                                                                                                                                                                                        Description
          ------------------------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `static NoSuchBuildTargetException`   `createForMissingBuildRule​(UnconfiguredBuildTarget buildTarget,                          com.google.common.collect.ImmutableList<UnconfiguredBuildTarget> similarTargets,                          int totalTargets,                          java.util.function.Function<Path,​OptionalLong> fileSizeFetcher,                          Path buildFilePath)`    
          `String`                              `getHumanReadableErrorMessage()`                                                                                                                                                                                                                                                                                                                               

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.parser.exceptions.BuildFileParseException}

            ### Methods inherited from class com.facebook.buck.parser.exceptions.[BuildFileParseException](BuildFileParseException.html "class in com.facebook.buck.parser.exceptions")

            `createForBuildFileParseError, createForUnknownParseError`

        ```{=html}
        <!-- -->
        ```
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

        []{#<init>(com.facebook.buck.core.model.BuildTarget)}

        -   #### NoSuchBuildTargetException

                public NoSuchBuildTargetException​(BuildTarget target)

        []{#<init>(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### NoSuchBuildTargetException

                public NoSuchBuildTargetException​(UnconfiguredBuildTarget target)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#createForMissingBuildRule(com.facebook.buck.core.model.UnconfiguredBuildTarget,com.google.common.collect.ImmutableList,int,java.util.function.Function,java.nio.file.Path)}

        -   #### createForMissingBuildRule

            ``` methodSignature
            public static NoSuchBuildTargetException createForMissingBuildRule​(UnconfiguredBuildTarget buildTarget,
                                                                               com.google.common.collect.ImmutableList<UnconfiguredBuildTarget> similarTargets,
                                                                               int totalTargets,
                                                                               java.util.function.Function<Path,​OptionalLong> fileSizeFetcher,
                                                                               Path buildFilePath)
            ```

            [Parameters:]{.paramLabel}
            :   `buildTarget` - the failing
                [`BuildTarget`](../../core/model/BuildTarget.html "class in com.facebook.buck.core.model")
            :   `similarTargets` - targets that are similar to
                `buildTarget` to suggest to users
            :   `totalTargets` - the total number of targets that were
                found in the build file
            :   `fileSizeFetcher` - a function that takes a path and
                returns its filesize, or
                [`Optional.empty()`](http://docs.oracle.com/javase/7/docs/api/java/util/Optional.html?is-external=true#empty() "class or interface in java.util"){.externalLink}
                if the file couldn\'t be read
            :   `buildFilePath` - the absolute path to the build file

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
                class `BuildFileParseException`

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

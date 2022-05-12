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
[Package]{.packageLabelInType} [com.facebook.buck.core.model.targetgraph](package-summary.html)
:::

## Class NoSuchTargetException {#class-nosuchtargetexception .title title="Class NoSuchTargetException"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Throwable](http://docs.oracle.com/javase/7/docs/api/java/lang/Throwable.html?is-external=true "class or interface in java.lang"){.externalLink}

    -   -   [java.lang.Exception](http://docs.oracle.com/javase/7/docs/api/java/lang/Exception.html?is-external=true "class or interface in java.lang"){.externalLink}

        -   -   [java.lang.RuntimeException](http://docs.oracle.com/javase/7/docs/api/java/lang/RuntimeException.html?is-external=true "class or interface in java.lang"){.externalLink}

            -   -   com.facebook.buck.core.model.targetgraph.NoSuchTargetException

::: description
-   

    All Implemented Interfaces:
    :   `ExceptionWithHumanReadableMessage`, `Serializable`

    ------------------------------------------------------------------------

        public class NoSuchTargetException
        extends RuntimeException
        implements ExceptionWithHumanReadableMessage

    [See Also:]{.seeLabel}
    :   [Serialized
        Form](../../../../../../serialized-form.html#com.facebook.buck.core.model.targetgraph.NoSuchTargetException)
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                              Description
          -------------------------------------------------------------------------------------------------------- -------------
          `NoSuchTargetException​(DependencyStack dependencyStack,                      BuildTarget buildTarget)`    

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

        []{#<init>(com.facebook.buck.core.exceptions.DependencyStack,com.facebook.buck.core.model.BuildTarget)}

        -   #### NoSuchTargetException

                public NoSuchTargetException​(DependencyStack dependencyStack,
                                             BuildTarget buildTarget)
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
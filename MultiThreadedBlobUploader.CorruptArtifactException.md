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
[Package]{.packageLabelInType} [com.facebook.buck.remoteexecution.util](package-summary.html)
:::

## Class MultiThreadedBlobUploader.CorruptArtifactException {#class-multithreadedblobuploader.corruptartifactexception .title title="Class MultiThreadedBlobUploader.CorruptArtifactException"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Throwable](http://docs.oracle.com/javase/7/docs/api/java/lang/Throwable.html?is-external=true "class or interface in java.lang"){.externalLink}

    -   -   [java.lang.Exception](http://docs.oracle.com/javase/7/docs/api/java/lang/Exception.html?is-external=true "class or interface in java.lang"){.externalLink}

        -   -   [java.io.IOException](http://docs.oracle.com/javase/7/docs/api/java/io/IOException.html?is-external=true "class or interface in java.io"){.externalLink}

            -   -   com.facebook.buck.remoteexecution.util.MultiThreadedBlobUploader.CorruptArtifactException

::: description
-   

    All Implemented Interfaces:
    :   `Serializable`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [MultiThreadedBlobUploader](MultiThreadedBlobUploader.html "class in com.facebook.buck.remoteexecution.util")

    ------------------------------------------------------------------------

        public static class MultiThreadedBlobUploader.CorruptArtifactException
        extends IOException

    ::: block
    An exception that indicates that an upload failed because the
    artifact was corrupted.
    :::

    [See Also:]{.seeLabel}
    :   [Serialized
        Form](../../../../../serialized-form.html#com.facebook.buck.remoteexecution.util.MultiThreadedBlobUploader.CorruptArtifactException)
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                          Description
          ------------------------------------------------------------------------------------ -------------
          `CorruptArtifactException​(String msg,                         String description)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `String`              | `getDescription()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `getDes               | ::: block             |
        | tic Optional<String>` | cription​(ThrowableCau | Returns               |
        |                       | seIterable iterable)` | Cor                   |
        |                       |                       | ruptArtifactException |
        |                       |                       | throwable if any of   |
        |                       |                       | the causes in the     |
        |                       |                       | [`ThrowableCauseI     |
        |                       |                       | terable`](../../core/ |
        |                       |                       | exceptions/ThrowableC |
        |                       |                       | auseIterable.html "cl |
        |                       |                       | ass in com.facebook.b |
        |                       |                       | uck.core.exceptions") |
        |                       |                       | are                   |
        |                       |                       | Corr                  |
        |                       |                       | uptArtifactException. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `isCause​(ThrowableCau | ::: block             |
        |                       | seIterable iterable)` | Determines if any of  |
        |                       |                       | the causes in the     |
        |                       |                       | [`ThrowableCauseI     |
        |                       |                       | terable`](../../core/ |
        |                       |                       | exceptions/ThrowableC |
        |                       |                       | auseIterable.html "cl |
        |                       |                       | ass in com.facebook.b |
        |                       |                       | uck.core.exceptions") |
        |                       |                       | are                   |
        |                       |                       | Cor                   |
        |                       |                       | ruptArtifactException |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
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

        []{#<init>(java.lang.String,java.lang.String)}

        -   #### CorruptArtifactException

                public CorruptArtifactException​(String msg,
                                                String description)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getDescription()}

        -   #### getDescription

            ``` methodSignature
            public String getDescription()
            ```

        []{#isCause(com.facebook.buck.core.exceptions.ThrowableCauseIterable)}

        -   #### isCause

            ``` methodSignature
            public static boolean isCause​(ThrowableCauseIterable iterable)
            ```

            ::: block
            Determines if any of the causes in the
            [`ThrowableCauseIterable`](../../core/exceptions/ThrowableCauseIterable.html "class in com.facebook.buck.core.exceptions")
            are CorruptArtifactException
            :::

            [Parameters:]{.paramLabel}

            `iterable` -

            [Returns:]{.returnLabel}

        []{#getDescription(com.facebook.buck.core.exceptions.ThrowableCauseIterable)}

        -   #### getDescription

            ``` methodSignature
            public static Optional<String> getDescription​(ThrowableCauseIterable iterable)
            ```

            ::: block
            Returns CorruptArtifactException throwable if any of the
            causes in the
            [`ThrowableCauseIterable`](../../core/exceptions/ThrowableCauseIterable.html "class in com.facebook.buck.core.exceptions")
            are CorruptArtifactException. Check
            [`isCause(ThrowableCauseIterable)`](#isCause(com.facebook.buck.core.exceptions.ThrowableCauseIterable))
            first
            :::

            [Parameters:]{.paramLabel}

            `iterable` -

            [Returns:]{.returnLabel}
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

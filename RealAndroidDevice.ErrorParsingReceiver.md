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
[Package]{.packageLabelInType} [com.facebook.buck.android.exopackage](package-summary.html)
:::

## Class RealAndroidDevice.ErrorParsingReceiver {#class-realandroiddevice.errorparsingreceiver .title title="Class RealAndroidDevice.ErrorParsingReceiver"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.android.ddmlib.MultiLineReceiver

    -   -   com.facebook.buck.android.exopackage.RealAndroidDevice.ErrorParsingReceiver

::: description
-   

    All Implemented Interfaces:
    :   `com.android.ddmlib.IShellOutputReceiver`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [RealAndroidDevice](RealAndroidDevice.html "class in com.facebook.buck.android.exopackage")

    ------------------------------------------------------------------------

        public abstract static class RealAndroidDevice.ErrorParsingReceiver
        extends com.android.ddmlib.MultiLineReceiver

    ::: block
    Implementation of `IShellOutputReceiver` with helper functions to
    parse output lines and figure out if a call to
    `IDevice.executeShellCommand(String,  com.android.ddmlib.IShellOutputReceiver)`
    succeeded.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                Description
          -------------------------- -------------
          `ErrorParsingReceiver()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `String`              | `getErrorMessage()`   |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isCancelled()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `prote                | `matchF               | ::: block             |
        | cted abstract String` | orError​(String line)` | Look for an error     |
        |                       |                       | message in `line`.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `processNewL          |                       |
        |                       | ines​(String[] lines)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.android.ddmlib.MultiLineReceiver}

            ### Methods inherited from class com.android.ddmlib.MultiLineReceiver

            `addOutput, done, flush, setTrimLine`

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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### ErrorParsingReceiver

                public ErrorParsingReceiver()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#matchForError(java.lang.String)}

        -   #### matchForError

            ``` methodSignature
            @Nullable
            protected abstract String matchForError​(String line)
            ```

            ::: block
            Look for an error message in `line`.
            :::

            [Parameters:]{.paramLabel}
            :   `line` -

            [Returns:]{.returnLabel}
            :   an error message if `line` is indicative of an error,
                `null` otherwise.

        []{#processNewLines(java.lang.String[])}

        -   #### processNewLines

            ``` methodSignature
            public void processNewLines​(String[] lines)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `processNewLines` in
                class `com.android.ddmlib.MultiLineReceiver`

        []{#isCancelled()}

        -   #### isCancelled

            ``` methodSignature
            public boolean isCancelled()
            ```

        []{#getErrorMessage()}

        -   #### getErrorMessage

            ``` methodSignature
            @Nullable
            public String getErrorMessage()
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

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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.apple](package-summary.html)
:::

## Class AppleInfoPlistParsing {#class-appleinfoplistparsing .title title="Class AppleInfoPlistParsing"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.AppleInfoPlistParsing

::: description
-   

    ------------------------------------------------------------------------

        public class AppleInfoPlistParsing
        extends Object

    ::: block
    Utility class to parse Info.plist from an Apple bundle.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `sta                  | `getBundleI           | ::: block             |
        | tic Optional<String>` | dFromPlistStream​(Path | Extracts the bundle   |
        |                       |  plistPath,           | ID                    |
        |                       |                  Inpu | (CFBundleIdentifier)  |
        |                       | tStream inputStream)` | from an Info.plist,   |
        |                       |                       | returning it if       |
        |                       |                       | present.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `getBundleTypeF       | ::: block             |
        | tic Optional<String>` | romPlistStream​(Path p | Extracts the bundle   |
        |                       | listPath,             | type                  |
        |                       |                  Inpu | (CFBundlePackageType) |
        |                       | tStream inputStream)` | from an Info.plist,   |
        |                       |                       | returning it if       |
        |                       |                       | present.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static c             | `getPrope             | ::: block             |
        | om.dd.plist.NSObject` | rtyValueFromPlistStre | Extracts a property   |
        |                       | am​(Path plistPath,    | value from an         |
        |                       |                       | Info.plist, returning |
        |                       |         InputStream i | it if present.        |
        |                       | nputStream,           | :::                   |
        |                       |                       |                       |
        |                       |  String propertyKey)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `stat                 | `isWatchOSApp         | ::: block             |
        | ic Optional<Boolean>` | FromPlistStream​(Path  | Extracts the watchOS  |
        |                       | plistPath,            | app flag              |
        |                       |                  Inpu | (WKWatchKitApp) from  |
        |                       | tStream inputStream)` | an Info.plist,        |
        |                       |                       | returning it if       |
        |                       |                       | present.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBundleIdFromPlistStream(java.nio.file.Path,java.io.InputStream)}

        -   #### getBundleIdFromPlistStream

            ``` methodSignature
            public static Optional<String> getBundleIdFromPlistStream​(Path plistPath,
                                                                      InputStream inputStream)
                                                               throws IOException
            ```

            ::: block
            Extracts the bundle ID (CFBundleIdentifier) from an
            Info.plist, returning it if present.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getBundleTypeFromPlistStream(java.nio.file.Path,java.io.InputStream)}

        -   #### getBundleTypeFromPlistStream

            ``` methodSignature
            public static Optional<String> getBundleTypeFromPlistStream​(Path plistPath,
                                                                        InputStream inputStream)
                                                                 throws IOException
            ```

            ::: block
            Extracts the bundle type (CFBundlePackageType) from an
            Info.plist, returning it if present.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#isWatchOSAppFromPlistStream(java.nio.file.Path,java.io.InputStream)}

        -   #### isWatchOSAppFromPlistStream

            ``` methodSignature
            public static Optional<Boolean> isWatchOSAppFromPlistStream​(Path plistPath,
                                                                        InputStream inputStream)
                                                                 throws IOException
            ```

            ::: block
            Extracts the watchOS app flag (WKWatchKitApp) from an
            Info.plist, returning it if present.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getPropertyValueFromPlistStream(java.nio.file.Path,java.io.InputStream,java.lang.String)}

        -   #### getPropertyValueFromPlistStream

            ``` methodSignature
            public static com.dd.plist.NSObject getPropertyValueFromPlistStream​(Path plistPath,
                                                                                InputStream inputStream,
                                                                                String propertyKey)
                                                                         throws IOException
            ```

            ::: block
            Extracts a property value from an Info.plist, returning it
            if present.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`
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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

<div>

-   Summary: 
-   Nested \| 
-   Field \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

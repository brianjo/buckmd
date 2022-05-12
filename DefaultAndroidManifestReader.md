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
[Package]{.packageLabelInType} [com.facebook.buck.android](package-summary.html)
:::

## Class DefaultAndroidManifestReader {#class-defaultandroidmanifestreader .title title="Class DefaultAndroidManifestReader"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.DefaultAndroidManifestReader

::: description
-   

    All Implemented Interfaces:
    :   `AndroidManifestReader`

    ------------------------------------------------------------------------

        public class DefaultAndroidManifestReader
        extends Object
        implements AndroidManifestReader
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static A             | `forPat               | ::: block             |
        | ndroidManifestReader` | h​(Path absolutePath)` | Parses an XML given   |
        |                       |                       | via its path and      |
        |                       |                       | returns an            |
        |                       |                       | [`AndroidM            |
        |                       |                       | anifestReader`](Andro |
        |                       |                       | idManifestReader.html |
        |                       |                       |  "interface in com.fa |
        |                       |                       | cebook.buck.android") |
        |                       |                       | for it.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static A             | `forStri              | ::: block             |
        | ndroidManifestReader` | ng​(String xmlString)` | Parses an XML given   |
        |                       |                       | as a string and       |
        |                       |                       | returns an            |
        |                       |                       | [`AndroidM            |
        |                       |                       | anifestReader`](Andro |
        |                       |                       | idManifestReader.html |
        |                       |                       |  "interface in com.fa |
        |                       |                       | cebook.buck.android") |
        |                       |                       | for it.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getInstrum           |                       |
        |                       | entationTestRunner()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `List<String>`        | `get                  |                       |
        |                       | LauncherActivities()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getPackage()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getTargetPackage()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getVersionCode()`    |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
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
    -   []{#method.detail}

        ### Method Detail

        []{#getLauncherActivities()}

        -   #### getLauncherActivities

            ``` methodSignature
            public List<String> getLauncherActivities()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLauncherActivities` in
                interface `AndroidManifestReader`

            [Returns:]{.returnLabel}
            :   list of names (as they appear in the manifest) of
                activities that should appear in the Android app drawer.

        []{#getPackage()}

        -   #### getPackage

            ``` methodSignature
            public String getPackage()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPackage` in interface `AndroidManifestReader`

            [Returns:]{.returnLabel}
            :   the value of the package attribute to the manifest
                element.

        []{#getVersionCode()}

        -   #### getVersionCode

            ``` methodSignature
            public String getVersionCode()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getVersionCode` in interface `AndroidManifestReader`

            [Returns:]{.returnLabel}
            :   the value of the versionCode attribute to the manifest
                element.

        []{#getInstrumentationTestRunner()}

        -   #### getInstrumentationTestRunner

            ``` methodSignature
            public String getInstrumentationTestRunner()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getInstrumentationTestRunner` in
                interface `AndroidManifestReader`

            [Returns:]{.returnLabel}
            :   the name of the instrumentation test runner.

        []{#getTargetPackage()}

        -   #### getTargetPackage

            ``` methodSignature
            public String getTargetPackage()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTargetPackage` in interface `AndroidManifestReader`

            [Returns:]{.returnLabel}
            :   the value of the target package attribute to the
                manifest element.

        []{#forPath(java.nio.file.Path)}

        -   #### forPath

            ``` methodSignature
            public static AndroidManifestReader forPath​(Path absolutePath)
                                                 throws IOException
            ```

            ::: block
            Parses an XML given via its path and returns an
            [`AndroidManifestReader`](AndroidManifestReader.html "interface in com.facebook.buck.android")
            for it.
            :::

            [Parameters:]{.paramLabel}
            :   `absolutePath` - absolute path to an AndroidManifest.xml
                file

            [Returns:]{.returnLabel}
            :   an `AndroidManifestReader` for `path`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#forString(java.lang.String)}

        -   #### forString

            ``` methodSignature
            public static AndroidManifestReader forString​(String xmlString)
                                                   throws IOException
            ```

            ::: block
            Parses an XML given as a string and returns an
            [`AndroidManifestReader`](AndroidManifestReader.html "interface in com.facebook.buck.android")
            for it.
            :::

            [Parameters:]{.paramLabel}
            :   `xmlString` - a string representation of an XML document

            [Returns:]{.returnLabel}
            :   an `AndroidManifestReader` for the XML document

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

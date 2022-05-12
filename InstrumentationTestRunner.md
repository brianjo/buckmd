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
[Package]{.packageLabelInType} [com.facebook.buck.testrunner](package-summary.html)
:::

## Class InstrumentationTestRunner {#class-instrumentationtestrunner .title title="Class InstrumentationTestRunner"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.testrunner.InstrumentationTestRunner

::: description
-   

    ------------------------------------------------------------------------

        public class InstrumentationTestRunner
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    Description
          ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `InstrumentationTestRunner​(String adbExecutablePath,                          String deviceSerial,                          String packageName,                          String targetPackageName,                          String testRunner,                          File outputDirectory,                          String instrumentationApkPath,                          String apkUnderTestPath,                          String exopackageLocalPath,                          String apkUnderTestExopackageLocalPath,                          boolean attemptUninstallApkUnderTest,                          boolean attemptUninstallInstrumentationApk,                          boolean debug,                          boolean codeCoverage,                          String codeCoverageOutputFile,                          Map<String,​String> extraInstrumentationArguments)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static Instr         | `from                 |                       |
        | umentationTestRunner` | Args​(String... args)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `run()`               |                       |
        +-----------------------+-----------------------+-----------------------+
        | `p                    | `sy                   | ::: block             |
        | rotected static void` | ncExopackageDir​(Path  | Copy all local files  |
        |                       | localBase,            | to the remote device  |
        |                       |        com.android.dd | location              |
        |                       | mlib.IDevice device)` | :::                   |
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.lang.String,java.lang.String,java.lang.String,java.lang.String,java.lang.String,java.io.File,java.lang.String,java.lang.String,java.lang.String,java.lang.String,boolean,boolean,boolean,boolean,java.lang.String,java.util.Map)}

        -   #### InstrumentationTestRunner

                public InstrumentationTestRunner​(String adbExecutablePath,
                                                 String deviceSerial,
                                                 String packageName,
                                                 String targetPackageName,
                                                 String testRunner,
                                                 File outputDirectory,
                                                 String instrumentationApkPath,
                                                 String apkUnderTestPath,
                                                 String exopackageLocalPath,
                                                 String apkUnderTestExopackageLocalPath,
                                                 boolean attemptUninstallApkUnderTest,
                                                 boolean attemptUninstallInstrumentationApk,
                                                 boolean debug,
                                                 boolean codeCoverage,
                                                 String codeCoverageOutputFile,
                                                 Map<String,​String> extraInstrumentationArguments)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#fromArgs(java.lang.String...)}

        -   #### fromArgs

            ``` methodSignature
            public static InstrumentationTestRunner fromArgs​(String... args)
            ```

        []{#run()}

        -   #### run

            ``` methodSignature
            public void run()
                     throws Throwable
            ```

            [Throws:]{.throwsLabel}
            :   `Throwable`

        []{#syncExopackageDir(java.nio.file.Path,com.android.ddmlib.IDevice)}

        -   #### syncExopackageDir

            ``` methodSignature
            protected static void syncExopackageDir​(Path localBase,
                                                    com.android.ddmlib.IDevice device)
                                             throws Exception
            ```

            ::: block
            Copy all local files to the remote device location
            :::

            [Throws:]{.throwsLabel}
            :   `Exception`
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

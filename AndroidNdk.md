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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.android.toolchain.ndk](package-summary.html)
:::

## Class AndroidNdk {#class-androidndk .title title="Class AndroidNdk"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.toolchain.ndk.AndroidNdk

::: description
-   

    All Implemented Interfaces:
    :   `ComparableToolchain`, `Toolchain`, `ToolchainWithCapability`

    ------------------------------------------------------------------------

        public abstract class AndroidNdk
        extends Object
        implements ComparableToolchain

    ::: block
    Part of Android toolchain that provides access to Android NDK
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field            Description
          ------------------- ---------------- -------------
          `static String`     `DEFAULT_NAME`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor      Description
          ---------------- -------------
          `AndroidNdk()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `protected abstr      | `g                    |                       |
        | act ExecutableFinder` | etExecutableFinder()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getName()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `get                  |                       |
        |                       | NdkBuildExecutable()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Path`       | `getNdkRootPath()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract String`     | `getNdkVersion()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static AndroidNdk`   | `of​(String ndkVersi   |                       |
        |                       | on,   Path ndkRootPat |                       |
        |                       | h,   boolean shouldEs |                       |
        |                       | capeCFlagsInDoubleQuo |                       |
        |                       | tes,   ExecutableFind |                       |
        |                       | er executableFinder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract boolean`    | `shouldEscapeCF       | ::: block             |
        |                       | lagsInDoubleQuotes()` | Escaping logic can be |
        |                       |                       | different and depends |
        |                       |                       | on the version of     |
        |                       |                       | Android NDK.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#DEFAULT_NAME}

        -   #### DEFAULT_NAME

                public static final String DEFAULT_NAME

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.android.toolchain.ndk.AndroidNdk.DEFAULT_NAME)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### AndroidNdk

                public AndroidNdk()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getName()}

        -   #### getName

            ``` methodSignature
            public String getName()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getName` in interface `Toolchain`

        []{#getNdkVersion()}

        -   #### getNdkVersion

            ``` methodSignature
            public abstract String getNdkVersion()
            ```

        []{#getNdkRootPath()}

        -   #### getNdkRootPath

            ``` methodSignature
            public abstract Path getNdkRootPath()
            ```

        []{#shouldEscapeCFlagsInDoubleQuotes()}

        -   #### shouldEscapeCFlagsInDoubleQuotes

            ``` methodSignature
            public abstract boolean shouldEscapeCFlagsInDoubleQuotes()
            ```

            ::: block
            Escaping logic can be different and depends on the version
            of Android NDK.
            :::

        []{#getExecutableFinder()}

        -   #### getExecutableFinder

            ``` methodSignature
            @Auxiliary
            protected abstract ExecutableFinder getExecutableFinder()
            ```

        []{#getNdkBuildExecutable()}

        -   #### getNdkBuildExecutable

            ``` methodSignature
            @Lazy
            public Path getNdkBuildExecutable()
            ```

        []{#of(java.lang.String,java.nio.file.Path,boolean,com.facebook.buck.io.ExecutableFinder)}

        -   #### of

            ``` methodSignature
            public static AndroidNdk of​(String ndkVersion,
                                        Path ndkRootPath,
                                        boolean shouldEscapeCFlagsInDoubleQuotes,
                                        ExecutableFinder executableFinder)
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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

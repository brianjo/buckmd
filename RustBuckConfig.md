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
[Package]{.packageLabelInType} [com.facebook.buck.features.rust](package-summary.html)
:::

## Class RustBuckConfig {#class-rustbuckconfig .title title="Class RustBuckConfig"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.rust.RustBuckConfig

::: description
-   

    ------------------------------------------------------------------------

        public class RustBuckConfig
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                             Description
          --------------------------------------- -------------
          `RustBuckConfig​(BuckConfig delegate)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Optional<Path>`      | `getAppl              |                       |
        |                       | eDeveloperDirIfSet()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Path>`      | `getAppleXcrunPath()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getLinkerFl          |                       |
        | ogle.common.collect.I | ags​(String platform)` |                       |
        | mmutableList<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<            | `getLinkerPlatf       |                       |
        | LinkerProvider.Type>` | orm​(String platform)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getRustcBinaryFl     | ::: block             |
        | ogle.common.collect.I | ags​(String platform)` | Get rustc flags for   |
        | mmutableList<String>` |                       | rust_binary() rules.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getRustcCheckFl      | ::: block             |
        | ogle.common.collect.I | ags​(String platform)` | Get rustc flags for   |
        | mmutableList<String>` |                       | #check flavored       |
        |                       |                       | builds.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getRustcLibraryFl    | ::: block             |
        | ogle.common.collect.I | ags​(String platform)` | Get rustc flags for   |
        | mmutableList<String>` |                       | rust_library() rules. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Op                   | `getRustCompi         |                       |
        | tional<ToolProvider>` | ler​(String platform)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getRustcTestFl       | ::: block             |
        | ogle.common.collect.I | ags​(String platform)` | Get rustc flags for   |
        | mmutableList<String>` |                       | rust_test() rules.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Op                   | `getRustLin           |                       |
        | tional<ToolProvider>` | ker​(String platform)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
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

        []{#<init>(com.facebook.buck.core.config.BuckConfig)}

        -   #### RustBuckConfig

                public RustBuckConfig​(BuckConfig delegate)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getRustCompiler(java.lang.String)}

        -   #### getRustCompiler

            ``` methodSignature
            public Optional<ToolProvider> getRustCompiler​(String platform)
            ```

        []{#getRustcLibraryFlags(java.lang.String)}

        -   #### getRustcLibraryFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getRustcLibraryFlags​(String platform)
            ```

            ::: block
            Get rustc flags for rust_library() rules.
            :::

            [Returns:]{.returnLabel}
            :   List of rustc_library_flags, as well as common
                rustc_flags.

        []{#getRustcBinaryFlags(java.lang.String)}

        -   #### getRustcBinaryFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getRustcBinaryFlags​(String platform)
            ```

            ::: block
            Get rustc flags for rust_binary() rules.
            :::

            [Returns:]{.returnLabel}
            :   List of rustc_binary_flags, as well as common
                rustc_flags.

        []{#getRustcTestFlags(java.lang.String)}

        -   #### getRustcTestFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getRustcTestFlags​(String platform)
            ```

            ::: block
            Get rustc flags for rust_test() rules.
            :::

            [Returns:]{.returnLabel}
            :   List of rustc_test_flags, as well as common rustc_flags.

        []{#getRustcCheckFlags(java.lang.String)}

        -   #### getRustcCheckFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getRustcCheckFlags​(String platform)
            ```

            ::: block
            Get rustc flags for #check flavored builds. Caller must also
            include rule-dependent flags and common flags.
            :::

            [Returns:]{.returnLabel}
            :   List of rustc_check_flags.

        []{#getRustLinker(java.lang.String)}

        -   #### getRustLinker

            ``` methodSignature
            public Optional<ToolProvider> getRustLinker​(String platform)
            ```

        []{#getLinkerPlatform(java.lang.String)}

        -   #### getLinkerPlatform

            ``` methodSignature
            public Optional<LinkerProvider.Type> getLinkerPlatform​(String platform)
            ```

        []{#getLinkerFlags(java.lang.String)}

        -   #### getLinkerFlags

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getLinkerFlags​(String platform)
            ```

        []{#getAppleXcrunPath()}

        -   #### getAppleXcrunPath

            ``` methodSignature
            public Optional<Path> getAppleXcrunPath()
            ```

        []{#getAppleDeveloperDirIfSet()}

        -   #### getAppleDeveloperDirIfSet

            ``` methodSignature
            public Optional<Path> getAppleDeveloperDirIfSet()
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

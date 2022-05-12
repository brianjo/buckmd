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
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.core](package-summary.html)
:::

## Class JavaAbis {#class-javaabis .title title="Class JavaAbis"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.core.JavaAbis

::: description
-   

    ------------------------------------------------------------------------

        public class JavaAbis
        extends Object

    ::: block
    Provides some utilities for dealing with Java abis and abi rules.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                          Description
          ------------------- ------------------------------ -------------
          `static Flavor`     `CLASS_ABI_FLAVOR`              
          `static Flavor`     `SOURCE_ABI_FLAVOR`             
          `static Flavor`     `SOURCE_ONLY_ABI_FLAVOR`        
          `static Flavor`     `VERIFIED_SOURCE_ABI_FLAVOR`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static BuildTarget`  | `                     |                       |
        |                       | getClassAbiJar​(BuildT |                       |
        |                       | arget libraryTarget)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static BuildTarget`  | `getLibraryTarget​(Bu  | ::: block             |
        |                       | ildTarget abiTarget)` | Returns the library   |
        |                       |                       | target for an abi     |
        |                       |                       | target.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static BuildTarget`  | `g                    |                       |
        |                       | etSourceAbiJar​(BuildT |                       |
        |                       | arget libraryTarget)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static BuildTarget`  | `getSo                |                       |
        |                       | urceOnlyAbiJar​(BuildT |                       |
        |                       | arget libraryTarget)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Path`         | `getTmpGe             |                       |
        |                       | nPathForSourceAbi​(Pro |                       |
        |                       | jectFilesystem projec |                       |
        |                       | tFilesystem,          |                       |
        |                       |                  Buil |                       |
        |                       | dTarget buildTarget)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static BuildTarget`  | `getVerifi            |                       |
        |                       | edSourceAbiJar​(BuildT |                       |
        |                       | arget libraryTarget)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `isAbiTarget          | ::: block             |
        |                       | ​(BuildTarget target)` | Returns whether this  |
        |                       |                       | target is an abi      |
        |                       |                       | target.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `isClassAbiTarget     |                       |
        |                       | ​(BuildTarget target)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `isLibraryTarget      |                       |
        |                       | ​(BuildTarget target)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `isSourceAbiTarget    |                       |
        |                       | ​(BuildTarget target)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `                     |                       |
        |                       | isSourceOnlyAbiTarget |                       |
        |                       | ​(BuildTarget target)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `isVe                 |                       |
        |                       | rifiedSourceAbiTarget |                       |
        |                       | ​(BuildTarget target)` |                       |
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
    -   []{#field.detail}

        ### Field Detail

        []{#CLASS_ABI_FLAVOR}

        -   #### CLASS_ABI_FLAVOR

                public static final Flavor CLASS_ABI_FLAVOR

        []{#SOURCE_ABI_FLAVOR}

        -   #### SOURCE_ABI_FLAVOR

                public static final Flavor SOURCE_ABI_FLAVOR

        []{#SOURCE_ONLY_ABI_FLAVOR}

        -   #### SOURCE_ONLY_ABI_FLAVOR

                public static final Flavor SOURCE_ONLY_ABI_FLAVOR

        []{#VERIFIED_SOURCE_ABI_FLAVOR}

        -   #### VERIFIED_SOURCE_ABI_FLAVOR

                public static final Flavor VERIFIED_SOURCE_ABI_FLAVOR
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getClassAbiJar(com.facebook.buck.core.model.BuildTarget)}

        -   #### getClassAbiJar

            ``` methodSignature
            public static BuildTarget getClassAbiJar​(BuildTarget libraryTarget)
            ```

        []{#isAbiTarget(com.facebook.buck.core.model.BuildTarget)}

        -   #### isAbiTarget

            ``` methodSignature
            public static boolean isAbiTarget​(BuildTarget target)
            ```

            ::: block
            Returns whether this target is an abi target.
            :::

        []{#isClassAbiTarget(com.facebook.buck.core.model.BuildTarget)}

        -   #### isClassAbiTarget

            ``` methodSignature
            public static boolean isClassAbiTarget​(BuildTarget target)
            ```

        []{#getSourceAbiJar(com.facebook.buck.core.model.BuildTarget)}

        -   #### getSourceAbiJar

            ``` methodSignature
            public static BuildTarget getSourceAbiJar​(BuildTarget libraryTarget)
            ```

        []{#isSourceAbiTarget(com.facebook.buck.core.model.BuildTarget)}

        -   #### isSourceAbiTarget

            ``` methodSignature
            public static boolean isSourceAbiTarget​(BuildTarget target)
            ```

        []{#getSourceOnlyAbiJar(com.facebook.buck.core.model.BuildTarget)}

        -   #### getSourceOnlyAbiJar

            ``` methodSignature
            public static BuildTarget getSourceOnlyAbiJar​(BuildTarget libraryTarget)
            ```

        []{#isSourceOnlyAbiTarget(com.facebook.buck.core.model.BuildTarget)}

        -   #### isSourceOnlyAbiTarget

            ``` methodSignature
            public static boolean isSourceOnlyAbiTarget​(BuildTarget target)
            ```

        []{#getVerifiedSourceAbiJar(com.facebook.buck.core.model.BuildTarget)}

        -   #### getVerifiedSourceAbiJar

            ``` methodSignature
            public static BuildTarget getVerifiedSourceAbiJar​(BuildTarget libraryTarget)
            ```

        []{#isVerifiedSourceAbiTarget(com.facebook.buck.core.model.BuildTarget)}

        -   #### isVerifiedSourceAbiTarget

            ``` methodSignature
            public static boolean isVerifiedSourceAbiTarget​(BuildTarget target)
            ```

        []{#isLibraryTarget(com.facebook.buck.core.model.BuildTarget)}

        -   #### isLibraryTarget

            ``` methodSignature
            public static boolean isLibraryTarget​(BuildTarget target)
            ```

        []{#getLibraryTarget(com.facebook.buck.core.model.BuildTarget)}

        -   #### getLibraryTarget

            ``` methodSignature
            public static BuildTarget getLibraryTarget​(BuildTarget abiTarget)
            ```

            ::: block
            Returns the library target for an abi target.
            :::

        []{#getTmpGenPathForSourceAbi(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.model.BuildTarget)}

        -   #### getTmpGenPathForSourceAbi

            ``` methodSignature
            public static Path getTmpGenPathForSourceAbi​(ProjectFilesystem projectFilesystem,
                                                         BuildTarget buildTarget)
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
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

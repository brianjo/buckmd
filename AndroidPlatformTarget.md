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
[Package]{.packageLabelInType} [com.facebook.buck.android.toolchain](package-summary.html)
:::

## Class AndroidPlatformTarget {#class-androidplatformtarget .title title="Class AndroidPlatformTarget"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.toolchain.AndroidPlatformTarget

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`, `Toolchain`

    ------------------------------------------------------------------------

        public abstract class AndroidPlatformTarget
        extends Object
        implements Toolchain, AddsToRuleKey

    ::: block
    Represents a platform to target for Android. Eventually, it should
    be possible to construct an arbitrary platform target, but
    currently, we only recognize a fixed set of targets.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                               Description
          ------------------- ----------------------------------- -------------
          `static String`     `DEFAULT_ANDROID_PLATFORM_TARGET`    
          `static String`     `DEFAULT_NAME`                       

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                 Description
          --------------------------- -------------
          `AndroidPlatformTarget()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `add                  | ::: block             |
        |                       | ParseTimeDeps​(com.goo | Process aapt2 tool\'s |
        |                       | gle.common.collect.Im | parse dependencies    |
        |                       | mutableCollection.Bui | and adds them to the  |
        |                       | lder<BuildTarget> bui | `builder`             |
        |                       | lder,                 | :::                   |
        |                       |  TargetConfiguration  |                       |
        |                       | targetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `a                    | `ge                   |                       |
        | bstract ToolProvider` | tAapt2ToolProvider()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `a                    | `getAaptExecutable()` |                       |
        | bstract java.util.fun |                       |                       |
        | ction.Supplier<Tool>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Path`       | `getAdbExecutable()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Path`       | `getAidlExecutable()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Path`       | `getAndro             |                       |
        |                       | idFrameworkIdlFile()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Path`       | `getAndroidJar()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract List<Path>` | `getBo                |                       |
        |                       | otclasspathEntries()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Path`       | `getDxExecutable()`   |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getName()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Path`       | `getOptim             |                       |
        |                       | izedProguardConfig()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract String`     | `getPlatformName()`   | ::: block             |
        |                       |                       | This is likely        |
        |                       |                       | something like        |
        |                       |                       | `"Google I            |
        |                       |                       | nc.:Google APIs:21"`. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Path`       | `getProguardConfig()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Path`       | `getProguardJar()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Path`       | `get                  |                       |
        |                       | ZipalignExecutable()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static A             | `of​(Stri              |                       |
        | ndroidPlatformTarget` | ng platformName,   Pa |                       |
        |                       | th androidJar,   List |                       |
        |                       | <Path> bootclasspathE |                       |
        |                       | ntries,   java.util.f |                       |
        |                       | unction.Supplier<Tool |                       |
        |                       | > aaptExecutable,   T |                       |
        |                       | oolProvider aapt2Tool |                       |
        |                       | Provider,   Path adbE |                       |
        |                       | xecutable,   Path aid |                       |
        |                       | lExecutable,   Path z |                       |
        |                       | ipalignExecutable,    |                       |
        |                       | Path dxExecutable,    |                       |
        |                       | Path androidFramework |                       |
        |                       | IdlFile,   Path progu |                       |
        |                       | ardJar,   Path progua |                       |
        |                       | rdConfig,   Path opti |                       |
        |                       | mizedProguardConfig)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          |                       |
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

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, wait, wait, wait`
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
                Values](../../../../../constant-values.html#com.facebook.buck.android.toolchain.AndroidPlatformTarget.DEFAULT_NAME)

        []{#DEFAULT_ANDROID_PLATFORM_TARGET}

        -   #### DEFAULT_ANDROID_PLATFORM_TARGET

                public static final String DEFAULT_ANDROID_PLATFORM_TARGET

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.android.toolchain.AndroidPlatformTarget.DEFAULT_ANDROID_PLATFORM_TARGET)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### AndroidPlatformTarget

                public AndroidPlatformTarget()
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

        []{#getPlatformName()}

        -   #### getPlatformName

            ``` methodSignature
            public abstract String getPlatformName()
            ```

            ::: block
            This is likely something like
            `"Google Inc.:Google APIs:21"`.
            :::

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

        []{#getAndroidJar()}

        -   #### getAndroidJar

            ``` methodSignature
            public abstract Path getAndroidJar()
            ```

        []{#getBootclasspathEntries()}

        -   #### getBootclasspathEntries

            ``` methodSignature
            public abstract List<Path> getBootclasspathEntries()
            ```

            [Returns:]{.returnLabel}
            :   bootclasspath entries as absolute
                [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}s

        []{#getAaptExecutable()}

        -   #### getAaptExecutable

            ``` methodSignature
            public abstract java.util.function.Supplier<Tool> getAaptExecutable()
            ```

        []{#getAapt2ToolProvider()}

        -   #### getAapt2ToolProvider

            ``` methodSignature
            public abstract ToolProvider getAapt2ToolProvider()
            ```

        []{#getAdbExecutable()}

        -   #### getAdbExecutable

            ``` methodSignature
            public abstract Path getAdbExecutable()
            ```

        []{#getAidlExecutable()}

        -   #### getAidlExecutable

            ``` methodSignature
            public abstract Path getAidlExecutable()
            ```

        []{#getZipalignExecutable()}

        -   #### getZipalignExecutable

            ``` methodSignature
            public abstract Path getZipalignExecutable()
            ```

        []{#getDxExecutable()}

        -   #### getDxExecutable

            ``` methodSignature
            public abstract Path getDxExecutable()
            ```

        []{#getAndroidFrameworkIdlFile()}

        -   #### getAndroidFrameworkIdlFile

            ``` methodSignature
            public abstract Path getAndroidFrameworkIdlFile()
            ```

        []{#getProguardJar()}

        -   #### getProguardJar

            ``` methodSignature
            public abstract Path getProguardJar()
            ```

        []{#getProguardConfig()}

        -   #### getProguardConfig

            ``` methodSignature
            public abstract Path getProguardConfig()
            ```

        []{#getOptimizedProguardConfig()}

        -   #### getOptimizedProguardConfig

            ``` methodSignature
            public abstract Path getOptimizedProguardConfig()
            ```

        []{#addParseTimeDeps(com.google.common.collect.ImmutableCollection.Builder,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### addParseTimeDeps

            ``` methodSignature
            @Derived
            public void addParseTimeDeps​(com.google.common.collect.ImmutableCollection.Builder<BuildTarget> builder,
                                         TargetConfiguration targetConfiguration)
            ```

            ::: block
            Process aapt2 tool\'s parse dependencies and adds them to
            the `builder`
            :::

        []{#of(java.lang.String,java.nio.file.Path,java.util.List,java.util.function.Supplier,com.facebook.buck.core.toolchain.toolprovider.ToolProvider,java.nio.file.Path,java.nio.file.Path,java.nio.file.Path,java.nio.file.Path,java.nio.file.Path,java.nio.file.Path,java.nio.file.Path,java.nio.file.Path)}

        -   #### of

            ``` methodSignature
            public static AndroidPlatformTarget of​(String platformName,
                                                   Path androidJar,
                                                   List<Path> bootclasspathEntries,
                                                   java.util.function.Supplier<Tool> aaptExecutable,
                                                   ToolProvider aapt2ToolProvider,
                                                   Path adbExecutable,
                                                   Path aidlExecutable,
                                                   Path zipalignExecutable,
                                                   Path dxExecutable,
                                                   Path androidFrameworkIdlFile,
                                                   Path proguardJar,
                                                   Path proguardConfig,
                                                   Path optimizedProguardConfig)
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

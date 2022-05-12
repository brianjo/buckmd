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
[Package]{.packageLabelInType} [com.facebook.buck.util.env](package-summary.html)
:::

## Class BuckClasspath {#class-buckclasspath .title title="Class BuckClasspath"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.env.BuckClasspath

::: description
-   

    ------------------------------------------------------------------------

        public class BuckClasspath
        extends Object

    ::: block
    Current process classpath. Set by buckd or by launcher script.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                      Description
          ------------------- -------------------------- -------------
          `static String`     `BOOTSTRAP_ENV_VAR_NAME`    
          `static String`     `ENV_VAR_NAME`              
          `static String`     `TEST_ENV_VAR_NAME`         

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor         Description
          ------------------- -------------
          `BuckClasspath()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static com.          | `get                  | ::: block             |
        | google.common.collect | BootstrapClasspath()` | Returns Buck\'s       |
        | .ImmutableList<Path>` |                       | \"bootstrap\"         |
        |                       |                       | classpath.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `ge                   |                       |
        |                       | tBuckBootstrapClasspa |                       |
        |                       | thFromEnvVarOrNull()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static com.          | `getBuckCl            | ::: block             |
        | google.common.collect | asspathForIntellij()` | Return Buck\'s        |
        | .ImmutableList<Path>` |                       | classpath when        |
        |                       |                       | running under         |
        |                       |                       | Intellij.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `getBuckClasspa       |                       |
        |                       | thFromEnvVarOrNull()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `getBuckClasspat      |                       |
        |                       | hFromEnvVarOrThrow()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static com.          | `getClasspath()`      | ::: block             |
        | google.common.collect |                       | Returns Buck\'s       |
        | .ImmutableList<Path>` |                       | classpath.            |
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
    -   []{#field.detail}

        ### Field Detail

        []{#ENV_VAR_NAME}

        -   #### ENV_VAR_NAME

                public static final String ENV_VAR_NAME

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.env.BuckClasspath.ENV_VAR_NAME)

        []{#BOOTSTRAP_ENV_VAR_NAME}

        -   #### BOOTSTRAP_ENV_VAR_NAME

                public static final String BOOTSTRAP_ENV_VAR_NAME

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.env.BuckClasspath.BOOTSTRAP_ENV_VAR_NAME)

        []{#TEST_ENV_VAR_NAME}

        -   #### TEST_ENV_VAR_NAME

                public static final String TEST_ENV_VAR_NAME

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.env.BuckClasspath.TEST_ENV_VAR_NAME)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### BuckClasspath

                public BuckClasspath()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBuckClasspathFromEnvVarOrThrow()}

        -   #### getBuckClasspathFromEnvVarOrThrow

            ``` methodSignature
            public static String getBuckClasspathFromEnvVarOrThrow()
            ```

        []{#getBuckClasspathFromEnvVarOrNull()}

        -   #### getBuckClasspathFromEnvVarOrNull

            ``` methodSignature
            @Nullable
            public static String getBuckClasspathFromEnvVarOrNull()
            ```

        []{#getBuckBootstrapClasspathFromEnvVarOrNull()}

        -   #### getBuckBootstrapClasspathFromEnvVarOrNull

            ``` methodSignature
            @Nullable
            public static String getBuckBootstrapClasspathFromEnvVarOrNull()
            ```

        []{#getBootstrapClasspath()}

        -   #### getBootstrapClasspath

            ``` methodSignature
            public static com.google.common.collect.ImmutableList<Path> getBootstrapClasspath()
                                                                                       throws IOException
            ```

            ::: block
            Returns Buck\'s \"bootstrap\" classpath. See
            ClassLoaderBootstrapper.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getClasspath()}

        -   #### getClasspath

            ``` methodSignature
            public static com.google.common.collect.ImmutableList<Path> getClasspath()
                                                                              throws IOException
            ```

            ::: block
            Returns Buck\'s classpath.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getBuckClasspathForIntellij()}

        -   #### getBuckClasspathForIntellij

            ``` methodSignature
            public static com.google.common.collect.ImmutableList<Path> getBuckClasspathForIntellij()
                                                                                             throws IOException
            ```

            ::: block
            Return Buck\'s classpath when running under Intellij. Use
            getClasspath() or getBootstrapClasspath() instead.
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

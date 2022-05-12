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
[Package]{.packageLabelInType} [com.facebook.buck.android.agent.util](package-summary.html)
:::

## Class AgentUtil {#class-agentutil .title title="Class AgentUtil"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.agent.util.AgentUtil

::: description
-   

    ------------------------------------------------------------------------

        public final class AgentUtil
        extends Object

    ::: block
    Non-instantiable class for holding functionality that runs both on
    the host and in the android agent.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Field                 | Description           |
        +=======================+=======================+=======================+
        | `static String`       | `AGENT_PACKAGE_NAME`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `AGENT_VERSION_CODE`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static int`          | `BI                   | ::: block             |
        |                       | NARY_SECRET_KEY_SIZE` | Size in bytes of the  |
        |                       |                       | binary data use to    |
        |                       |                       | generate the secret   |
        |                       |                       | key for receive-file. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `TEMP_PREFIX`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static int`          | `                     | ::: block             |
        |                       | TEXT_SECRET_KEY_SIZE` | Size of the text      |
        |                       |                       | version of the        |
        |                       |                       | receive-file secret   |
        |                       |                       | key.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                  Description
          ------------------- --------------------------------------- -------------
          `static String`     `getJarSignature​(String packagePath)`    

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

        []{#AGENT_PACKAGE_NAME}

        -   #### AGENT_PACKAGE_NAME

                public static final String AGENT_PACKAGE_NAME

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.android.agent.util.AgentUtil.AGENT_PACKAGE_NAME)

        []{#AGENT_VERSION_CODE}

        -   #### AGENT_VERSION_CODE

                public static final String AGENT_VERSION_CODE

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.android.agent.util.AgentUtil.AGENT_VERSION_CODE)

        []{#BINARY_SECRET_KEY_SIZE}

        -   #### BINARY_SECRET_KEY_SIZE

                public static final int BINARY_SECRET_KEY_SIZE

            ::: block
            Size in bytes of the binary data use to generate the secret
            key for receive-file.
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.android.agent.util.AgentUtil.BINARY_SECRET_KEY_SIZE)

        []{#TEXT_SECRET_KEY_SIZE}

        -   #### TEXT_SECRET_KEY_SIZE

                public static final int TEXT_SECRET_KEY_SIZE

            ::: block
            Size of the text version of the receive-file secret key.
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.android.agent.util.AgentUtil.TEXT_SECRET_KEY_SIZE)

        []{#TEMP_PREFIX}

        -   #### TEMP_PREFIX

                public static final String TEMP_PREFIX

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.android.agent.util.AgentUtil.TEMP_PREFIX)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getJarSignature(java.lang.String)}

        -   #### getJarSignature

            ``` methodSignature
            public static String getJarSignature​(String packagePath)
                                          throws IOException
            ```

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

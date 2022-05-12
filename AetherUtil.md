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
[Package]{.packageLabelInType} [com.facebook.buck.maven.aether](package-summary.html)
:::

## Class AetherUtil {#class-aetherutil .title title="Class AetherUtil"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.maven.aether.AetherUtil

::: description
-   

    ------------------------------------------------------------------------

        public class AetherUtil
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                  Description
          ------------------- ---------------------- -------------
          `static String`     `CLASSIFIER_SOURCES`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static String`       | `add                  | ::: block             |
        |                       | Classifier​(String mav | Transforms maven      |
        |                       | enCoords,             | coordinates, adding   |
        |                       |   String classifier)` | the specified         |
        |                       |                       | classifier            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static org.          | `                     |                       |
        | eclipse.aether.spi.lo | initServiceLocator()` |                       |
        | cator.ServiceLocator` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static org.e         | `toRemoteReposit      |                       |
        | clipse.aether.reposit | ory​(Repository repo)` |                       |
        | ory.RemoteRepository` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static org.e         | `toRemoteRepository​(S |                       |
        | clipse.aether.reposit | tring repoUrl,        |                       |
        | ory.RemoteRepository` |             Optional< |                       |
        |                       | String> username,     |                       |
        |                       |                Option |                       |
        |                       | al<String> password)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static org.e         | `toRemoteRepositor    |                       |
        | clipse.aether.reposit | y​(URL repoUrl,        |                       |
        | ory.RemoteRepository` |             Optional< |                       |
        |                       | String> username,     |                       |
        |                       |                Option |                       |
        |                       | al<String> password)` |                       |
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

        []{#CLASSIFIER_SOURCES}

        -   #### CLASSIFIER_SOURCES

                public static final String CLASSIFIER_SOURCES

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.maven.aether.AetherUtil.CLASSIFIER_SOURCES)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#toRemoteRepository(java.net.URL,java.util.Optional,java.util.Optional)}

        -   #### toRemoteRepository

            ``` methodSignature
            public static org.eclipse.aether.repository.RemoteRepository toRemoteRepository​(URL repoUrl,
                                                                                            Optional<String> username,
                                                                                            Optional<String> password)
            ```

        []{#toRemoteRepository(java.lang.String,java.util.Optional,java.util.Optional)}

        -   #### toRemoteRepository

            ``` methodSignature
            public static org.eclipse.aether.repository.RemoteRepository toRemoteRepository​(String repoUrl,
                                                                                            Optional<String> username,
                                                                                            Optional<String> password)
            ```

        []{#toRemoteRepository(com.facebook.buck.maven.aether.Repository)}

        -   #### toRemoteRepository

            ``` methodSignature
            public static org.eclipse.aether.repository.RemoteRepository toRemoteRepository​(Repository repo)
            ```

        []{#initServiceLocator()}

        -   #### initServiceLocator

            ``` methodSignature
            public static org.eclipse.aether.spi.locator.ServiceLocator initServiceLocator()
            ```

        []{#addClassifier(java.lang.String,java.lang.String)}

        -   #### addClassifier

            ``` methodSignature
            public static String addClassifier​(String mavenCoords,
                                               String classifier)
            ```

            ::: block
            Transforms maven coordinates, adding the specified
            classifier
            :::
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

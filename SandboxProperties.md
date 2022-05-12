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
-   [Nested](#nested.class.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.sandbox](package-summary.html)
:::

## Class SandboxProperties {#class-sandboxproperties .title title="Class SandboxProperties"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.sandbox.SandboxProperties

::: description
-   

    ------------------------------------------------------------------------

        public abstract class SandboxProperties
        extends Object

    ::: block
    A set of properties for a single execution of a process under a
    sandbox.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                         Description
          ------------------- ----------------------------- -------------
          `static class `     `SandboxProperties.Builder`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor             Description
          ----------------------- -------------
          `SandboxProperties()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static Sandb         | `builder()`           |                       |
        | oxProperties.Builder` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract com.g       | `getAllowedT          | ::: block             |
        | oogle.common.collect. | oReadMetadataPaths()` | Paths which metadata  |
        | ImmutableSet<String>` |                       | is allowed to be read |
        |                       |                       | during process        |
        |                       |                       | execution.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract com.g       | `get                  | ::: block             |
        | oogle.common.collect. | AllowedToReadPaths()` | Paths that are        |
        | ImmutableSet<String>` |                       | allowed to be read    |
        |                       |                       | during process        |
        |                       |                       | execution.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract com.g       | `getA                 | ::: block             |
        | oogle.common.collect. | llowedToWritePaths()` | Paths that are        |
        | ImmutableSet<String>` |                       | allowed to be writen  |
        |                       |                       | during process        |
        |                       |                       | execution.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract com.g       | `ge                   | ::: block             |
        | oogle.common.collect. | tDeniedToReadPaths()` | Paths that are not    |
        | ImmutableSet<String>` |                       | allowed to be read    |
        |                       |                       | during process        |
        |                       |                       | execution.            |
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### SandboxProperties

                public SandboxProperties()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getDeniedToReadPaths()}

        -   #### getDeniedToReadPaths

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSet<String> getDeniedToReadPaths()
            ```

            ::: block
            Paths that are not allowed to be read during process
            execution.
            :::

        []{#getAllowedToReadPaths()}

        -   #### getAllowedToReadPaths

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSet<String> getAllowedToReadPaths()
            ```

            ::: block
            Paths that are allowed to be read during process execution.
            :::

        []{#getAllowedToReadMetadataPaths()}

        -   #### getAllowedToReadMetadataPaths

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSet<String> getAllowedToReadMetadataPaths()
            ```

            ::: block
            Paths which metadata is allowed to be read during process
            execution.
            :::

        []{#getAllowedToWritePaths()}

        -   #### getAllowedToWritePaths

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSet<String> getAllowedToWritePaths()
            ```

            ::: block
            Paths that are allowed to be writen during process
            execution.
            :::

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static SandboxProperties.Builder builder()
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
-   [Nested](#nested.class.summary) \| 
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

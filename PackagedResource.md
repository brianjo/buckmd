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
[Package]{.packageLabelInType} [com.facebook.buck.android](package-summary.html)
:::

## Class PackagedResource {#class-packagedresource .title title="Class PackagedResource"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.PackagedResource

::: description
-   

    All Implemented Interfaces:
    :   `java.util.function.Supplier<Path>`

    ------------------------------------------------------------------------

        public class PackagedResource
        extends Object
        implements java.util.function.Supplier<Path>

    ::: block
    Represents a zip that has been packaged as a resource with Buck, but
    which should be expanded at most once during Buck\'s execution (not
    per-build).
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                         Description
          ----------------------------------------------------------------------------------------------------------------------------------- -------------
          `PackagedResource​(ProjectFilesystem filesystem,                 Class<?> relativeTo,                 String pathRelativeToClass)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Path`                | `get()`               |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getFilenamePath()`   | ::: block             |
        |                       |                       | Use this combined     |
        |                       |                       | with file hash as     |
        |                       |                       | unique ID when        |
        |                       |                       | hashing is enabled.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `get                  | ::: block             |
        |                       | ResourceIdentifier()` | Use this as unique ID |
        |                       |                       | for resource when     |
        |                       |                       | hashing is not        |
        |                       |                       | enabled               |
        |                       |                       | :::                   |
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

        []{#<init>(com.facebook.buck.io.filesystem.ProjectFilesystem,java.lang.Class,java.lang.String)}

        -   #### PackagedResource

                public PackagedResource​(ProjectFilesystem filesystem,
                                        Class<?> relativeTo,
                                        String pathRelativeToClass)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#get()}

        -   #### get

            ``` methodSignature
            public Path get()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `get` in interface `java.util.function.Supplier<Path>`

        []{#getResourceIdentifier()}

        -   #### getResourceIdentifier

            ``` methodSignature
            public String getResourceIdentifier()
            ```

            ::: block
            Use this as unique ID for resource when hashing is not
            enabled
            :::

            [Returns:]{.returnLabel}
            :   Class name followed by relative file path. E.g.
                com.facebook.buck.MyClass#some_resource_file.abc

        []{#getFilenamePath()}

        -   #### getFilenamePath

            ``` methodSignature
            public Path getFilenamePath()
            ```

            ::: block
            Use this combined with file hash as unique ID when hashing
            is enabled.
            :::

            [Returns:]{.returnLabel}
            :   [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
                representing filename of packaged resource
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

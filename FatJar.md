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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java](package-summary.html)
:::

## Class FatJar {#class-fatjar .title title="Class FatJar"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.FatJar

::: description
-   

    All Implemented Interfaces:
    :   `Serializable`

    ------------------------------------------------------------------------

        public class FatJar
        extends Object
        implements Serializable

    ::: block
    Helper class for unpacking fat JAR resources.
    :::

    [See Also:]{.seeLabel}
    :   [Serialized
        Form](../../../../../serialized-form.html#com.facebook.buck.jvm.java.FatJar)
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                     Description
          ------------------- ------------------------- -------------
          `static String`     `FAT_JAR_INFO_RESOURCE`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                           Description
          --------------------------------------------------------------------- -------------
          `FatJar​(String innerJar,       Map<String,​String> nativeLibraries)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static FatJar`       | `load                 |                       |
        |                       | ​(ClassLoader loader)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `store​(Output         | ::: block             |
        |                       | Stream outputStream)` | Serialize this        |
        |                       |                       | instance as binary to |
        |                       |                       | `outputStream`.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `unpackJarTo​(ClassLo  |                       |
        |                       | ader loader,          |                       |
        |                       |    Path destination)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `unpac                |                       |
        |                       | kNativeLibrariesInto​( |                       |
        |                       | ClassLoader loader,   |                       |
        |                       |                       |                       |
        |                       |    Path destination)` |                       |
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
    -   []{#field.detail}

        ### Field Detail

        []{#FAT_JAR_INFO_RESOURCE}

        -   #### FAT_JAR_INFO_RESOURCE

                public static final String FAT_JAR_INFO_RESOURCE

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.jvm.java.FatJar.FAT_JAR_INFO_RESOURCE)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.lang.String,java.util.Map)}

        -   #### FatJar

                public FatJar​(String innerJar,
                              Map<String,​String> nativeLibraries)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#load(java.lang.ClassLoader)}

        -   #### load

            ``` methodSignature
            public static FatJar load​(ClassLoader loader)
                               throws ClassNotFoundException,
                                      IOException
            ```

            [Returns:]{.returnLabel}
            :   the
                [`FatJar`](FatJar.html "class in com.facebook.buck.jvm.java")
                object deserialized from the resource name via `loader`.

            [Throws:]{.throwsLabel}
            :   `ClassNotFoundException`
            :   `IOException`

        []{#store(java.io.OutputStream)}

        -   #### store

            ``` methodSignature
            public void store​(OutputStream outputStream)
                       throws IOException
            ```

            ::: block
            Serialize this instance as binary to `outputStream`.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#unpackNativeLibrariesInto(java.lang.ClassLoader,java.nio.file.Path)}

        -   #### unpackNativeLibrariesInto

            ``` methodSignature
            public void unpackNativeLibrariesInto​(ClassLoader loader,
                                                  Path destination)
                                           throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#unpackJarTo(java.lang.ClassLoader,java.nio.file.Path)}

        -   #### unpackJarTo

            ``` methodSignature
            public void unpackJarTo​(ClassLoader loader,
                                    Path destination)
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

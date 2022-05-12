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
[Package]{.packageLabelInType} [com.facebook.buck.util.cache](package-summary.html)
:::

## Class JarHashCodeAndFileType {#class-jarhashcodeandfiletype .title title="Class JarHashCodeAndFileType"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.util.cache.HashCodeAndFileType](HashCodeAndFileType.html "class in com.facebook.buck.util.cache")

    -   -   com.facebook.buck.util.cache.JarHashCodeAndFileType

::: description
-   

    ------------------------------------------------------------------------

        public class JarHashCodeAndFileType
        extends HashCodeAndFileType

    ::: block
    HashCodeAndFileType that also stores and caches hashes or file in a
    jar
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.util.cache.HashCodeAndFileType}

            ### Fields inherited from class com.facebook.buck.util.cache.[HashCodeAndFileType](HashCodeAndFileType.html "class in com.facebook.buck.util.cache")

            `TYPE_ARCHIVE, TYPE_DIRECTORY, TYPE_FILE`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                                                                                                                                                    Description
          -------------- -------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `protected `   `JarHashCodeAndFileType​(byte type,                       com.google.common.hash.HashCode hashCode,                       JarContentHasher jarContentHasher)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `co                   | `getContents()`       | ::: block             |
        | m.google.common.colle |                       | Return hash values    |
        | ct.ImmutableMap<Path, |                       | for all files in an   |
        | ​HashCodeAndFileType>` |                       | archive (like a JAR)  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `ofArchive​(co         |                       |
        |  HashCodeAndFileType` | m.google.common.hash. |                       |
        |                       | HashCode hashCode,    |                       |
        |                       |        JarContentHash |                       |
        |                       | er jarContentHasher)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.util.cache.HashCodeAndFileType}

            ### Methods inherited from class com.facebook.buck.util.cache.[HashCodeAndFileType](HashCodeAndFileType.html "class in com.facebook.buck.util.cache")

            `equals, getHashCode, getType, hashCode, ofDirectory, ofFile`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(byte,com.google.common.hash.HashCode,com.facebook.buck.util.cache.JarContentHasher)}

        -   #### JarHashCodeAndFileType

                protected JarHashCodeAndFileType​(byte type,
                                                 com.google.common.hash.HashCode hashCode,
                                                 JarContentHasher jarContentHasher)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getContents()}

        -   #### getContents

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<Path,​HashCodeAndFileType> getContents()
            ```

            ::: block
            Return hash values for all files in an archive (like a JAR)
            :::

        []{#ofArchive(com.google.common.hash.HashCode,com.facebook.buck.util.cache.JarContentHasher)}

        -   #### ofArchive

            ``` methodSignature
            public static HashCodeAndFileType ofArchive​(com.google.common.hash.HashCode hashCode,
                                                        JarContentHasher jarContentHasher)
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
-   Field \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

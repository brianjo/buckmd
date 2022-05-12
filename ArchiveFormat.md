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
-   [Enum Constants](#enum.constant.summary) \| 
-   Field \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Enum Constants](#enum.constant.detail) \| 
-   Field \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.util.unarchive](package-summary.html)
:::

## Enum ArchiveFormat {#enum-archiveformat .title title="Enum ArchiveFormat"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<[ArchiveFormat](ArchiveFormat.html "enum in com.facebook.buck.util.unarchive")\>

    -   -   com.facebook.buck.util.unarchive.ArchiveFormat

::: description
-   

    All Implemented Interfaces:
    :   `Serializable`, `Comparable<ArchiveFormat>`

    ------------------------------------------------------------------------

        public enum ArchiveFormat
        extends Enum<ArchiveFormat>

    ::: block
    A collection different archive types, and the unarchiver that should
    be used to extract archives
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#enum.constant.summary}

        ### Enum Constant Summary

          Enum Constant   Description
          --------------- -------------
          `TAR`            
          `TAR_BZ2`        
          `TAR_GZ`         
          `TAR_XZ`         
          `TAR_ZSTD`       
          `ZIP`            

          : Enum Constants[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `String`              | `getExtension()`      | ::: block             |
        |                       |                       | Get the extension     |
        |                       |                       | (including \'.\') for |
        |                       |                       | this archive type     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static com.go        | `getFileExtensions()` | ::: block             |
        | ogle.common.collect.I |                       | Get all available     |
        | mmutableList<String>` |                       | file extensions       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Opt           | `getFormatFromFilen   | ::: block             |
        | ional<ArchiveFormat>` | ame​(String filename)` | Gets the archive      |
        |                       |                       | format based on a     |
        |                       |                       | file                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Opt           | `getFormatFromShortNa | ::: block             |
        | ional<ArchiveFormat>` | me​(String shortName)` | Gets the archive      |
        |                       |                       | format based on a     |
        |                       |                       | short name            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getShortName()`      | ::: block             |
        |                       |                       | Get the short name    |
        |                       |                       | for the archive type  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static com.go        | `getShortNames()`     | ::: block             |
        | ogle.common.collect.I |                       | Get all available     |
        | mmutableList<String>` |                       | short names           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Unarchiver`          | `getUnarchiver()`     | ::: block             |
        |                       |                       | Get the unarchiver    |
        |                       |                       | used to extract       |
        |                       |                       | archives of this type |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `                     | ::: block             |
        | static ArchiveFormat` | valueOf​(String name)` | Returns the enum      |
        |                       |                       | constant of this type |
        |                       |                       | with the specified    |
        |                       |                       | name.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `values()`            | ::: block             |
        | atic ArchiveFormat[]` |                       | Returns an array      |
        |                       |                       | containing the        |
        |                       |                       | constants of this     |
        |                       |                       | enum type, in the     |
        |                       |                       | order they are        |
        |                       |                       | declared.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Enum}

            ### Methods inherited from class java.lang.[Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, compareTo, equals, finalize, getDeclaringClass, hashCode, name, ordinal, valueOf`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `getClass, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#enum.constant.detail}

        ### Enum Constant Detail

        []{#TAR}

        -   #### TAR

                public static final ArchiveFormat TAR

        []{#TAR_BZ2}

        -   #### TAR_BZ2

                public static final ArchiveFormat TAR_BZ2

        []{#TAR_GZ}

        -   #### TAR_GZ

                public static final ArchiveFormat TAR_GZ

        []{#TAR_XZ}

        -   #### TAR_XZ

                public static final ArchiveFormat TAR_XZ

        []{#TAR_ZSTD}

        -   #### TAR_ZSTD

                public static final ArchiveFormat TAR_ZSTD

        []{#ZIP}

        -   #### ZIP

                public static final ArchiveFormat ZIP
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#values()}

        -   #### values

            ``` methodSignature
            public static ArchiveFormat[] values()
            ```

            ::: block
            Returns an array containing the constants of this enum type,
            in the order they are declared. This method may be used to
            iterate over the constants as follows:
                for (ArchiveFormat c : ArchiveFormat.values())
                    System.out.println(c);
            :::

            [Returns:]{.returnLabel}
            :   an array containing the constants of this enum type, in
                the order they are declared

        []{#valueOf(java.lang.String)}

        -   #### valueOf

            ``` methodSignature
            public static ArchiveFormat valueOf​(String name)
            ```

            ::: block
            Returns the enum constant of this type with the specified
            name. The string must match *exactly* an identifier used to
            declare an enum constant in this type. (Extraneous
            whitespace characters are not permitted.)
            :::

            [Parameters:]{.paramLabel}
            :   `name` - the name of the enum constant to be returned.

            [Returns:]{.returnLabel}
            :   the enum constant with the specified name

            [Throws:]{.throwsLabel}
            :   `IllegalArgumentException` - if this enum type has no
                constant with the specified name
            :   `NullPointerException` - if the argument is null

        []{#getFormatFromFilename(java.lang.String)}

        -   #### getFormatFromFilename

            ``` methodSignature
            public static Optional<ArchiveFormat> getFormatFromFilename​(String filename)
            ```

            ::: block
            Gets the archive format based on a file
            :::

            [Parameters:]{.paramLabel}
            :   `filename` - The filename to try to use

            [Returns:]{.returnLabel}
            :   The archive format, or empty if no matching format could
                be found

        []{#getFormatFromShortName(java.lang.String)}

        -   #### getFormatFromShortName

            ``` methodSignature
            public static Optional<ArchiveFormat> getFormatFromShortName​(String shortName)
            ```

            ::: block
            Gets the archive format based on a short name
            :::

            [Parameters:]{.paramLabel}
            :   `shortName` - The short name used in build files

            [Returns:]{.returnLabel}
            :   The archive format, or empty if no matching format could
                be found

        []{#getUnarchiver()}

        -   #### getUnarchiver

            ``` methodSignature
            public Unarchiver getUnarchiver()
            ```

            ::: block
            Get the unarchiver used to extract archives of this type
            :::

        []{#getExtension()}

        -   #### getExtension

            ``` methodSignature
            public String getExtension()
            ```

            ::: block
            Get the extension (including \'.\') for this archive type
            :::

        []{#getShortName()}

        -   #### getShortName

            ``` methodSignature
            public String getShortName()
            ```

            ::: block
            Get the short name for the archive type
            :::

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Enum<ArchiveFormat>`

        []{#getShortNames()}

        -   #### getShortNames

            ``` methodSignature
            public static com.google.common.collect.ImmutableList<String> getShortNames()
            ```

            ::: block
            Get all available short names
            :::

        []{#getFileExtensions()}

        -   #### getFileExtensions

            ``` methodSignature
            public static com.google.common.collect.ImmutableList<String> getFileExtensions()
            ```

            ::: block
            Get all available file extensions
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
-   [Enum Constants](#enum.constant.summary) \| 
-   Field \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Enum Constants](#enum.constant.detail) \| 
-   Field \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

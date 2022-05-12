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
[Package]{.packageLabelInType} [com.facebook.buck.util.cache](package-summary.html)
:::

## Class HashCodeAndFileType {#class-hashcodeandfiletype .title title="Class HashCodeAndFileType"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.cache.HashCodeAndFileType

::: description
-   

    Direct Known Subclasses:
    :   `JarHashCodeAndFileType`

    ------------------------------------------------------------------------

        public class HashCodeAndFileType
        extends Object

    ::: block
    Data container to hold hash value for a file or directory
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field              Description
          ------------------- ------------------ -------------
          `static byte`       `TYPE_ARCHIVE`      
          `static byte`       `TYPE_DIRECTORY`    
          `static byte`       `TYPE_FILE`         

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                                                                                     Description
          -------------- ----------------------------------------------------------------------------------------------- -------------
          `protected `   `HashCodeAndFileType​(byte type,                    com.google.common.hash.HashCode hashCode)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `boolean`             | `eq                   | ::: block             |
        |                       | uals​(Object another)` | This instance is      |
        |                       |                       | equal to all          |
        |                       |                       | instances of          |
        |                       |                       | `HashCodeAndFileType` |
        |                       |                       | that have equal       |
        |                       |                       | attribute values.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `getHashCode()`       |                       |
        | common.hash.HashCode` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `byte`                | `getType()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          | ::: block             |
        |                       |                       | Computes a hash code  |
        |                       |                       | from attributes:      |
        |                       |                       | `type`, `hashCode`.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `ofDirectory​(         |                       |
        |  HashCodeAndFileType` | com.google.common.has |                       |
        |                       | h.HashCode hashCode)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `ofFile​(              |                       |
        |  HashCodeAndFileType` | com.google.common.has |                       |
        |                       | h.HashCode hashCode)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#TYPE_DIRECTORY}

        -   #### TYPE_DIRECTORY

                public static final byte TYPE_DIRECTORY

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.cache.HashCodeAndFileType.TYPE_DIRECTORY)

        []{#TYPE_FILE}

        -   #### TYPE_FILE

                public static final byte TYPE_FILE

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.cache.HashCodeAndFileType.TYPE_FILE)

        []{#TYPE_ARCHIVE}

        -   #### TYPE_ARCHIVE

                public static final byte TYPE_ARCHIVE

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.cache.HashCodeAndFileType.TYPE_ARCHIVE)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(byte,com.google.common.hash.HashCode)}

        -   #### HashCodeAndFileType

                protected HashCodeAndFileType​(byte type,
                                              com.google.common.hash.HashCode hashCode)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getType()}

        -   #### getType

            ``` methodSignature
            public byte getType()
            ```

            [Returns:]{.returnLabel}
            :   type of the file as a constant; can be TYPE_DIRECTORY,
                TYPE_FILE or TYPE_ARCHIVE

        []{#getHashCode()}

        -   #### getHashCode

            ``` methodSignature
            public com.google.common.hash.HashCode getHashCode()
            ```

            [Returns:]{.returnLabel}
            :   Hash value of the file or directory

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(@Nullable
                                  Object another)
            ```

            ::: block
            This instance is equal to all instances of
            `HashCodeAndFileType` that have equal attribute values.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `Object`

            [Returns:]{.returnLabel}
            :   `true` if `this` is equal to `another` instance

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            ::: block
            Computes a hash code from attributes: `type`, `hashCode`.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `Object`

            [Returns:]{.returnLabel}
            :   hashCode value

        []{#ofDirectory(com.google.common.hash.HashCode)}

        -   #### ofDirectory

            ``` methodSignature
            public static HashCodeAndFileType ofDirectory​(com.google.common.hash.HashCode hashCode)
            ```

        []{#ofFile(com.google.common.hash.HashCode)}

        -   #### ofFile

            ``` methodSignature
            public static HashCodeAndFileType ofFile​(com.google.common.hash.HashCode hashCode)
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

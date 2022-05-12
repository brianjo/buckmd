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
[Package]{.packageLabelInType} [com.facebook.buck.artifact_cache](package-summary.html)
:::

## Enum CacheResultType {#enum-cacheresulttype .title title="Enum CacheResultType"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<[CacheResultType](CacheResultType.html "enum in com.facebook.buck.artifact_cache")\>

    -   -   com.facebook.buck.artifact_cache.CacheResultType

::: description
-   

    All Implemented Interfaces:
    :   `Serializable`, `Comparable<CacheResultType>`

    ------------------------------------------------------------------------

        public enum CacheResultType
        extends Enum<CacheResultType>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#enum.constant.summary}

        ### Enum Constant Summary

        +-----------------------------------+-----------------------------------+
        | Enum Constant                     | Description                       |
        +===================================+===================================+
        | `CONTAINS`                        | ::: block                         |
        |                                   | The cache contains this artifact, |
        |                                   | but was not fetched               |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `ERROR`                           | ::: block                         |
        |                                   | An error occurred when fetching   |
        |                                   | artifact from cache               |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `HIT`                             | ::: block                         |
        |                                   | Artifact was successfully fetched |
        |                                   | from cache                        |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `IGNORED`                         | ::: block                         |
        |                                   | The rule was uncachable           |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `LOCAL_KEY_UNCHANGED_HIT`         | ::: block                         |
        |                                   | Artifact cache not queried        |
        |                                   | because the local cache key was   |
        |                                   | unchanged.                        |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `MISS`                            | ::: block                         |
        |                                   | Artifact was missing from cache   |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `SKIPPED`                         | ::: block                         |
        |                                   | The cache skipped checking this   |
        |                                   | result                            |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `SOFT_ERROR`                      | ::: block                         |
        |                                   | An unexpected exception is thrown |
        |                                   | when fetching the artifact, which |
        |                                   | becomes converted to soft error.  |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+

        : Enum Constants[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `boolean`             | `isSuccess()`         | ::: block             |
        |                       |                       | Whether the artifact  |
        |                       |                       | was successfully      |
        |                       |                       | fetched.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `                     | ::: block             |
        | atic CacheResultType` | valueOf​(String name)` | Returns the enum      |
        |                       |                       | constant of this type |
        |                       |                       | with the specified    |
        |                       |                       | name.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `stat                 | `values()`            | ::: block             |
        | ic CacheResultType[]` |                       | Returns an array      |
        |                       |                       | containing the        |
        |                       |                       | constants of this     |
        |                       |                       | enum type, in the     |
        |                       |                       | order they are        |
        |                       |                       | declared.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `ve                   |                       |
        |                       | rifyValidFinalType()` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Enum}

            ### Methods inherited from class java.lang.[Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, compareTo, equals, finalize, getDeclaringClass, hashCode, name, ordinal, toString, valueOf`

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

        []{#HIT}

        -   #### HIT

                public static final CacheResultType HIT

            ::: block
            Artifact was successfully fetched from cache
            :::

        []{#MISS}

        -   #### MISS

                public static final CacheResultType MISS

            ::: block
            Artifact was missing from cache
            :::

        []{#ERROR}

        -   #### ERROR

                public static final CacheResultType ERROR

            ::: block
            An error occurred when fetching artifact from cache
            :::

        []{#IGNORED}

        -   #### IGNORED

                public static final CacheResultType IGNORED

            ::: block
            The rule was uncachable
            :::

        []{#SKIPPED}

        -   #### SKIPPED

                public static final CacheResultType SKIPPED

            ::: block
            The cache skipped checking this result
            :::

        []{#CONTAINS}

        -   #### CONTAINS

                public static final CacheResultType CONTAINS

            ::: block
            The cache contains this artifact, but was not fetched
            :::

        []{#LOCAL_KEY_UNCHANGED_HIT}

        -   #### LOCAL_KEY_UNCHANGED_HIT

                public static final CacheResultType LOCAL_KEY_UNCHANGED_HIT

            ::: block
            Artifact cache not queried because the local cache key was
            unchanged.
            :::

        []{#SOFT_ERROR}

        -   #### SOFT_ERROR

                public static final CacheResultType SOFT_ERROR

            ::: block
            An unexpected exception is thrown when fetching the
            artifact, which becomes converted to soft error.
            :::
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#values()}

        -   #### values

            ``` methodSignature
            public static CacheResultType[] values()
            ```

            ::: block
            Returns an array containing the constants of this enum type,
            in the order they are declared. This method may be used to
            iterate over the constants as follows:
                for (CacheResultType c : CacheResultType.values())
                    System.out.println(c);
            :::

            [Returns:]{.returnLabel}
            :   an array containing the constants of this enum type, in
                the order they are declared

        []{#valueOf(java.lang.String)}

        -   #### valueOf

            ``` methodSignature
            public static CacheResultType valueOf​(String name)
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

        []{#isSuccess()}

        -   #### isSuccess

            ``` methodSignature
            public boolean isSuccess()
            ```

            ::: block
            Whether the artifact was successfully fetched.
            :::

        []{#verifyValidFinalType()}

        -   #### verifyValidFinalType

            ``` methodSignature
            public void verifyValidFinalType()
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

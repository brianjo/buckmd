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
-   Field \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.util.sha1](package-summary.html)
:::

## Class Sha1HashCode {#class-sha1hashcode .title title="Class Sha1HashCode"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.sha1.Sha1HashCode

::: description
-   

    ------------------------------------------------------------------------

        public final class Sha1HashCode
        extends Object

    ::: block
    A typesafe representation of a SHA-1 hash. It is safer to pass this
    around than a `byte[]`.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.google.          | `asHashCode()`        | ::: block             |
        | common.hash.HashCode` |                       | **This method should  |
        |                       |                       | be used sparingly as  |
        |                       |                       | we are trying to      |
        |                       |                       | favor                 |
        |                       |                       | [`Sha1HashC           |
        |                       |                       | ode`](Sha1HashCode.ht |
        |                       |                       | ml "class in com.face |
        |                       |                       | book.buck.util.sha1") |
        |                       |                       | over `HashCode`,      |
        |                       |                       | where appropriate.**  |
        |                       |                       | Currently, the        |
        |                       |                       | `FileHashCache` API   |
        |                       |                       | is written in terms   |
        |                       |                       | of `HashCode`, so     |
        |                       |                       | conversions are       |
        |                       |                       | common.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `equals​(Object obj)`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Sha1HashCode` | `fro                  | ::: block             |
        |                       | mBytes​(byte[] bytes)` | Clones the specified  |
        |                       |                       | bytes and uses the    |
        |                       |                       | clone to create a new |
        |                       |                       | [`Sha1HashCo          |
        |                       |                       | de`](Sha1HashCode.htm |
        |                       |                       | l "class in com.faceb |
        |                       |                       | ook.buck.util.sha1"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Sha1HashCode` | `fromHashCode​(        |                       |
        |                       | com.google.common.has |                       |
        |                       | h.HashCode hashCode)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getHash()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Sha1HashCode` | `of​(String hash)`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          | ::: block             |
        |                       |                       | Same as               |
        |                       |                       | [`get                 |
        |                       |                       | Hash()`](#getHash()). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `upd                  | ::: block             |
        | e.common.hash.Hasher` | ate​(com.google.common | Updates the specified |
        |                       | .hash.Hasher hasher)` | `Hasher` by putting   |
        |                       |                       | the 20 bytes of this  |
        |                       |                       | SHA-1 to it in order. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#fromBytes(byte[])}

        -   #### fromBytes

            ``` methodSignature
            public static Sha1HashCode fromBytes​(byte[] bytes)
            ```

            ::: block
            Clones the specified bytes and uses the clone to create a
            new
            [`Sha1HashCode`](Sha1HashCode.html "class in com.facebook.buck.util.sha1").
            :::

        []{#fromHashCode(com.google.common.hash.HashCode)}

        -   #### fromHashCode

            ``` methodSignature
            public static Sha1HashCode fromHashCode​(com.google.common.hash.HashCode hashCode)
            ```

        []{#of(java.lang.String)}

        -   #### of

            ``` methodSignature
            public static Sha1HashCode of​(String hash)
            ```

        []{#update(com.google.common.hash.Hasher)}

        -   #### update

            ``` methodSignature
            public com.google.common.hash.Hasher update​(com.google.common.hash.Hasher hasher)
            ```

            ::: block
            Updates the specified `Hasher` by putting the 20 bytes of
            this SHA-1 to it in order.
            :::

            [Returns:]{.returnLabel}
            :   The specified `Hasher`.

        []{#asHashCode()}

        -   #### asHashCode

            ``` methodSignature
            public com.google.common.hash.HashCode asHashCode()
            ```

            ::: block
            **This method should be used sparingly as we are trying to
            favor
            [`Sha1HashCode`](Sha1HashCode.html "class in com.facebook.buck.util.sha1")
            over `HashCode`, where appropriate.** Currently, the
            `FileHashCache` API is written in terms of `HashCode`, so
            conversions are common. As we migrate it to use
            [`Sha1HashCode`](Sha1HashCode.html "class in com.facebook.buck.util.sha1"),
            this method should become unnecessary.
            :::

            [Returns:]{.returnLabel}
            :   a `HashCode` with an equivalent value

        []{#getHash()}

        -   #### getHash

            ``` methodSignature
            public String getHash()
            ```

            [Returns:]{.returnLabel}
            :   the hash as a 40-character string from the alphabet
                \[a-f0-9\].

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            ::: block
            Same as [`getHash()`](#getHash()).
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(Object obj)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `Object`

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `Object`
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
-   Field \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

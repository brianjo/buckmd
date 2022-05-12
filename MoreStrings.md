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
[Package]{.packageLabelInType} [com.facebook.buck.util.string](package-summary.html)
:::

## Class MoreStrings {#class-morestrings .title title="Class MoreStrings"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.string.MoreStrings

::: description
-   

    ------------------------------------------------------------------------

        public final class MoreStrings
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static String`       | `                     | ::: block             |
        |                       | abbreviate​(String s,  | If string width       |
        |                       |           int width)` | exceeds passed        |
        |                       |                       | parameter, replace    |
        |                       |                       | string tail with      |
        |                       |                       | dot-dot-dot.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `ca                   |                       |
        |                       | pitalize​(String str)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static int`          | `compare              | ::: block             |
        |                       | Strings​(String a,     | Compare two strings   |
        |                       |            String b)` | lexicographically.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `e                    |                       |
        |                       | ndsWithIgnoreCase​(Str |                       |
        |                       | ing str,              |                       |
        |                       |       String suffix)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static int`          | `getLeven             |                       |
        |                       | shteinDistance​(String |                       |
        |                       |  str1,                |                       |
        |                       |         String str2)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static List<String>` | `                     |                       |
        |                       | getSpellingSuggestion |                       |
        |                       | s​(String input,       |                       |
        |                       |                  Coll |                       |
        |                       | ection<String> option |                       |
        |                       | s,                    |                       |
        |                       |     int maxDistance)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `isEmpty​(Ch           |                       |
        |                       | arSequence sequence)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static com.go        | `lines​(String data)`  |                       |
        | ogle.common.collect.I |                       |                       |
        | mmutableList<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `linesToT             | ::: block             |
        |                       | ext​(String... lines)` | Joins the les passed  |
        |                       |                       | in with the platform  |
        |                       |                       | line separator.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `re                   |                       |
        |                       | gexPatternForAny​(Iter |                       |
        |                       | able<String> values)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `regexPatternForA     |                       |
        |                       | ny​(String... values)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `stripP               |                       |
        | tic Optional<String>` | refix​(String s,       |                       |
        |                       |       String prefix)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `stripS               |                       |
        | tic Optional<String>` | uffix​(String s,       |                       |
        |                       |       String suffix)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `truncateMid          |                       |
        |                       | dle​(String data,      |                       |
        |                       |           int keepFir |                       |
        |                       | stChars,              |                       |
        |                       |   int keepLastChars)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `truncat              |                       |
        |                       | eMiddle​(String data,  |                       |
        |                       |               int kee |                       |
        |                       | pFirstChars,          |                       |
        |                       |       int keepLastCha |                       |
        |                       | rs,               Str |                       |
        |                       | ing truncateMessage)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `truncat              |                       |
        |                       | ePretty​(String data)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `truncateTail​(Str     |                       |
        |                       | ing data,             |                       |
        |                       |  int keepFirstChars)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `withoutSuffi         |                       |
        |                       | x​(String str,         |                       |
        |                       |       String suffix)` |                       |
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
    -   []{#method.detail}

        ### Method Detail

        []{#linesToText(java.lang.String...)}

        -   #### linesToText

            ``` methodSignature
            public static String linesToText​(String... lines)
            ```

            ::: block
            Joins the les passed in with the platform line separator.
            :::

            [Parameters:]{.paramLabel}
            :   `lines` - the lines that need to be joined.

            [Returns:]{.returnLabel}
            :   String, containing the joined lines using the platform
                line separator as delimiter.

        []{#isEmpty(java.lang.CharSequence)}

        -   #### isEmpty

            ``` methodSignature
            public static boolean isEmpty​(CharSequence sequence)
            ```

        []{#withoutSuffix(java.lang.String,java.lang.String)}

        -   #### withoutSuffix

            ``` methodSignature
            public static String withoutSuffix​(String str,
                                               String suffix)
            ```

        []{#capitalize(java.lang.String)}

        -   #### capitalize

            ``` methodSignature
            public static String capitalize​(String str)
            ```

        []{#getLevenshteinDistance(java.lang.String,java.lang.String)}

        -   #### getLevenshteinDistance

            ``` methodSignature
            public static int getLevenshteinDistance​(String str1,
                                                     String str2)
            ```

        []{#regexPatternForAny(java.lang.String...)}

        -   #### regexPatternForAny

            ``` methodSignature
            public static String regexPatternForAny​(String... values)
            ```

        []{#regexPatternForAny(java.lang.Iterable)}

        -   #### regexPatternForAny

            ``` methodSignature
            public static String regexPatternForAny​(Iterable<String> values)
            ```

        []{#endsWithIgnoreCase(java.lang.String,java.lang.String)}

        -   #### endsWithIgnoreCase

            ``` methodSignature
            public static boolean endsWithIgnoreCase​(String str,
                                                     String suffix)
            ```

        []{#stripPrefix(java.lang.String,java.lang.String)}

        -   #### stripPrefix

            ``` methodSignature
            public static Optional<String> stripPrefix​(String s,
                                                       String prefix)
            ```

        []{#stripSuffix(java.lang.String,java.lang.String)}

        -   #### stripSuffix

            ``` methodSignature
            public static Optional<String> stripSuffix​(String s,
                                                       String suffix)
            ```

        []{#truncatePretty(java.lang.String)}

        -   #### truncatePretty

            ``` methodSignature
            public static String truncatePretty​(String data)
            ```

        []{#truncateTail(java.lang.String,int)}

        -   #### truncateTail

            ``` methodSignature
            public static String truncateTail​(String data,
                                              int keepFirstChars)
            ```

        []{#truncateMiddle(java.lang.String,int,int)}

        -   #### truncateMiddle

            ``` methodSignature
            public static String truncateMiddle​(String data,
                                                int keepFirstChars,
                                                int keepLastChars)
            ```

        []{#truncateMiddle(java.lang.String,int,int,java.lang.String)}

        -   #### truncateMiddle

            ``` methodSignature
            public static String truncateMiddle​(String data,
                                                int keepFirstChars,
                                                int keepLastChars,
                                                String truncateMessage)
            ```

        []{#lines(java.lang.String)}

        -   #### lines

            ``` methodSignature
            public static com.google.common.collect.ImmutableList<String> lines​(String data)
                                                                         throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#compareStrings(java.lang.String,java.lang.String)}

        -   #### compareStrings

            ``` methodSignature
            public static int compareStrings​(String a,
                                             String b)
            ```

            ::: block
            Compare two strings lexicographically.
            :::

        []{#getSpellingSuggestions(java.lang.String,java.util.Collection,int)}

        -   #### getSpellingSuggestions

            ``` methodSignature
            public static List<String> getSpellingSuggestions​(String input,
                                                              Collection<String> options,
                                                              int maxDistance)
            ```

            [Returns:]{.returnLabel}
            :   The spelling suggestion for the `input` based on its
                Levenstein distance from a list of available `options`.

        []{#abbreviate(java.lang.String,int)}

        -   #### abbreviate

            ``` methodSignature
            public static String abbreviate​(String s,
                                            int width)
            ```

            ::: block
            If string width exceeds passed parameter, replace string
            tail with dot-dot-dot.
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

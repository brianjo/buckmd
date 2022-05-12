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
[Package]{.packageLabelInType} [com.facebook.buck.util](package-summary.html)
:::

## Class Escaper {#class-escaper .title title="Class Escaper"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.Escaper

::: description
-   

    ------------------------------------------------------------------------

        public final class Escaper
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `Escaper.Quoter`      | ::: block             |
        |                       |                       | The quoting style to  |
        |                       |                       | use when escaping.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Field                 | Description           |
        +=======================+=======================+=======================+
        | `static j             | `ARGFILE_ESCAPER`     | ::: block             |
        | ava.util.function.Fun |                       | Escaper for argfiles  |
        | ction<String,​String>` |                       | for clang and gcc.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static j             | `BASH_ESCAPER`        | ::: block             |
        | ava.util.function.Fun |                       | Bash quoting          |
        | ction<String,​String>` |                       | `Function` which can  |
        |                       |                       | be passed to          |
        |                       |                       | `It                   |
        |                       |                       | erables.transform()`. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static j             | `CR                   | ::: block             |
        | ava.util.function.Fun | EATE_PROCESS_ESCAPER` | CreateProcess         |
        | ction<String,​String>` |                       | (Windows) quoting     |
        |                       |                       | `Function` which can  |
        |                       |                       | be passed to          |
        |                       |                       | `It                   |
        |                       |                       | erables.transform()`. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static j             | `SHELL_ESCAPER`       | ::: block             |
        | ava.util.function.Fun |                       | Platform-aware shell  |
        | ction<String,​String>` |                       | quoting `Function`    |
        |                       |                       | which can be passed   |
        |                       |                       | to                    |
        |                       |                       | `I                    |
        |                       |                       | terables.transform()` |
        |                       |                       | TODO(sdwilsh): get    |
        |                       |                       | proper cmd.EXE        |
        |                       |                       | escaping implemented  |
        |                       |                       | on Windows            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static int`          | `d                    | ::: block             |
        |                       | ecodeNumericEscape​(St | Call                  |
        |                       | ringBuilder out,      | [`decodeNumericEscap  |
        |                       |                String | e(StringBuilder, Stri |
        |                       |  escaped,             | ng, int, int, int, in |
        |                       |         int pos,      | t)`](#decodeNumericEs |
        |                       |                int ma | cape(java.lang.String |
        |                       | xCodeLength,          | Builder,java.lang.Str |
        |                       |            int base)` | ing,int,int,int,int)) |
        |                       |                       | to parse at most one  |
        |                       |                       | escaped character;    |
        |                       |                       | i.e.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static int`          | `decodeNumeric        | ::: block             |
        |                       | Escape​(StringBuilder  | Decode a numeric      |
        |                       | out,                  | escape as explained   |
        |                       |    String escaped,    | in this page:         |
        |                       |                  int  | <http://              |
        |                       | pos,                  | en.cppreference.com/w |
        |                       |    int maxCodeLength, | /cpp/language/escape> |
        |                       |                     i | .                     |
        |                       | nt base,              | :::                   |
        |                       |        int maxCodes)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `escape​(Escaper       | ::: block             |
        |                       | .Quoter quoter,       | Escapes the special   |
        |                       |  com.google.common.ba | characters identified |
        |                       | se.CharMatcher matche | the `CharMatcher`,    |
        |                       | r,       String str)` | using single quotes.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `escapeAsBa           | ::: block             |
        |                       | shString​(String str)` | Quotes a string to be |
        |                       |                       | passed to Bash, if    |
        |                       |                       | necessary.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `escapeAsB            |                       |
        |                       | ashString​(Path path)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `escapeAsMakefileVal  |                       |
        |                       | ueString​(String str)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `escapeAsPyth         |                       |
        |                       | onString​(String str)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `escapeAsShe          | ::: block             |
        |                       | llString​(String str)` | Quotes a string to be |
        |                       |                       | passed to the shell,  |
        |                       |                       | if necessary.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `escapePathForCIncl   | ::: block             |
        |                       | udeString​(Path path)` | Escapes forward       |
        |                       |                       | slashes in a Path as  |
        |                       |                       | a String that is safe |
        |                       |                       | to consume with other |
        |                       |                       | tools (such as gcc).  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static j             | `escaper​(Escaper.Quo  |                       |
        | ava.util.function.Fun | ter quoter,        co |                       |
        | ction<String,​String>` | m.google.common.base. |                       |
        |                       | CharMatcher matcher)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `escapeWi             |                       |
        |                       | thQuotesAsMakefileVal |                       |
        |                       | ueString​(String str)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static j             | `javacEscaper()`      |                       |
        | ava.util.function.Fun |                       |                       |
        | ction<String,​String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `unescapeLineMarker   | ::: block             |
        |                       | Path​(String escaped)` | Unescape a path       |
        |                       |                       | string obtained from  |
        |                       |                       | preprocessor output,  |
        |                       |                       | as in:                |
        |                       |                       | <https://gcc.gnu.or   |
        |                       |                       | g/onlinedocs/cpp/Prep |
        |                       |                       | rocessor-Output.html> |
        |                       |                       | .                     |
        |                       |                       | :::                   |
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

        []{#BASH_ESCAPER}

        -   #### BASH_ESCAPER

                public static final java.util.function.Function<String,​String> BASH_ESCAPER

            ::: block
            Bash quoting `Function` which can be passed to
            `Iterables.transform()`.
            :::

        []{#CREATE_PROCESS_ESCAPER}

        -   #### CREATE_PROCESS_ESCAPER

                public static final java.util.function.Function<String,​String> CREATE_PROCESS_ESCAPER

            ::: block
            CreateProcess (Windows) quoting `Function` which can be
            passed to `Iterables.transform()`.
            :::

        []{#SHELL_ESCAPER}

        -   #### SHELL_ESCAPER

                public static final java.util.function.Function<String,​String> SHELL_ESCAPER

            ::: block
            Platform-aware shell quoting `Function` which can be passed
            to `Iterables.transform()` TODO(sdwilsh): get proper cmd.EXE
            escaping implemented on Windows
            :::

        []{#ARGFILE_ESCAPER}

        -   #### ARGFILE_ESCAPER

                public static final java.util.function.Function<String,​String> ARGFILE_ESCAPER

            ::: block
            Escaper for argfiles for clang and gcc.
            Based on the following docs in the gcc manual:

            \@file Read command-line options from file. The options read
            are inserted in place of the original \@file option. If file
            does not exist, or cannot be read, then the option will be
            treated literally, and not removed.

            Options in file are separated by whitespace. A whitespace
            character may be included in an option by surrounding the
            entire option in either single or double quotes. Any
            character (including a backslash) may be included by
            prefixing the character to be included with a backslash. The
            file may itself contain additional \@file options; any such
            options will be processed recursively.
            :::
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#escape(com.facebook.buck.util.Escaper.Quoter,com.google.common.base.CharMatcher,java.lang.String)}

        -   #### escape

            ``` methodSignature
            public static String escape​(Escaper.Quoter quoter,
                                        com.google.common.base.CharMatcher matcher,
                                        String str)
            ```

            ::: block
            Escapes the special characters identified the `CharMatcher`,
            using single quotes.
            :::

            [Parameters:]{.paramLabel}
            :   `matcher` - identifies characters to be escaped
            :   `str` - string to quote

            [Returns:]{.returnLabel}
            :   possibly quoted string

        []{#escaper(com.facebook.buck.util.Escaper.Quoter,com.google.common.base.CharMatcher)}

        -   #### escaper

            ``` methodSignature
            public static java.util.function.Function<String,​String> escaper​(Escaper.Quoter quoter,
                                                                                   com.google.common.base.CharMatcher matcher)
            ```

            [Returns:]{.returnLabel}
            :   a escaper function using the given quote style and
                escaping characters determined by the given matcher.

        []{#javacEscaper()}

        -   #### javacEscaper

            ``` methodSignature
            public static java.util.function.Function<String,​String> javacEscaper()
            ```

        []{#escapeAsShellString(java.lang.String)}

        -   #### escapeAsShellString

            ``` methodSignature
            public static String escapeAsShellString​(String str)
            ```

            ::: block
            Quotes a string to be passed to the shell, if necessary.
            This works for the appropriate shell regardless of the
            platform it is run on.
            :::

            [Parameters:]{.paramLabel}
            :   `str` - string to escape

            [Returns:]{.returnLabel}
            :   possibly escaped string

        []{#escapeAsBashString(java.lang.String)}

        -   #### escapeAsBashString

            ``` methodSignature
            public static String escapeAsBashString​(String str)
            ```

            ::: block
            Quotes a string to be passed to Bash, if necessary. Uses
            single quotes to prevent variable expansion, \`\...\`
            evaluation etc.
            :::

            [Parameters:]{.paramLabel}
            :   `str` - string to quote

            [Returns:]{.returnLabel}
            :   possibly quoted string

        []{#escapeAsBashString(java.nio.file.Path)}

        -   #### escapeAsBashString

            ``` methodSignature
            public static String escapeAsBashString​(Path path)
            ```

        []{#escapeAsPythonString(java.lang.String)}

        -   #### escapeAsPythonString

            ``` methodSignature
            public static String escapeAsPythonString​(String str)
            ```

            [Returns:]{.returnLabel}
            :   a double-quoted string with metacharacters and quotes
                escaped with a backslash; non-ASCII characters escaped
                as \\u

        []{#escapeAsMakefileValueString(java.lang.String)}

        -   #### escapeAsMakefileValueString

            ``` methodSignature
            public static String escapeAsMakefileValueString​(String str)
            ```

            [Returns:]{.returnLabel}
            :   an escaped string suitable for use in a GNU makefile on
                the right side of a variable assignment.

        []{#escapeWithQuotesAsMakefileValueString(java.lang.String)}

        -   #### escapeWithQuotesAsMakefileValueString

            ``` methodSignature
            public static String escapeWithQuotesAsMakefileValueString​(String str)
            ```

            [Returns:]{.returnLabel}
            :   quoted string if it contains at least one character that
                needs to be escaped

        []{#escapePathForCIncludeString(java.nio.file.Path)}

        -   #### escapePathForCIncludeString

            ``` methodSignature
            public static String escapePathForCIncludeString​(Path path)
            ```

            ::: block
            Escapes forward slashes in a Path as a String that is safe
            to consume with other tools (such as gcc). On Unix systems,
            this is equivalent to
            [`Path.toString()`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}.
            :::

            [Parameters:]{.paramLabel}
            :   `path` - the Path to escape

            [Returns:]{.returnLabel}
            :   the escaped Path

        []{#unescapeLineMarkerPath(java.lang.String)}

        -   #### unescapeLineMarkerPath

            ``` methodSignature
            public static String unescapeLineMarkerPath​(String escaped)
            ```

            ::: block
            Unescape a path string obtained from preprocessor output, as
            in:
            <https://gcc.gnu.org/onlinedocs/cpp/Preprocessor-Output.html>
            .
            :::

            [See Also:]{.seeLabel}
            :   [`decodeNumericEscape(StringBuilder, String, int, int, int, int)`](#decodeNumericEscape(java.lang.StringBuilder,java.lang.String,int,int,int,int))

        []{#decodeNumericEscape(java.lang.StringBuilder,java.lang.String,int,int,int,int)}

        -   #### decodeNumericEscape

            ``` methodSignature
            public static int decodeNumericEscape​(StringBuilder out,
                                                  String escaped,
                                                  int pos,
                                                  int maxCodeLength,
                                                  int base,
                                                  int maxCodes)
            ```

            ::: block
            Decode a numeric escape as explained in this page:
            <http://en.cppreference.com/w/cpp/language/escape> . The
            pointed-to substring shouldn\'t contain the leading
            backslash + optional \'x\' or \'u\'.
            :::

            [Parameters:]{.paramLabel}
            :   `out` - receives decoded characters
            :   `escaped` - the string containing the escape sequence
            :   `pos` - starting index of escape (but after the
                backslash)
            :   `base` - number base, e.g. 8 for octal, or 16 for hex or
                unicode.
            :   `maxCodes` - maximum number of sequences of escape
                numbers to decode. This is mainly to support unicode
                escape sequences which might represent one or two
                characters.

            [Returns:]{.returnLabel}
            :   position to first character just after the consumed
                numeric code. Is number of consumed code bytes + `pos`
                argument.

        []{#decodeNumericEscape(java.lang.StringBuilder,java.lang.String,int,int,int)}

        -   #### decodeNumericEscape

            ``` methodSignature
            public static int decodeNumericEscape​(StringBuilder out,
                                                  String escaped,
                                                  int pos,
                                                  int maxCodeLength,
                                                  int base)
            ```

            ::: block
            Call
            [`decodeNumericEscape(StringBuilder, String, int, int, int, int)`](#decodeNumericEscape(java.lang.StringBuilder,java.lang.String,int,int,int,int))
            to parse at most one escaped character; i.e. calls that
            method with `maxCodes = 1`.
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

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
[Package]{.packageLabelInType} [com.facebook.buck.util](package-summary.html)
:::

## Class Ansi {#class-ansi .title title="Class Ansi"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.Ansi

::: description
-   

    ------------------------------------------------------------------------

        public final class Ansi
        extends Object

    ::: block
    Encapsulates the specifics of writing to a particular kind of
    terminal.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                  Description
          ------------------- ---------------------- -------------
          `static class `     `Ansi.SeverityLevel`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `Ansi​(boolean isAnsiTerminal)`    | ::: block                         |
        |                                   | Construct an Ansi object and      |
        |                                   | conditionally enable fancy escape |
        |                                   | sequences.                        |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+

        : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `String`              | `asEr                 |                       |
        |                       | rorText​(String text)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `asGr                 |                       |
        |                       | eenText​(String text)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `asHighlightedFail    |                       |
        |                       | ureText​(String text)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `as                   |                       |
        |                       | HighlightedStatusText |                       |
        |                       | ​(Ansi.SeverityLevel l |                       |
        |                       | evel,                 |                       |
        |                       |         String text)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `asHighlightedSucc    |                       |
        |                       | essText​(String text)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `asHighlightedWarn    |                       |
        |                       | ingText​(String text)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `asInformat           |                       |
        |                       | ionText​(String text)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable<String>`    | `asNoWrap​(Iterabl     |                       |
        |                       | e<String> textParts)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `as                   |                       |
        |                       | RedText​(String text)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `asSub                |                       |
        |                       | tleText​(String text)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `asSucc               |                       |
        |                       | essText​(String text)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `asWarn               |                       |
        |                       | ingText​(String text)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `clearLine()`         | ::: block             |
        |                       |                       | Clears the line the   |
        |                       |                       | cursor is currently   |
        |                       |                       | on.                   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `c                    | ::: block             |
        |                       | learToTheEndOfLine()` | Clears from the       |
        |                       |                       | cursor to the end of  |
        |                       |                       | line.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `curso                | ::: block             |
        |                       | rPreviousLine​(int y)` | Moves the cursor `y`  |
        |                       |                       | lines up.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Ansi`         | `forceTty()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getHighli            |                       |
        |                       | ghtedResetSequence()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getHighligh          |                       |
        |                       | tedWarningSequence()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isAnsiTerminal()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `prin                 |                       |
        |                       | tHighlightedSuccessTe |                       |
        |                       | xt​(PrintStream stream |                       |
        |                       | ,                     |                       |
        |                       |         String text)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `printlnH             |                       |
        |                       | ighlightedFailureText |                       |
        |                       | ​(PrintStream stream,  |                       |
        |                       |                       |                       |
        |                       |         String text)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Ansi`         | `withoutTty()`        |                       |
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(boolean)}

        -   #### Ansi

                public Ansi​(boolean isAnsiTerminal)

            ::: block
            Construct an Ansi object and conditionally enable fancy
            escape sequences.
            :::
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#withoutTty()}

        -   #### withoutTty

            ``` methodSignature
            public static Ansi withoutTty()
            ```

        []{#forceTty()}

        -   #### forceTty

            ``` methodSignature
            public static Ansi forceTty()
            ```

        []{#isAnsiTerminal()}

        -   #### isAnsiTerminal

            ``` methodSignature
            public boolean isAnsiTerminal()
            ```

        []{#asErrorText(java.lang.String)}

        -   #### asErrorText

            ``` methodSignature
            public String asErrorText​(String text)
            ```

        []{#asWarningText(java.lang.String)}

        -   #### asWarningText

            ``` methodSignature
            public String asWarningText​(String text)
            ```

        []{#asSuccessText(java.lang.String)}

        -   #### asSuccessText

            ``` methodSignature
            public String asSuccessText​(String text)
            ```

        []{#asSubtleText(java.lang.String)}

        -   #### asSubtleText

            ``` methodSignature
            public String asSubtleText​(String text)
            ```

        []{#asInformationText(java.lang.String)}

        -   #### asInformationText

            ``` methodSignature
            public String asInformationText​(String text)
            ```

        []{#asGreenText(java.lang.String)}

        -   #### asGreenText

            ``` methodSignature
            public String asGreenText​(String text)
            ```

        []{#asRedText(java.lang.String)}

        -   #### asRedText

            ``` methodSignature
            public String asRedText​(String text)
            ```

        []{#getHighlightedWarningSequence()}

        -   #### getHighlightedWarningSequence

            ``` methodSignature
            public String getHighlightedWarningSequence()
            ```

        []{#getHighlightedResetSequence()}

        -   #### getHighlightedResetSequence

            ``` methodSignature
            public String getHighlightedResetSequence()
            ```

        []{#asHighlightedFailureText(java.lang.String)}

        -   #### asHighlightedFailureText

            ``` methodSignature
            public String asHighlightedFailureText​(String text)
            ```

        []{#asHighlightedWarningText(java.lang.String)}

        -   #### asHighlightedWarningText

            ``` methodSignature
            public String asHighlightedWarningText​(String text)
            ```

        []{#asHighlightedSuccessText(java.lang.String)}

        -   #### asHighlightedSuccessText

            ``` methodSignature
            public String asHighlightedSuccessText​(String text)
            ```

        []{#asNoWrap(java.lang.Iterable)}

        -   #### asNoWrap

            ``` methodSignature
            public Iterable<String> asNoWrap​(Iterable<String> textParts)
            ```

        []{#printHighlightedSuccessText(java.io.PrintStream,java.lang.String)}

        -   #### printHighlightedSuccessText

            ``` methodSignature
            public void printHighlightedSuccessText​(PrintStream stream,
                                                    String text)
            ```

        []{#printlnHighlightedFailureText(java.io.PrintStream,java.lang.String)}

        -   #### printlnHighlightedFailureText

            ``` methodSignature
            public void printlnHighlightedFailureText​(PrintStream stream,
                                                      String text)
            ```

        []{#asHighlightedStatusText(com.facebook.buck.util.Ansi.SeverityLevel,java.lang.String)}

        -   #### asHighlightedStatusText

            ``` methodSignature
            public String asHighlightedStatusText​(Ansi.SeverityLevel level,
                                                  String text)
            ```

        []{#cursorPreviousLine(int)}

        -   #### cursorPreviousLine

            ``` methodSignature
            public String cursorPreviousLine​(int y)
            ```

            ::: block
            Moves the cursor `y` lines up.
            :::

        []{#clearLine()}

        -   #### clearLine

            ``` methodSignature
            public String clearLine()
            ```

            ::: block
            Clears the line the cursor is currently on.
            :::

        []{#clearToTheEndOfLine()}

        -   #### clearToTheEndOfLine

            ``` methodSignature
            public String clearToTheEndOfLine()
            ```

            ::: block
            Clears from the cursor to the end of line.
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

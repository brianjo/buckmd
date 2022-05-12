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
[Package]{.packageLabelInType} [com.facebook.buck.core.macros](package-summary.html)
:::

## Class MacroFinderAutomaton {#class-macrofinderautomaton .title title="Class MacroFinderAutomaton"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.google.common.collect.UnmodifiableIterator\<[MacroMatchResult](MacroMatchResult.html "interface in com.facebook.buck.core.macros")\>

    -   -   com.facebook.buck.core.macros.MacroFinderAutomaton

::: description
-   

    All Implemented Interfaces:
    :   `Iterator<MacroMatchResult>`

    ------------------------------------------------------------------------

        public class MacroFinderAutomaton
        extends com.google.common.collect.UnmodifiableIterator<MacroMatchResult>

    ::: block
    A push-down automaton that searches for occurrences of a macro in
    linear time with respect to the search string. The automaton keeps
    track of 5 pieces of state: 1) The current automaton state 2) The
    position in the input string 3) The current nested depth of
    parentheses 4) The type of quote (if any) which bounds the current
    sequence 5) The return state to go back to after an escape sequence
    ends
    The automaton accumulates intermediate values in the string builder
    and the match result builder. The `find()` method will advance the
    automaton along the input string until it finds a macro, and returns
    a match, or until it reaches the end of the string and returns null.

    Examples of valid matching patterns: \$(macro) \$(macro argument)
    \$(macro nested parens(argument)) \$(macro \'ignored paren )\')

    If the macro is preceeded by a \'\\\' the match result will be
    marked as escaped, and the capture group will include the escaping
    backslash. Example: \\\$(macro)

    Here are the state transitions in dot format (with glossing over of
    saved state):

           digraph G {
             "SEARCHING" -> "FOUND_DOLLAR"  [label="'$'"];
             "FOUND_DOLLAR" -> "SEARCHING"  [label="*"];
             "FOUND_DOLLAR" -> "READING_MACRO_NAME"  [label="'('"];
             "READING_MACRO_NAME" -> "FOUND_MACRO"  [label="')'"];
             "READING_MACRO_NAME" -> "READING_ARGS"  [label="\\s"];
             "READING_MACRO_NAME" -> "READING_MACRO_NAME"  [label="\\w"];
             "READING_ARGS" -> "FOUND_MACRO"  [label="Balanced ')'"];
             "READING_ARGS" -> "READING_QUOTED_ARGS"  [label="'|\""];
             "READING_QUOTED_ARGS" -> "READING_ARGS"  [label="Matching '|\""];
             "READING_QUOTED_ARGS" -> "READING_QUOTED_ARGS"  [label="[^'\"]"];
             "READING_ARGS" -> "READING_ARGS"  [label="[^'\")]"];
             "SEARCHING" -> "IN_ESCAPE_SEQUENCE"  [label="\\"];
             "IN_ESCAPE_SEQUENCE" -> "FOUND_DOLLAR"  [label="$"];
             "READING_ARGS" -> "IN_ESCAPE_ARG_SEQUENCE"  [label="\\"];
             "READING_QUOTED_ARGS" -> "IN_ESCAPE_ARG_SEQUENCE"  [label="\\"];
           }
         

    Not shown: transitions back from \"IN_ESCAPE_SEQUENCE\" and
    \"IN_ESCAPE_ARG_SEQUENCE\", as they return to the previous state
    The EBNF grammar for a macro definition is as follows:

           macro = "$(", macro_name, whitespace, [arg_list], ")";
           macro_name = {all_ascii_chars - whitespace - parens};
           whitespace = "\t" | "\n" | " " | "\r";
           parens = "(" | ")";
           arg_list = arg | arg, whitespace, arg_list;
           arg = {all_ascii_chars - whitespace - parens}
                 | "(", arg, ")"
                 | "\"", [{-"\""}], "\""
                 | "'", [{-"'"}], "'";

         

    This documentation and grammar are published in the
    string_parameters_macro.soy documentation.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                           Description
          ------------------------------------- -------------
          `MacroFinderAutomaton​(String blob)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type    Method        Description
          -------------------- ------------- -------------
          `boolean`            `hasNext()`    
          `MacroMatchResult`   `next()`       

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.google.common.collect.UnmodifiableIterator}

            ### Methods inherited from class com.google.common.collect.UnmodifiableIterator

            `remove`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.util.Iterator}

            ### Methods inherited from interface java.util.[Iterator](http://docs.oracle.com/javase/7/docs/api/java/util/Iterator.html?is-external=true "class or interface in java.util"){.externalLink}

            `forEachRemaining`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.lang.String)}

        -   #### MacroFinderAutomaton

                public MacroFinderAutomaton​(String blob)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#hasNext()}

        -   #### hasNext

            ``` methodSignature
            public boolean hasNext()
            ```

        []{#next()}

        -   #### next

            ``` methodSignature
            public MacroMatchResult next()
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

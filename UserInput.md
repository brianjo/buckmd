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
[Package]{.packageLabelInType} [com.facebook.buck.doctor](package-summary.html)
:::

## Class UserInput {#class-userinput .title title="Class UserInput"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.doctor.UserInput

::: description
-   

    ------------------------------------------------------------------------

        public class UserInput
        extends Object

    ::: block
    Helper methods for handling input from the user.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                            Description
          ---------------------------------------------------------------------- -------------
          `UserInput​(PrintStream output,          BufferedReader inputReader)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                          Method                                                                                                                      Description
          ---------------------------------------------------------- --------------------------------------------------------------------------------------------------------------------------- -------------
          `String`                                                   `ask​(String question)`                                                                                                       
          `boolean`                                                  `confirm​(String question)`                                                                                                   
          `static Integer`                                           `parseOne​(String input)`                                                                                                     
          `static com.google.common.collect.ImmutableSet<Integer>`   `parseRange​(String input)`                                                                                                   
          `<T> Optional<T>`                                          `selectOne​(String prompt,          List<T> entries,          java.util.function.Function<T,​String> entryFormatter)`          
          `<T> com.google.common.collect.ImmutableSet<T>`            `selectRange​(String prompt,            List<T> entries,            java.util.function.Function<T,​String> entryFormatter)`    

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

        []{#<init>(java.io.PrintStream,java.io.BufferedReader)}

        -   #### UserInput

                public UserInput​(PrintStream output,
                                 BufferedReader inputReader)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#ask(java.lang.String)}

        -   #### ask

            ``` methodSignature
            public String ask​(String question)
                       throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#confirm(java.lang.String)}

        -   #### confirm

            ``` methodSignature
            public boolean confirm​(String question)
                            throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#parseOne(java.lang.String)}

        -   #### parseOne

            ``` methodSignature
            public static Integer parseOne​(String input)
            ```

        []{#parseRange(java.lang.String)}

        -   #### parseRange

            ``` methodSignature
            public static com.google.common.collect.ImmutableSet<Integer> parseRange​(String input)
            ```

        []{#selectOne(java.lang.String,java.util.List,java.util.function.Function)}

        -   #### selectOne

            ``` methodSignature
            public <T> Optional<T> selectOne​(String prompt,
                                             List<T> entries,
                                             java.util.function.Function<T,​String> entryFormatter)
                                      throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#selectRange(java.lang.String,java.util.List,java.util.function.Function)}

        -   #### selectRange

            ``` methodSignature
            public <T> com.google.common.collect.ImmutableSet<T> selectRange​(String prompt,
                                                                             List<T> entries,
                                                                             java.util.function.Function<T,​String> entryFormatter)
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

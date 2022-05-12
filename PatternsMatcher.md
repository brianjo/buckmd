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
[Package]{.packageLabelInType} [com.facebook.buck.util](package-summary.html)
:::

## Class PatternsMatcher {#class-patternsmatcher .title title="Class PatternsMatcher"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.PatternsMatcher

::: description
-   

    ------------------------------------------------------------------------

        public class PatternsMatcher
        extends Object

    ::: block
    Helper class that keeps a list of compiled patterns and provides a
    method to check whether a string matches at least one of them.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Field                 | Description           |
        +=======================+=======================+=======================+
        | `st                   | `ANY`                 | ::: block             |
        | atic PatternsMatcher` |                       | A pattern which       |
        |                       |                       | patches any string    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `NONE`                | ::: block             |
        | atic PatternsMatcher` |                       | A pattern which       |
        |                       |                       | matches no string     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                           Description
          ------------------------------------------------------------------------------------- -------------
          `PatternsMatcher​(com.google.common.collect.ImmutableSet<Pattern> compiledPatterns)`    
          `PatternsMatcher​(Collection<String> rawPatterns)`                                      

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type     Method                                           Description
          --------------------- ------------------------------------------------ -------------
          `<V> Map<String,​V>`   `filterMatchingMapKeys​(Map<String,​V> entries)`    
          `boolean`             `isMatchesAny()`                                  
          `boolean`             `isMatchesNone()`                                 
          `boolean`             `matches​(String string)`                          
          `boolean`             `substringMatches​(String string)`                 

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
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
    -   []{#field.detail}

        ### Field Detail

        []{#ANY}

        -   #### ANY

                public static final PatternsMatcher ANY

            ::: block
            A pattern which patches any string
            :::

        []{#NONE}

        -   #### NONE

                public static final PatternsMatcher NONE

            ::: block
            A pattern which matches no string
            :::
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.util.Collection)}

        -   #### PatternsMatcher

                public PatternsMatcher​(Collection<String> rawPatterns)

        []{#<init>(com.google.common.collect.ImmutableSet)}

        -   #### PatternsMatcher

                public PatternsMatcher​(com.google.common.collect.ImmutableSet<Pattern> compiledPatterns)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#matches(java.lang.String)}

        -   #### matches

            ``` methodSignature
            public boolean matches​(String string)
            ```

            [Returns:]{.returnLabel}
            :   true if the given string matches some of the patterns

        []{#substringMatches(java.lang.String)}

        -   #### substringMatches

            ``` methodSignature
            public boolean substringMatches​(String string)
            ```

            [Returns:]{.returnLabel}
            :   true if a substring of the given string matches some of
                the patterns or there are no patterns

        []{#isMatchesAny()}

        -   #### isMatchesAny

            ``` methodSignature
            public boolean isMatchesAny()
            ```

            [Returns:]{.returnLabel}
            :   true if this pattern matches any string

        []{#isMatchesNone()}

        -   #### isMatchesNone

            ``` methodSignature
            public boolean isMatchesNone()
            ```

            [Returns:]{.returnLabel}
            :   true if no string matches this pattern

        []{#filterMatchingMapKeys(java.util.Map)}

        -   #### filterMatchingMapKeys

            ``` methodSignature
            public <V> Map<String,​V> filterMatchingMapKeys​(Map<String,​V> entries)
            ```

            [Returns:]{.returnLabel}
            :   a view of the given map where all non-matching keys are
                removed.
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

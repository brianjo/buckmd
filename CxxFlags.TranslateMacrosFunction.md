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
[Package]{.packageLabelInType} [com.facebook.buck.cxx](package-summary.html)
:::

## Class CxxFlags.TranslateMacrosFunction {#class-cxxflags.translatemacrosfunction .title title="Class CxxFlags.TranslateMacrosFunction"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.CxxFlags.TranslateMacrosFunction

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`, `AddsToRuleKeyFunction<String,​String>`,
        `java.util.function.Function<String,​String>`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [CxxFlags](CxxFlags.html "class in com.facebook.buck.cxx")

    ------------------------------------------------------------------------

        public static class CxxFlags.TranslateMacrosFunction
        extends Object
        implements AddsToRuleKeyFunction<String,​String>

    ::: block
    Function for translating cxx flag macros.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                         Description
          --------------------------------------------------------------------------------------------------- -------------
          `TranslateMacrosFunction​(com.google.common.collect.ImmutableSortedMap<String,​String> flagMacros)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                 Description
          ------------------- ---------------------- -------------
          `String`            `apply​(String flag)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.util.function.Function}

            ### Methods inherited from interface java.util.function.Function

            `andThen, compose`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.google.common.collect.ImmutableSortedMap)}

        -   #### TranslateMacrosFunction

                public TranslateMacrosFunction​(com.google.common.collect.ImmutableSortedMap<String,​String> flagMacros)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#apply(java.lang.String)}

        -   #### apply

            ``` methodSignature
            public String apply​(String flag)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `apply` in
                interface `java.util.function.Function<String,​String>`
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
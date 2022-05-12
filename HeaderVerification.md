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
[Package]{.packageLabelInType} [com.facebook.buck.cxx.toolchain](package-summary.html)
:::

## Class HeaderVerification {#class-headerverification .title title="Class HeaderVerification"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.toolchain.HeaderVerification

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`

    ------------------------------------------------------------------------

        public abstract class HeaderVerification
        extends Object
        implements AddsToRuleKey

    ::: block
    Defines how to handle headers that get included during the build but
    aren\'t explicitly tracked in any build files.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                       Description
          ------------------- --------------------------- -------------
          `static class `     `HeaderVerification.Mode`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor              Description
          ------------------------ -------------
          `HeaderVerification()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                    Method                                                                                                                                                                           Description
          -------------------------------------------------------------------- -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `abstract HeaderVerification.Mode`                                   `getMode()`                                                                                                                                                                       
          `abstract com.google.common.collect.ImmutableSortedSet<String>`      `getPlatformWhitelist()`                                                                                                                                                          
          `abstract com.google.common.collect.ImmutableSortedSet<String>`      `getWhitelist()`                                                                                                                                                                  
          `protected com.google.common.collect.ImmutableList<FasterPattern>`   `getWhitelistPatterns()`                                                                                                                                                          
          `boolean`                                                            `isWhitelisted​(String header)`                                                                                                                                                    
          `static HeaderVerification`                                          `of​(HeaderVerification.Mode mode)`                                                                                                                                                
          `static HeaderVerification`                                          `of​(HeaderVerification.Mode mode,   com.google.common.collect.ImmutableSortedSet<String> whitelist,   com.google.common.collect.ImmutableSortedSet<String> platformWhitelist)`    
          `HeaderVerification`                                                 `withPlatformWhitelist​(Iterable<String> elements)`                                                                                                                                

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
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

        []{#<init>()}

        -   #### HeaderVerification

                public HeaderVerification()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getMode()}

        -   #### getMode

            ``` methodSignature
            public abstract HeaderVerification.Mode getMode()
            ```

        []{#getWhitelist()}

        -   #### getWhitelist

            ``` methodSignature
            @NaturalOrder
            public abstract com.google.common.collect.ImmutableSortedSet<String> getWhitelist()
            ```

            [Returns:]{.returnLabel}
            :   a list of regexes which match headers which should be
                exempt from verification.

        []{#getPlatformWhitelist()}

        -   #### getPlatformWhitelist

            ``` methodSignature
            @NaturalOrder
            public abstract com.google.common.collect.ImmutableSortedSet<String> getPlatformWhitelist()
            ```

            [Returns:]{.returnLabel}
            :   a list of regexes which match headers from the platform
                SDK. The path for the platforms might depend on the disk
                layout. Therefore, we don\'t want that one to be
                included in the rule keys.

        []{#getWhitelistPatterns()}

        -   #### getWhitelistPatterns

            ``` methodSignature
            @Derived
            protected com.google.common.collect.ImmutableList<FasterPattern> getWhitelistPatterns()
            ```

        []{#of(com.facebook.buck.cxx.toolchain.HeaderVerification.Mode)}

        -   #### of

            ``` methodSignature
            public static HeaderVerification of​(HeaderVerification.Mode mode)
            ```

        []{#of(com.facebook.buck.cxx.toolchain.HeaderVerification.Mode,com.google.common.collect.ImmutableSortedSet,com.google.common.collect.ImmutableSortedSet)}

        -   #### of

            ``` methodSignature
            public static HeaderVerification of​(HeaderVerification.Mode mode,
                                                com.google.common.collect.ImmutableSortedSet<String> whitelist,
                                                com.google.common.collect.ImmutableSortedSet<String> platformWhitelist)
            ```

        []{#isWhitelisted(java.lang.String)}

        -   #### isWhitelisted

            ``` methodSignature
            public boolean isWhitelisted​(String header)
            ```

            [Returns:]{.returnLabel}
            :   whether the given header has been whitelisted.

        []{#withPlatformWhitelist(java.lang.Iterable)}

        -   #### withPlatformWhitelist

            ``` methodSignature
            public HeaderVerification withPlatformWhitelist​(Iterable<String> elements)
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

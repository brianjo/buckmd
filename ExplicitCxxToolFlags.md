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
[Package]{.packageLabelInType} [com.facebook.buck.cxx](package-summary.html)
:::

## Class ExplicitCxxToolFlags {#class-explicitcxxtoolflags .title title="Class ExplicitCxxToolFlags"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.cxx.CxxToolFlags](CxxToolFlags.html "class in com.facebook.buck.cxx")

    -   -   com.facebook.buck.cxx.ExplicitCxxToolFlags

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`

    ------------------------------------------------------------------------

        public abstract class ExplicitCxxToolFlags
        extends CxxToolFlags

    ::: block
    `CxxToolFlags` implementation where the flags are stored explicitly
    as lists.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                            Description
          ------------------- -------------------------------- -------------
          `static class `     `ExplicitCxxToolFlags.Builder`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                Description
          -------------------------- -------------
          `ExplicitCxxToolFlags()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static void`         | `addCx                |                       |
        |                       | xToolFlags​(ExplicitCx |                       |
        |                       | xToolFlags.Builder bu |                       |
        |                       | ilder,                |                       |
        |                       |  CxxToolFlags flags)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract com         | `getPlatformFlags()`  | ::: block             |
        | .google.common.collec |                       | Flags that precede    |
        | t.ImmutableList<Arg>` |                       | flags from            |
        |                       |                       | `#getRuleFlags()`.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract com         | `getRuleFlags()`      | ::: block             |
        | .google.common.collec |                       | Flags that succeed    |
        | t.ImmutableList<Arg>` |                       | flags from            |
        |                       |                       | `                     |
        |                       |                       | #getPlatformFlags()`. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.cxx.CxxToolFlags}

            ### Methods inherited from class com.facebook.buck.cxx.[CxxToolFlags](CxxToolFlags.html "class in com.facebook.buck.cxx")

            `concat, copyOf, explicitBuilder, getAllFlags, of`

        ```{=html}
        <!-- -->
        ```
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

        -   #### ExplicitCxxToolFlags

                public ExplicitCxxToolFlags()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getPlatformFlags()}

        -   #### getPlatformFlags

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<Arg> getPlatformFlags()
            ```

            ::: block
            [Description copied from
            class: `CxxToolFlags`]{.descfrmTypeLabel}
            :::

            ::: block
            Flags that precede flags from `#getRuleFlags()`.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPlatformFlags` in class `CxxToolFlags`

        []{#getRuleFlags()}

        -   #### getRuleFlags

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<Arg> getRuleFlags()
            ```

            ::: block
            [Description copied from
            class: `CxxToolFlags`]{.descfrmTypeLabel}
            :::

            ::: block
            Flags that succeed flags from `#getPlatformFlags()`.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRuleFlags` in class `CxxToolFlags`

        []{#addCxxToolFlags(com.facebook.buck.cxx.ExplicitCxxToolFlags.Builder,com.facebook.buck.cxx.CxxToolFlags)}

        -   #### addCxxToolFlags

            ``` methodSignature
            public static void addCxxToolFlags​(ExplicitCxxToolFlags.Builder builder,
                                               CxxToolFlags flags)
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

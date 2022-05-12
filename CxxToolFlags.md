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

## Class CxxToolFlags {#class-cxxtoolflags .title title="Class CxxToolFlags"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.CxxToolFlags

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `ExplicitCxxToolFlags`

    ------------------------------------------------------------------------

        public abstract class CxxToolFlags
        extends Object
        implements AddsToRuleKey

    ::: block
    Tracks flags passed to the preprocessor or compiler.
    Flags derived from the \"platform\" are differentiated from flags
    derived from the \"rule\" to allow for rule flags to override
    platform flags. This is particularly important when the platform and
    rule flags from different sources are merged together.

    Users should use the API in this class instead of the concrete
    implementations.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor        Description
          ------------------ -------------
          `CxxToolFlags()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static CxxToolFlags` | `concat​(Cx            | ::: block             |
        |                       | xToolFlags... parts)` | Concatenate multiple  |
        |                       |                       | flags in a pairwise   |
        |                       |                       | manner.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static CxxToolFlags` | `copy                 | ::: block             |
        |                       | Of​(Iterable<Arg> plat | Directly construct an |
        |                       | formFlags,       Iter | instance from the     |
        |                       | able<Arg> ruleFlags)` | given members.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Explicit      | `explicitBuilder()`   | ::: block             |
        | CxxToolFlags.Builder` |                       | Returns a builder for |
        |                       |                       | explicitly specifying |
        |                       |                       | the flags.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable<Arg>`       | `getAllFlags()`       | ::: block             |
        |                       |                       | Returns all flags in  |
        |                       |                       | the appropriate       |
        |                       |                       | order.                |
        |                       |                       | :::                   |
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
        | `static CxxToolFlags` | `of()`                | ::: block             |
        |                       |                       | Returns the empty     |
        |                       |                       | lists of flags.       |
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

        -   #### CxxToolFlags

                public CxxToolFlags()
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
            Flags that precede flags from `#getRuleFlags()`.
            :::

        []{#getRuleFlags()}

        -   #### getRuleFlags

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<Arg> getRuleFlags()
            ```

            ::: block
            Flags that succeed flags from `#getPlatformFlags()`.
            :::

        []{#getAllFlags()}

        -   #### getAllFlags

            ``` methodSignature
            public final Iterable<Arg> getAllFlags()
            ```

            ::: block
            Returns all flags in the appropriate order.
            :::

        []{#explicitBuilder()}

        -   #### explicitBuilder

            ``` methodSignature
            public static ExplicitCxxToolFlags.Builder explicitBuilder()
            ```

            ::: block
            Returns a builder for explicitly specifying the flags.
            :::

        []{#of()}

        -   #### of

            ``` methodSignature
            public static CxxToolFlags of()
            ```

            ::: block
            Returns the empty lists of flags.
            :::

        []{#copyOf(java.lang.Iterable,java.lang.Iterable)}

        -   #### copyOf

            ``` methodSignature
            public static CxxToolFlags copyOf​(Iterable<Arg> platformFlags,
                                              Iterable<Arg> ruleFlags)
            ```

            ::: block
            Directly construct an instance from the given members.
            :::

        []{#concat(com.facebook.buck.cxx.CxxToolFlags...)}

        -   #### concat

            ``` methodSignature
            public static CxxToolFlags concat​(CxxToolFlags... parts)
            ```

            ::: block
            Concatenate multiple flags in a pairwise manner.
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

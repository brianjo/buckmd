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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.cxx.toolchain.nativelink](package-summary.html)
:::

## Class NativeLinkableInput {#class-nativelinkableinput .title title="Class NativeLinkableInput"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.toolchain.nativelink.NativeLinkableInput

::: description
-   

    ------------------------------------------------------------------------

        public abstract class NativeLinkableInput
        extends Object

    ::: block
    A class containing inputs to be passed to the native linker.
    Dependencies (e.g. C++ libraries) of a top-level native linkable
    rule (e.g. C++ binary) can use this to contribute components to the
    final link.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                           Description
          ------------------- ------------------------------- -------------
          `static class `     `NativeLinkableInput.Builder`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor               Description
          ------------------------- -------------
          `NativeLinkableInput()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static NativeL       | `builder()`           |                       |
        | inkableInput.Builder` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `co                   | ::: block             |
        |  NativeLinkableInput` | ncat​(Iterable<NativeL | Combine, in order,    |
        |                       | inkableInput> items)` | several               |
        |                       |                       | [`NativeLinkableInp   |
        |                       |                       | ut`](NativeLinkableIn |
        |                       |                       | put.html "class in co |
        |                       |                       | m.facebook.buck.cxx.t |
        |                       |                       | oolchain.nativelink") |
        |                       |                       | objects into a single |
        |                       |                       | one.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract com         | `getArgs()`           |                       |
        | .google.common.collec |                       |                       |
        | t.ImmutableList<Arg>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getFrameworks()`     |                       |
        | abstract com.google.c |                       |                       |
        | ommon.collect.Immutab |                       |                       |
        | leSet<FrameworkPath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getLibraries()`      |                       |
        | abstract com.google.c |                       |                       |
        | ommon.collect.Immutab |                       |                       |
        | leSet<FrameworkPath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `of()`                |                       |
        |  NativeLinkableInput` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `                     |                       |
        |  NativeLinkableInput` | of​(List<Arg> args,    |                       |
        |                       | Set<FrameworkPath> fr |                       |
        |                       | ameworks,   Set<Frame |                       |
        |                       | workPath> libraries)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `NativeLinkableInput` | `with                 |                       |
        |                       | Args​(List<Arg> args)` |                       |
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

        -   #### NativeLinkableInput

                public NativeLinkableInput()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getArgs()}

        -   #### getArgs

            ``` methodSignature
            @Parameter
            public abstract com.google.common.collect.ImmutableList<Arg> getArgs()
            ```

        []{#getFrameworks()}

        -   #### getFrameworks

            ``` methodSignature
            @Parameter
            public abstract com.google.common.collect.ImmutableSet<FrameworkPath> getFrameworks()
            ```

        []{#getLibraries()}

        -   #### getLibraries

            ``` methodSignature
            @Parameter
            public abstract com.google.common.collect.ImmutableSet<FrameworkPath> getLibraries()
            ```

        []{#concat(java.lang.Iterable)}

        -   #### concat

            ``` methodSignature
            public static NativeLinkableInput concat​(Iterable<NativeLinkableInput> items)
            ```

            ::: block
            Combine, in order, several
            [`NativeLinkableInput`](NativeLinkableInput.html "class in com.facebook.buck.cxx.toolchain.nativelink")
            objects into a single one.
            :::

        []{#withArgs(java.util.List)}

        -   #### withArgs

            ``` methodSignature
            public NativeLinkableInput withArgs​(List<Arg> args)
            ```

        []{#of()}

        -   #### of

            ``` methodSignature
            public static NativeLinkableInput of()
            ```

        []{#of(java.util.List,java.util.Set,java.util.Set)}

        -   #### of

            ``` methodSignature
            public static NativeLinkableInput of​(List<Arg> args,
                                                 Set<FrameworkPath> frameworks,
                                                 Set<FrameworkPath> libraries)
            ```

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static NativeLinkableInput.Builder builder()
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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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

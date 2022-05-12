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
[Package]{.packageLabelInType} [com.facebook.buck.core.sourcepath](package-summary.html)
:::

## Class DefaultBuildTargetSourcePath {#class-defaultbuildtargetsourcepath .title title="Class DefaultBuildTargetSourcePath"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.sourcepath.DefaultBuildTargetSourcePath

::: description
-   

    All Implemented Interfaces:
    :   `BuildTargetSourcePath`, `SourcePath`, `Comparable<SourcePath>`

    ------------------------------------------------------------------------

        public abstract class DefaultBuildTargetSourcePath
        extends Object
        implements BuildTargetSourcePath

    ::: block
    A
    [`BuildTargetSourcePath`](BuildTargetSourcePath.html "interface in com.facebook.buck.core.sourcepath")
    which resolves to the default output of the
    [`BuildRule`](../rules/BuildRule.html "interface in com.facebook.buck.core.rules")
    referred to by its target.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                        Description
          ---------------------------------- -------------
          `DefaultBuildTargetSourcePath()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `int`                 | `compare              |                       |
        |                       | To​(SourcePath other)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `                     |                       |
        |                       | equals​(Object other)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract             | `                     | ::: block             |
        | Optional<com.google.c | getPrecomputedHash()` | In rare cases, a      |
        | ommon.hash.HashCode>` |                       | BuildTargetSourcePath |
        |                       |                       | may know a hash of    |
        |                       |                       | its content on disk   |
        |                       |                       | before it even        |
        |                       |                       | creates its output.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Bu          | `ge                   |                       |
        | ildTargetWithOutputs` | tTargetWithOutputs()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static DefaultB      | `of                   | ::: block             |
        | uildTargetSourcePath` | ​(BuildTarget target)` | Returns a default     |
        |                       |                       | [`BuildTargetSourc    |
        |                       |                       | ePath`](BuildTargetSo |
        |                       |                       | urcePath.html "interf |
        |                       |                       | ace in com.facebook.b |
        |                       |                       | uck.core.sourcepath") |
        |                       |                       | with an empty output  |
        |                       |                       | label.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static DefaultB      | `of​(                  | ::: block             |
        | uildTargetSourcePath` | BuildTargetWithOutput | Construct a new       |
        |                       | s targetWithOutputs)` | immutable             |
        |                       |                       | `DefaultB             |
        |                       |                       | uildTargetSourcePath` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static DefaultB      | `of​(BuildTar          |                       |
        | uildTargetSourcePath` | getWithOutputs target |                       |
        |                       | WithOutputs,   Option |                       |
        |                       | al<? extends com.goog |                       |
        |                       | le.common.hash.HashCo |                       |
        |                       | de> precomputedHash)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          |                       |
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

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.sourcepath.BuildTargetSourcePath}

            ### Methods inherited from interface com.facebook.buck.core.sourcepath.[BuildTargetSourcePath](BuildTargetSourcePath.html "interface in com.facebook.buck.core.sourcepath")

            `getTarget, representationForRuleKey`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.sourcepath.SourcePath}

            ### Methods inherited from interface com.facebook.buck.core.sourcepath.[SourcePath](SourcePath.html "interface in com.facebook.buck.core.sourcepath")

            `compareClasses`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### DefaultBuildTargetSourcePath

                public DefaultBuildTargetSourcePath()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#of(com.facebook.buck.core.model.BuildTarget)}

        -   #### of

            ``` methodSignature
            public static DefaultBuildTargetSourcePath of​(BuildTarget target)
            ```

            ::: block
            Returns a default
            [`BuildTargetSourcePath`](BuildTargetSourcePath.html "interface in com.facebook.buck.core.sourcepath")
            with an empty output label.
            :::

        []{#of(com.facebook.buck.core.model.BuildTargetWithOutputs)}

        -   #### of

            ``` methodSignature
            public static DefaultBuildTargetSourcePath of​(BuildTargetWithOutputs targetWithOutputs)
            ```

            ::: block
            Construct a new immutable `DefaultBuildTargetSourcePath`
            instance.
            :::

            [Parameters:]{.paramLabel}
            :   `targetWithOutputs` - The value for the
                `targetWithOutputs` attribute

            [Returns:]{.returnLabel}
            :   An immutable DefaultBuildTargetSourcePath instance

        []{#of(com.facebook.buck.core.model.BuildTargetWithOutputs,java.util.Optional)}

        -   #### of

            ``` methodSignature
            public static DefaultBuildTargetSourcePath of​(BuildTargetWithOutputs targetWithOutputs,
                                                          Optional<? extends com.google.common.hash.HashCode> precomputedHash)
            ```

        []{#getTargetWithOutputs()}

        -   #### getTargetWithOutputs

            ``` methodSignature
            public abstract BuildTargetWithOutputs getTargetWithOutputs()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTargetWithOutputs` in
                interface `BuildTargetSourcePath`

            [Returns:]{.returnLabel}
            :   the
                [`BuildTargetWithOutputs`](../model/BuildTargetWithOutputs.html "class in com.facebook.buck.core.model")
                this `SourcePath` is associated with

        []{#getPrecomputedHash()}

        -   #### getPrecomputedHash

            ``` methodSignature
            public abstract Optional<com.google.common.hash.HashCode> getPrecomputedHash()
            ```

            ::: block
            [Description copied from
            interface: `BuildTargetSourcePath`]{.descfrmTypeLabel}
            :::

            ::: block
            In rare cases, a BuildTargetSourcePath may know a hash of
            its content on disk before it even creates its output. In
            this case, we can skip hashing its output files entirely and
            simply use this precomputed hash code. Use Optional.empty()
            in the common case.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPrecomputedHash` in
                interface `BuildTargetSourcePath`

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `Object`

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(Object other)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `Object`

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

        []{#compareTo(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### compareTo

            ``` methodSignature
            public int compareTo​(SourcePath other)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `compareTo` in interface `Comparable<SourcePath>`
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

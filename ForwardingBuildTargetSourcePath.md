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

## Class ForwardingBuildTargetSourcePath {#class-forwardingbuildtargetsourcepath .title title="Class ForwardingBuildTargetSourcePath"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.sourcepath.ForwardingBuildTargetSourcePath

::: description
-   

    All Implemented Interfaces:
    :   `BuildTargetSourcePath`, `SourcePath`, `Comparable<SourcePath>`

    ------------------------------------------------------------------------

        public abstract class ForwardingBuildTargetSourcePath
        extends Object
        implements BuildTargetSourcePath

    ::: block
    A
    [`BuildTargetSourcePath`](BuildTargetSourcePath.html "interface in com.facebook.buck.core.sourcepath")
    which resolves to the value of another SourcePath.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                           Description
          ------------------------------------- -------------
          `ForwardingBuildTargetSourcePath()`    

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
        | `abstract SourcePath` | `getDelegate()`       |                       |
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
        | `static ForwardingB   | `of​(B                 | ::: block             |
        | uildTargetSourcePath` | uildTarget target,    | Construct a new       |
        |                       | SourcePath delegate)` | immutable             |
        |                       |                       | `ForwardingB          |
        |                       |                       | uildTargetSourcePath` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static ForwardingB   | `of​(BuildTargetW      | ::: block             |
        | uildTargetSourcePath` | ithOutputs target,    | Construct a new       |
        |                       | SourcePath delegate)` | immutable             |
        |                       |                       | `ForwardingB          |
        |                       |                       | uildTargetSourcePath` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static ForwardingB   | `of                   |                       |
        | uildTargetSourcePath` | ​(BuildTargetWithOutpu |                       |
        |                       | ts target,   SourcePa |                       |
        |                       | th delegate,   Option |                       |
        |                       | al<? extends com.goog |                       |
        |                       | le.common.hash.HashCo |                       |
        |                       | de> precomputedHash)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `repres               |                       |
        |                       | entationForRuleKey()` |                       |
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

            `getTarget`

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

        -   #### ForwardingBuildTargetSourcePath

                public ForwardingBuildTargetSourcePath()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#of(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### of

            ``` methodSignature
            public static ForwardingBuildTargetSourcePath of​(BuildTarget target,
                                                             SourcePath delegate)
            ```

            ::: block
            Construct a new immutable `ForwardingBuildTargetSourcePath`
            instance.
            :::

            [Parameters:]{.paramLabel}
            :   `target` - The value for the `target` attribute
            :   `delegate` - The value for the `delegate` attribute

            [Returns:]{.returnLabel}
            :   An immutable ForwardingBuildTargetSourcePath instance
                pointing to the given target\'s default outputs

        []{#of(com.facebook.buck.core.model.BuildTargetWithOutputs,com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### of

            ``` methodSignature
            public static ForwardingBuildTargetSourcePath of​(BuildTargetWithOutputs target,
                                                             SourcePath delegate)
            ```

            ::: block
            Construct a new immutable `ForwardingBuildTargetSourcePath`
            instance.
            :::

            [Parameters:]{.paramLabel}
            :   `target` - The
                [`BuildTargetWithOutputs`](../model/BuildTargetWithOutputs.html "class in com.facebook.buck.core.model")
                associated with this
                [`SourcePath`](SourcePath.html "interface in com.facebook.buck.core.sourcepath")
            :   `delegate` - The value for the `delegate` attribute

            [Returns:]{.returnLabel}
            :   An immutable ForwardingBuildTargetSourcePath instance
                pointing to outputs associated with the given
                `targetWithOutputs`

        []{#of(com.facebook.buck.core.model.BuildTargetWithOutputs,com.facebook.buck.core.sourcepath.SourcePath,java.util.Optional)}

        -   #### of

            ``` methodSignature
            public static ForwardingBuildTargetSourcePath of​(BuildTargetWithOutputs target,
                                                             SourcePath delegate,
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

        []{#getDelegate()}

        -   #### getDelegate

            ``` methodSignature
            public abstract SourcePath getDelegate()
            ```

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

        []{#representationForRuleKey()}

        -   #### representationForRuleKey

            ``` methodSignature
            public String representationForRuleKey()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `representationForRuleKey` in
                interface `BuildTargetSourcePath`

            [Returns:]{.returnLabel}
            :   a string that is safe to use for rule key calculations,
                i.e. does not include absolute paths.
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

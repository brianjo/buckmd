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
[Package]{.packageLabelInType} [com.facebook.buck.core.model](package-summary.html)
:::

## Class BuildTargetWithOutputs {#class-buildtargetwithoutputs .title title="Class BuildTargetWithOutputs"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.model.BuildTargetWithOutputs

::: description
-   

    All Implemented Interfaces:
    :   `Comparable<BuildTargetWithOutputs>`

    ------------------------------------------------------------------------

        public abstract class BuildTargetWithOutputs
        extends Object
        implements Comparable<BuildTargetWithOutputs>

    ::: block
    Wrapper for a build target and its output label.
    For example, for the target `//:foo`, the build target would be
    `//:foo`, and the output label would be empty.

    For the target `//:foo[baz]`, the build target would be `//:foo`,
    and the output label would be `baz`.

    For the target `//:foo#flavor[baz]`, the build target would be
    `//:foo#flavor`, and the output label would be `baz`.

    See also
    [`UnconfiguredBuildTargetWithOutputs`](UnconfiguredBuildTargetWithOutputs.html "class in com.facebook.buck.core.model")
    for outputs with unconfigured build targets.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                  Description
          ---------------------------- -------------
          `BuildTargetWithOutputs()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `int`                 | `compareTo​(BuildTarg  |                       |
        |                       | etWithOutputs other)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getBuildTarget()`    | ::: block             |
        | abstract BuildTarget` |                       | Returns the           |
        |                       |                       | associated            |
        |                       |                       | [`BuildTarg           |
        |                       |                       | et`](BuildTarget.html |
        |                       |                       |  "class in com.facebo |
        |                       |                       | ok.buck.core.model"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getOutputLabel()`    | ::: block             |
        | abstract OutputLabel` |                       | Returns the output    |
        |                       |                       | label associated with |
        |                       |                       | the build target, if  |
        |                       |                       | any.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Bu            | `of​(BuildTarge        |                       |
        | ildTargetWithOutputs` | t buildTarget,   Outp |                       |
        |                       | utLabel outputLabel)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          | ::: block             |
        |                       |                       | Returns the string    |
        |                       |                       | representation of a   |
        |                       |                       | `Bu                   |
        |                       |                       | ildTargetWithOutputs` |
        |                       |                       | in the form of        |
        |                       |                       | target                |
        |                       |                       | _name\[output_label\] |
        |                       |                       | if an output label is |
        |                       |                       | present.              |
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

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### BuildTargetWithOutputs

                public BuildTargetWithOutputs()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBuildTarget()}

        -   #### getBuildTarget

            ``` methodSignature
            public abstract BuildTarget getBuildTarget()
            ```

            ::: block
            Returns the associated
            [`BuildTarget`](BuildTarget.html "class in com.facebook.buck.core.model").
            :::

        []{#getOutputLabel()}

        -   #### getOutputLabel

            ``` methodSignature
            public abstract OutputLabel getOutputLabel()
            ```

            ::: block
            Returns the output label associated with the build target,
            if any.
            :::

        []{#compareTo(com.facebook.buck.core.model.BuildTargetWithOutputs)}

        -   #### compareTo

            ``` methodSignature
            public int compareTo​(BuildTargetWithOutputs other)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `compareTo` in
                interface `Comparable<BuildTargetWithOutputs>`

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            ::: block
            Returns the string representation of a
            `BuildTargetWithOutputs` in the form of
            target_name\[output_label\] if an output label is present.
            E.g. //foo:bar\[baz\]. If no output label is present, the
            square brackets are omitted. E.g. //foo:bar
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

        []{#of(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.model.OutputLabel)}

        -   #### of

            ``` methodSignature
            public static BuildTargetWithOutputs of​(BuildTarget buildTarget,
                                                    OutputLabel outputLabel)
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

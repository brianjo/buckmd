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

## Class UnconfiguredBuildTargetWithOutputs {#class-unconfiguredbuildtargetwithoutputs .title title="Class UnconfiguredBuildTargetWithOutputs"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.model.UnconfiguredBuildTargetWithOutputs

::: description
-   

    All Implemented Interfaces:
    :   `Comparable<UnconfiguredBuildTargetWithOutputs>`

    ------------------------------------------------------------------------

        public abstract class UnconfiguredBuildTargetWithOutputs
        extends Object
        implements Comparable<UnconfiguredBuildTargetWithOutputs>

    ::: block
    Wrapper for an unconfigured build target and its output label.
    For example, for the target `//:foo`, the unconfigured target would
    be `//:foo`, and the output label would be empty.

    For the target `//:foo[baz]`, the unconfigured target would be
    `//:foo`, and the output label would be `baz`.

    For the target `//:foo#flavor[baz]`, the unconfigured target would
    be `  //:foo#flavor`, and the output label would be `baz`.

    See also
    [`BuildTargetWithOutputs`](BuildTargetWithOutputs.html "class in com.facebook.buck.core.model")
    for outputs with configured build targets.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                              Description
          ---------------------------------------- -------------
          `UnconfiguredBuildTargetWithOutputs()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `int`                 | `compareTo​(           |                       |
        |                       | UnconfiguredBuildTarg |                       |
        |                       | etWithOutputs other)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Bu                   | `configure            | ::: block             |
        | ildTargetWithOutputs` | ​(TargetConfiguration  | Apply the             |
        |                       | targetConfiguration)` | configuration.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Unc         | `getBuildTarget()`    | ::: block             |
        | onfiguredBuildTarget` |                       | Returns the           |
        |                       |                       | associated            |
        |                       |                       | [`Unconfigured        |
        |                       |                       | BuildTarget`](Unconfi |
        |                       |                       | guredBuildTarget.html |
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
        | `                     | `of​(U                 |                       |
        | static UnconfiguredBu | nconfiguredBuildTarge |                       |
        | ildTargetWithOutputs` | t buildTarget,   Outp |                       |
        |                       | utLabel outputLabel)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          | ::: block             |
        |                       |                       | Returns the string    |
        |                       |                       | representation of a   |
        |                       |                       | `UnconfiguredBu       |
        |                       |                       | ildTargetWithOutputs` |
        |                       |                       | in the form of        |
        |                       |                       | target_               |
        |                       |                       | name\[output_label\]. |
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

        -   #### UnconfiguredBuildTargetWithOutputs

                public UnconfiguredBuildTargetWithOutputs()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBuildTarget()}

        -   #### getBuildTarget

            ``` methodSignature
            public abstract UnconfiguredBuildTarget getBuildTarget()
            ```

            ::: block
            Returns the associated
            [`UnconfiguredBuildTarget`](UnconfiguredBuildTarget.html "class in com.facebook.buck.core.model").
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

        []{#compareTo(com.facebook.buck.core.model.UnconfiguredBuildTargetWithOutputs)}

        -   #### compareTo

            ``` methodSignature
            public int compareTo​(UnconfiguredBuildTargetWithOutputs other)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `compareTo` in
                interface `Comparable<UnconfiguredBuildTargetWithOutputs>`

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            ::: block
            Returns the string representation of a
            `UnconfiguredBuildTargetWithOutputs` in the form of
            target_name\[output_label\]. E.g. //foo:bar\[baz\]. If no
            output label is available, the square brackets are omitted.
            E.g. //foo:bar
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

        []{#of(com.facebook.buck.core.model.UnconfiguredBuildTarget,com.facebook.buck.core.model.OutputLabel)}

        -   #### of

            ``` methodSignature
            public static UnconfiguredBuildTargetWithOutputs of​(UnconfiguredBuildTarget buildTarget,
                                                                OutputLabel outputLabel)
            ```

        []{#configure(com.facebook.buck.core.model.TargetConfiguration)}

        -   #### configure

            ``` methodSignature
            public BuildTargetWithOutputs configure​(TargetConfiguration targetConfiguration)
            ```

            ::: block
            Apply the configuration.
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

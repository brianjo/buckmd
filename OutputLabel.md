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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
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

## Class OutputLabel {#class-outputlabel .title title="Class OutputLabel"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.model.OutputLabel

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`, `Comparable<OutputLabel>`

    ------------------------------------------------------------------------

        public class OutputLabel
        extends Object
        implements Comparable<OutputLabel>, AddsToRuleKey

    ::: block
    Type-safe wrapper for a target output label.
    A build target can return different outputs groups, with each output
    group potentially containing zero or more outputs. A target output
    label is used to refer to a particular output group in a target.

    With providers, the output label maps to named output groups in
    [`DefaultInfo`](../rules/providers/lib/DefaultInfo.html "class in com.facebook.buck.core.rules.providers.lib").
    With the old action graph, each rule should maintain an internal
    mapping of output labels to output groups.

    A [`DEFAULT`](#DEFAULT) output label is provided when the user has
    not specified a named output label in a build target. For example,
    \"//foo:bar\" would be associated with the default output label,
    whereas \"//foo:bar\[baz\] would be associated with the named label
    \"baz\".
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `O                    | ::: block             |
        |                       | utputLabel.Internals` | Provides access to    |
        |                       |                       | internal              |
        |                       |                       | implementation        |
        |                       |                       | details of            |
        |                       |                       | OutputLabels.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `int`                 | `comp                 |                       |
        |                       | areTo​(OutputLabel o)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static OutputLabel`  | `defaultLabel()`      | ::: block             |
        |                       |                       | Returns the output    |
        |                       |                       | label for default     |
        |                       |                       | outputs.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `equals​(Object o)`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static O             | `internals()`         |                       |
        | utputLabel.Internals` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isDefault()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static OutputLabel`  | `of​(String label)`    | ::: block             |
        |                       |                       | Returns an output     |
        |                       |                       | label wrapping the    |
        |                       |                       | given String.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#of(java.lang.String)}

        -   #### of

            ``` methodSignature
            public static OutputLabel of​(String label)
            ```

            ::: block
            Returns an output label wrapping the given String. Use
            [`defaultLabel()`](#defaultLabel()) to get the default empty
            output label.
            :::

            [Throws:]{.throwsLabel}
            :   `IllegalArgumentException` - if the given `label` is an
                empty string

        []{#defaultLabel()}

        -   #### defaultLabel

            ``` methodSignature
            public static OutputLabel defaultLabel()
            ```

            ::: block
            Returns the output label for default outputs.
            :::

        []{#isDefault()}

        -   #### isDefault

            ``` methodSignature
            public boolean isDefault()
            ```

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(Object o)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `Object`

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `Object`

        []{#compareTo(com.facebook.buck.core.model.OutputLabel)}

        -   #### compareTo

            ``` methodSignature
            public int compareTo​(OutputLabel o)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `compareTo` in interface `Comparable<OutputLabel>`

        []{#internals()}

        -   #### internals

            ``` methodSignature
            public static OutputLabel.Internals internals()
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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

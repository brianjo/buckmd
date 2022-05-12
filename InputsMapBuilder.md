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
[Package]{.packageLabelInType} [com.facebook.buck.rules.modern.impl](package-summary.html)
:::

## Class InputsMapBuilder {#class-inputsmapbuilder .title title="Class InputsMapBuilder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.modern.impl.InputsMapBuilder

::: description
-   

    ------------------------------------------------------------------------

        public class InputsMapBuilder
        extends Object

    ::: block
    InputsMapBuilder is used to find all the input SourcePaths of a
    Buildable. For each instance of an
    [`AddsToRuleKey`](../../../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey")
    object that directly references other AddsToRuleKey objects or
    SourcePaths, or
    [`InputsMapBuilder.Data`](InputsMapBuilder.Data.html "class in com.facebook.buck.rules.modern.impl")
    node will be created. This allows two things: (1) we don\'t need to
    traverse the object structure of shared appendables multiple times
    and (2) it is easy for consumers to cache computed information based
    on this derived graph.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `I                    | ::: block             |
        |                       | nputsMapBuilder.Data` | Holds the information |
        |                       |                       | derived from a        |
        |                       |                       | rulekey appendable.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor            Description
          ---------------------- -------------
          `InputsMapBuilder()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `I                    | `getInputs​(Mode       |                       |
        | nputsMapBuilder.Data` | rnBuildRule<?> rule)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `<T ex                | `g                    | ::: block             |
        | tends AddsToRuleKey>I | etInputs​(T instance)` | Computes the          |
        | nputsMapBuilder.Data` |                       | \"inputs\" graph of   |
        |                       |                       | rule key appendables. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `<T ex                | `getInputs​(T i        | ::: block             |
        | tends AddsToRuleKey>I | nstance,          Cla | See getInputs(T       |
        | nputsMapBuilder.Data` | ssInfo<T> classInfo)` | instance) above.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
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

        -   #### InputsMapBuilder

                public InputsMapBuilder()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getInputs(com.facebook.buck.core.rulekey.AddsToRuleKey)}
        []{#getInputs(T)}

        -   #### getInputs

            ``` methodSignature
            public <T extends AddsToRuleKey> InputsMapBuilder.Data getInputs​(T instance)
            ```

            ::: block
            Computes the \"inputs\" graph of rule key appendables.
            Returns the root of that graph.
            :::

        []{#getInputs(com.facebook.buck.rules.modern.ModernBuildRule)}

        -   #### getInputs

            ``` methodSignature
            public InputsMapBuilder.Data getInputs​(ModernBuildRule<?> rule)
            ```

        []{#getInputs(com.facebook.buck.core.rulekey.AddsToRuleKey,com.facebook.buck.rules.modern.ClassInfo)}
        []{#getInputs(T,com.facebook.buck.rules.modern.ClassInfo)}

        -   #### getInputs

            ``` methodSignature
            public <T extends AddsToRuleKey> InputsMapBuilder.Data getInputs​(T instance,
                                                                             ClassInfo<T> classInfo)
            ```

            ::: block
            See getInputs(T instance) above.
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

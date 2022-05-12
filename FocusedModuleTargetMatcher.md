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
-   Nested \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.features.apple.project](package-summary.html)
:::

## Class FocusedModuleTargetMatcher {#class-focusedmoduletargetmatcher .title title="Class FocusedModuleTargetMatcher"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.apple.project.FocusedModuleTargetMatcher

::: description
-   

    ------------------------------------------------------------------------

        public final class FocusedModuleTargetMatcher
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static Focuse        | `focusedOn​(com.goog   | ::: block             |
        | dModuleTargetMatcher` | le.common.collect.Imm | Returns a matcher     |
        |                       | utableSet<UnflavoredB | that specifies a set  |
        |                       | uildTarget> targets)` | of targets to focus   |
        |                       |                       | on.                   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `hasFocus()`          | ::: block             |
        |                       |                       | Returns whether any   |
        |                       |                       | focus is set.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isFocusedOn​(Buil     | ::: block             |
        |                       | dTarget buildTarget)` | Test whether target   |
        |                       |                       | matches any focused   |
        |                       |                       | targets.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Focuse               | `map​(java.util.func   | ::: block             |
        | dModuleTargetMatcher` | tion.Function<com.goo | Apply a mapper to the |
        |                       | gle.common.collect.Im | focused targets held  |
        |                       | mutableSet<Unflavored | in this object.       |
        |                       | BuildTarget>,​com.goog | :::                   |
        |                       | le.common.collect.Imm |                       |
        |                       | utableSet<UnflavoredB |                       |
        |                       | uildTarget>> mapper)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Focuse        | `noFocus()`           | ::: block             |
        | dModuleTargetMatcher` |                       | Returns a matcher     |
        |                       |                       | that matches          |
        |                       |                       | everything, i.e.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
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
    -   []{#method.detail}

        ### Method Detail

        []{#noFocus()}

        -   #### noFocus

            ``` methodSignature
            public static FocusedModuleTargetMatcher noFocus()
            ```

            ::: block
            Returns a matcher that matches everything, i.e. no focus.
            :::

        []{#focusedOn(com.google.common.collect.ImmutableSet)}

        -   #### focusedOn

            ``` methodSignature
            public static FocusedModuleTargetMatcher focusedOn​(com.google.common.collect.ImmutableSet<UnflavoredBuildTarget> targets)
            ```

            ::: block
            Returns a matcher that specifies a set of targets to focus
            on.
            :::

        []{#hasFocus()}

        -   #### hasFocus

            ``` methodSignature
            public boolean hasFocus()
            ```

            ::: block
            Returns whether any focus is set.
            :::

        []{#isFocusedOn(com.facebook.buck.core.model.BuildTarget)}

        -   #### isFocusedOn

            ``` methodSignature
            public boolean isFocusedOn​(BuildTarget buildTarget)
            ```

            ::: block
            Test whether target matches any focused targets.
            If there is no focus, always return true.
            :::

        []{#map(java.util.function.Function)}

        -   #### map

            ``` methodSignature
            public FocusedModuleTargetMatcher map​(java.util.function.Function<com.google.common.collect.ImmutableSet<UnflavoredBuildTarget>,​com.google.common.collect.ImmutableSet<UnflavoredBuildTarget>> mapper)
            ```

            ::: block
            Apply a mapper to the focused targets held in this object.
            If no focus is set, this is a no-op.
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
-   Nested \| 
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

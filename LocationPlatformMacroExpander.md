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
[Package]{.packageLabelInType} [com.facebook.buck.rules.macros](package-summary.html)
:::

## Class LocationPlatformMacroExpander {#class-locationplatformmacroexpander .title title="Class LocationPlatformMacroExpander"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.rules.macros.AbstractMacroExpanderWithoutPrecomputedWork](AbstractMacroExpanderWithoutPrecomputedWork.html "class in com.facebook.buck.rules.macros")\<M\>

    -   -   [com.facebook.buck.rules.macros.BuildTargetMacroExpander](BuildTargetMacroExpander.html "class in com.facebook.buck.rules.macros")\<T\>

        -   -   [com.facebook.buck.rules.macros.AbstractLocationMacroExpander](AbstractLocationMacroExpander.html "class in com.facebook.buck.rules.macros")\<[LocationPlatformMacro](LocationPlatformMacro.html "class in com.facebook.buck.rules.macros")\>

            -   -   com.facebook.buck.rules.macros.LocationPlatformMacroExpander

::: description
-   

    All Implemented Interfaces:
    :   `MacroExpander<LocationPlatformMacro,​Object>`

    ------------------------------------------------------------------------

        public class LocationPlatformMacroExpander
        extends AbstractLocationMacroExpander<LocationPlatformMacro>

    ::: block
    Expands to the path of a build rules output.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                Description
          ---------------------------------------------------------- -------------
          `LocationPlatformMacroExpander​(CxxPlatform cxxPlatform)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                Method                                                                           Description
          -------------------------------- -------------------------------------------------------------------------------- -------------
          `Class<LocationPlatformMacro>`   `getInputClass()`                                                                 
          `protected BuildRule`            `resolve​(ActionGraphBuilder graphBuilder,        LocationPlatformMacro input)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.rules.macros.AbstractLocationMacroExpander}

            ### Methods inherited from class com.facebook.buck.rules.macros.[AbstractLocationMacroExpander](AbstractLocationMacroExpander.html "class in com.facebook.buck.rules.macros")

            `expand`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.rules.macros.BuildTargetMacroExpander}

            ### Methods inherited from class com.facebook.buck.rules.macros.[BuildTargetMacroExpander](BuildTargetMacroExpander.html "class in com.facebook.buck.rules.macros")

            `expandFrom`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.rules.macros.AbstractMacroExpanderWithoutPrecomputedWork}

            ### Methods inherited from class com.facebook.buck.rules.macros.[AbstractMacroExpanderWithoutPrecomputedWork](AbstractMacroExpanderWithoutPrecomputedWork.html "class in com.facebook.buck.rules.macros")

            `expandFrom, precomputeWorkFrom`

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

        []{#<init>(com.facebook.buck.cxx.toolchain.CxxPlatform)}

        -   #### LocationPlatformMacroExpander

                public LocationPlatformMacroExpander​(CxxPlatform cxxPlatform)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getInputClass()}

        -   #### getInputClass

            ``` methodSignature
            public Class<LocationPlatformMacro> getInputClass()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getInputClass` in
                interface `MacroExpander<LocationPlatformMacro,​Object>`

            [Overrides:]{.overrideSpecifyLabel}
            :   `getInputClass` in
                class `AbstractLocationMacroExpander<LocationPlatformMacro>`

            [Returns:]{.returnLabel}
            :   the class for the parsed macro input type.

        []{#resolve(com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.rules.macros.LocationPlatformMacro)}

        -   #### resolve

            ``` methodSignature
            protected BuildRule resolve​(ActionGraphBuilder graphBuilder,
                                        LocationPlatformMacro input)
                                 throws MacroException
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `resolve` in
                class `BuildTargetMacroExpander<LocationPlatformMacro>`

            [Throws:]{.throwsLabel}
            :   `MacroException`
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

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

## Class LocationPlatformMacro {#class-locationplatformmacro .title title="Class LocationPlatformMacro"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.rules.macros.BuildTargetMacro](BuildTargetMacro.html "class in com.facebook.buck.rules.macros")

    -   -   [com.facebook.buck.rules.macros.BaseLocationMacro](BaseLocationMacro.html "class in com.facebook.buck.rules.macros")

        -   -   com.facebook.buck.rules.macros.LocationPlatformMacro

::: description
-   

    All Implemented Interfaces:
    :   `Macro`, `TargetTranslatable<Macro>`

    ------------------------------------------------------------------------

        public abstract class LocationPlatformMacro
        extends BaseLocationMacro

    ::: block
    Macro that resolves to the output location of a build rule.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                 Description
          --------------------------- -------------
          `LocationPlatformMacro()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                   Method                                                                      Description
          ----------------------------------- --------------------------------------------------------------------------- -------------
          `boolean`                           `equals​(Object another)`                                                     
          `Class<? extends Macro>`            `getMacroClass()`                                                            
          `abstract BuildTargetWithOutputs`   `getTargetWithOutputs()`                                                     
          `int`                               `hashCode()`                                                                 
          `static LocationPlatformMacro`      `of​(BuildTargetWithOutputs target,   Iterable<? extends Flavor> flavors)`    
          `protected LocationPlatformMacro`   `withTargetWithOutputs​(BuildTargetWithOutputs target)`                       

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.rules.macros.BuildTargetMacro}

            ### Methods inherited from class com.facebook.buck.rules.macros.[BuildTargetMacro](BuildTargetMacro.html "class in com.facebook.buck.rules.macros")

            `getTarget, translateTargets`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### LocationPlatformMacro

                public LocationPlatformMacro()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getTargetWithOutputs()}

        -   #### getTargetWithOutputs

            ``` methodSignature
            public abstract BuildTargetWithOutputs getTargetWithOutputs()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTargetWithOutputs` in class `BuildTargetMacro`

        []{#getMacroClass()}

        -   #### getMacroClass

            ``` methodSignature
            public Class<? extends Macro> getMacroClass()
            ```

        []{#withTargetWithOutputs(com.facebook.buck.core.model.BuildTargetWithOutputs)}

        -   #### withTargetWithOutputs

            ``` methodSignature
            protected LocationPlatformMacro withTargetWithOutputs​(BuildTargetWithOutputs target)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `withTargetWithOutputs` in class `BuildTargetMacro`

            [Returns:]{.returnLabel}
            :   a copy of this
                [`BuildTargetMacro`](BuildTargetMacro.html "class in com.facebook.buck.rules.macros")
                with the given
                [`BuildTargetWithOutputs`](../../core/model/BuildTargetWithOutputs.html "class in com.facebook.buck.core.model").

        []{#of(com.facebook.buck.core.model.BuildTargetWithOutputs,java.lang.Iterable)}

        -   #### of

            ``` methodSignature
            public static LocationPlatformMacro of​(BuildTargetWithOutputs target,
                                                   Iterable<? extends Flavor> flavors)
            ```

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `BuildTargetMacro`

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(@Nullable
                                  Object another)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `BuildTargetMacro`
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

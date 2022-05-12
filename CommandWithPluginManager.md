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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.cli](package-summary.html)
:::

## Class CommandWithPluginManager {#class-commandwithpluginmanager .title title="Class CommandWithPluginManager"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cli.CommandWithPluginManager

::: description
-   

    All Implemented Interfaces:
    :   `Command`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `AbstractCommand`, `AbstractContainerCommand`

    ------------------------------------------------------------------------

        public abstract class CommandWithPluginManager
        extends Object
        implements Command

    ::: block
    An implementation of
    [`Command`](Command.html "interface in com.facebook.buck.cli") that
    allows keeping `PluginManager`.
    The `PluginManager` is not passed through the constructor because
    instances of
    [`Command`](Command.html "interface in com.facebook.buck.cli") are
    created by the args4j framework by calling the default constructor
    (the one without arguments). The `PluginManager` is saved by calling
    [`setPluginManager(PluginManager)`](#setPluginManager(org.pf4j.PluginManager))
    right after the creation of the command. Also, CLI arguments are
    parsed on a single thread so we don\'t need to worry about
    concurrent access.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                    Description
          ------------------------------ -------------
          `CommandWithPluginManager()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type          Method                                                     Description
          -------------------------- ---------------------------------------------------------- -------------
          `org.pf4j.PluginManager`   `getPluginManager()`                                        
          `void`                     `setPluginManager​(org.pf4j.PluginManager pluginManager)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.cli.Command}

            ### Methods inherited from interface com.facebook.buck.cli.[Command](Command.html "interface in com.facebook.buck.cli")

            `createParsingContext, getConfigOverrides, getEventListeners, getHostPlatform, getLogConfig, getShortDescription, getTargetPlatforms, isReadOnly, isSourceControlStatsGatheringEnabled, performsBuild, printUsage, run, runHelp`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### CommandWithPluginManager

                public CommandWithPluginManager()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#setPluginManager(org.pf4j.PluginManager)}

        -   #### setPluginManager

            ``` methodSignature
            public void setPluginManager​(org.pf4j.PluginManager pluginManager)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `setPluginManager` in interface `Command`

        []{#getPluginManager()}

        -   #### getPluginManager

            ``` methodSignature
            public org.pf4j.PluginManager getPluginManager()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPluginManager` in interface `Command`
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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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

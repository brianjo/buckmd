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
-   [Enum Constants](#enum.constant.summary) \| 
-   [Field](#field.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Enum Constants](#enum.constant.detail) \| 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.remoteexecution.config](package-summary.html)
:::

## Enum AutoRemoteExecutionStrategy {#enum-autoremoteexecutionstrategy .title title="Enum AutoRemoteExecutionStrategy"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<[AutoRemoteExecutionStrategy](AutoRemoteExecutionStrategy.html "enum in com.facebook.buck.remoteexecution.config")\>

    -   -   com.facebook.buck.remoteexecution.config.AutoRemoteExecutionStrategy

::: description
-   

    All Implemented Interfaces:
    :   `Serializable`, `Comparable<AutoRemoteExecutionStrategy>`

    ------------------------------------------------------------------------

        public enum AutoRemoteExecutionStrategy
        extends Enum<AutoRemoteExecutionStrategy>

    ::: block
    Strategy used to determine whether to enable Remote Execution
    automatically for the current build. If it passes,
    experimental_strategy setting will be used for the build. Note: if
    remoteexecution.strategy is explicitly set, this always takes
    priority over auto RE settings (i.e. remoteexecution.strategy=NONE
    means RE is always disabled)
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#enum.constant.summary}

        ### Enum Constant Summary

          Enum Constant                                    Description
          ------------------------------------------------ -------------
          `DISABLED`                                        
          `RE_IF_EXPERIMENT_ENABLED`                        
          `RE_IF_EXPERIMENT_ENABLED_AND_WHITELIST_MATCH`    
          `RE_IF_EXPERIMENT_ENABLED_OR_WHITELIST_MATCH`     
          `RE_IF_WHITELIST_MATCH`                           

          : Enum Constants[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                      Field       Description
          -------------------------------------- ----------- -------------
          `static AutoRemoteExecutionStrategy`   `DEFAULT`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static AutoRem       | `                     | ::: block             |
        | oteExecutionStrategy` | valueOf​(String name)` | Returns the enum      |
        |                       |                       | constant of this type |
        |                       |                       | with the specified    |
        |                       |                       | name.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static AutoRemot     | `values()`            | ::: block             |
        | eExecutionStrategy[]` |                       | Returns an array      |
        |                       |                       | containing the        |
        |                       |                       | constants of this     |
        |                       |                       | enum type, in the     |
        |                       |                       | order they are        |
        |                       |                       | declared.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Enum}

            ### Methods inherited from class java.lang.[Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, compareTo, equals, finalize, getDeclaringClass, hashCode, name, ordinal, toString, valueOf`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `getClass, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#enum.constant.detail}

        ### Enum Constant Detail

        []{#DISABLED}

        -   #### DISABLED

                public static final AutoRemoteExecutionStrategy DISABLED

        []{#RE_IF_EXPERIMENT_ENABLED}

        -   #### RE_IF_EXPERIMENT_ENABLED

                public static final AutoRemoteExecutionStrategy RE_IF_EXPERIMENT_ENABLED

        []{#RE_IF_WHITELIST_MATCH}

        -   #### RE_IF_WHITELIST_MATCH

                public static final AutoRemoteExecutionStrategy RE_IF_WHITELIST_MATCH

        []{#RE_IF_EXPERIMENT_ENABLED_AND_WHITELIST_MATCH}

        -   #### RE_IF_EXPERIMENT_ENABLED_AND_WHITELIST_MATCH

                public static final AutoRemoteExecutionStrategy RE_IF_EXPERIMENT_ENABLED_AND_WHITELIST_MATCH

        []{#RE_IF_EXPERIMENT_ENABLED_OR_WHITELIST_MATCH}

        -   #### RE_IF_EXPERIMENT_ENABLED_OR_WHITELIST_MATCH

                public static final AutoRemoteExecutionStrategy RE_IF_EXPERIMENT_ENABLED_OR_WHITELIST_MATCH
    :::

    ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#DEFAULT}

        -   #### DEFAULT

                public static final AutoRemoteExecutionStrategy DEFAULT
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#values()}

        -   #### values

            ``` methodSignature
            public static AutoRemoteExecutionStrategy[] values()
            ```

            ::: block
            Returns an array containing the constants of this enum type,
            in the order they are declared. This method may be used to
            iterate over the constants as follows:
                for (AutoRemoteExecutionStrategy c : AutoRemoteExecutionStrategy.values())
                    System.out.println(c);
            :::

            [Returns:]{.returnLabel}
            :   an array containing the constants of this enum type, in
                the order they are declared

        []{#valueOf(java.lang.String)}

        -   #### valueOf

            ``` methodSignature
            public static AutoRemoteExecutionStrategy valueOf​(String name)
            ```

            ::: block
            Returns the enum constant of this type with the specified
            name. The string must match *exactly* an identifier used to
            declare an enum constant in this type. (Extraneous
            whitespace characters are not permitted.)
            :::

            [Parameters:]{.paramLabel}
            :   `name` - the name of the enum constant to be returned.

            [Returns:]{.returnLabel}
            :   the enum constant with the specified name

            [Throws:]{.throwsLabel}
            :   `IllegalArgumentException` - if this enum type has no
                constant with the specified name
            :   `NullPointerException` - if the argument is null
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
-   [Enum Constants](#enum.constant.summary) \| 
-   [Field](#field.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Enum Constants](#enum.constant.detail) \| 
-   [Field](#field.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
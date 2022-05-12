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
-   Field \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Enum Constants](#enum.constant.detail) \| 
-   Field \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.support.state](package-summary.html)
:::

## Enum BuckGlobalStateLifecycleManager.LifecycleStatus {#enum-buckglobalstatelifecyclemanager.lifecyclestatus .title title="Enum BuckGlobalStateLifecycleManager.LifecycleStatus"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<[BuckGlobalStateLifecycleManager.LifecycleStatus](BuckGlobalStateLifecycleManager.LifecycleStatus.html "enum in com.facebook.buck.support.state")\>

    -   -   com.facebook.buck.support.state.BuckGlobalStateLifecycleManager.LifecycleStatus

::: description
-   

    All Implemented Interfaces:
    :   `Serializable`,
        `Comparable<BuckGlobalStateLifecycleManager.LifecycleStatus>`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [BuckGlobalStateLifecycleManager](BuckGlobalStateLifecycleManager.html "class in com.facebook.buck.support.state")

    ------------------------------------------------------------------------

        public static enum BuckGlobalStateLifecycleManager.LifecycleStatus
        extends Enum<BuckGlobalStateLifecycleManager.LifecycleStatus>

    ::: block
    Indicates whether a daemon\'s
    [`BuckGlobalState`](BuckGlobalState.html "class in com.facebook.buck.support.state")
    is reused, or why it can\'t be reused
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#enum.constant.summary}

        ### Enum Constant Summary

          Enum Constant                           Description
          --------------------------------------- -------------
          `INVALIDATED_BUCK_CONFIG_CHANGED`        
          `INVALIDATED_FILESYSTEM_CHANGED`         
          `INVALIDATED_NO_WATCHMAN`                
          `INVALIDATED_TOOLCHAINS_INCOMPATIBLE`    
          `INVALIDATED_WATCHMAN_RESTARTED`         
          `NEW`                                    
          `REUSED`                                 

          : Enum Constants[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Optional<String>`    | `getLif               | ::: block             |
        |                       | ecycleStatusString()` | Get the string to be  |
        |                       |                       | logged as an event,   |
        |                       |                       | if an event should be |
        |                       |                       | logged.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static BuckGl        | `                     | ::: block             |
        | obalStateLifecycleMan | valueOf​(String name)` | Returns the enum      |
        | ager.LifecycleStatus` |                       | constant of this type |
        |                       |                       | with the specified    |
        |                       |                       | name.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static BuckGlob      | `values()`            | ::: block             |
        | alStateLifecycleManag |                       | Returns an array      |
        | er.LifecycleStatus[]` |                       | containing the        |
        |                       |                       | constants of this     |
        |                       |                       | enum type, in the     |
        |                       |                       | order they are        |
        |                       |                       | declared.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
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

        []{#REUSED}

        -   #### REUSED

                public static final BuckGlobalStateLifecycleManager.LifecycleStatus REUSED

        []{#NEW}

        -   #### NEW

                public static final BuckGlobalStateLifecycleManager.LifecycleStatus NEW

        []{#INVALIDATED_NO_WATCHMAN}

        -   #### INVALIDATED_NO_WATCHMAN

                public static final BuckGlobalStateLifecycleManager.LifecycleStatus INVALIDATED_NO_WATCHMAN

        []{#INVALIDATED_WATCHMAN_RESTARTED}

        -   #### INVALIDATED_WATCHMAN_RESTARTED

                public static final BuckGlobalStateLifecycleManager.LifecycleStatus INVALIDATED_WATCHMAN_RESTARTED

        []{#INVALIDATED_FILESYSTEM_CHANGED}

        -   #### INVALIDATED_FILESYSTEM_CHANGED

                public static final BuckGlobalStateLifecycleManager.LifecycleStatus INVALIDATED_FILESYSTEM_CHANGED

        []{#INVALIDATED_BUCK_CONFIG_CHANGED}

        -   #### INVALIDATED_BUCK_CONFIG_CHANGED

                public static final BuckGlobalStateLifecycleManager.LifecycleStatus INVALIDATED_BUCK_CONFIG_CHANGED

        []{#INVALIDATED_TOOLCHAINS_INCOMPATIBLE}

        -   #### INVALIDATED_TOOLCHAINS_INCOMPATIBLE

                public static final BuckGlobalStateLifecycleManager.LifecycleStatus INVALIDATED_TOOLCHAINS_INCOMPATIBLE
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#values()}

        -   #### values

            ``` methodSignature
            public static BuckGlobalStateLifecycleManager.LifecycleStatus[] values()
            ```

            ::: block
            Returns an array containing the constants of this enum type,
            in the order they are declared. This method may be used to
            iterate over the constants as follows:
                for (BuckGlobalStateLifecycleManager.LifecycleStatus c : BuckGlobalStateLifecycleManager.LifecycleStatus.values())
                    System.out.println(c);
            :::

            [Returns:]{.returnLabel}
            :   an array containing the constants of this enum type, in
                the order they are declared

        []{#valueOf(java.lang.String)}

        -   #### valueOf

            ``` methodSignature
            public static BuckGlobalStateLifecycleManager.LifecycleStatus valueOf​(String name)
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

        []{#getLifecycleStatusString()}

        -   #### getLifecycleStatusString

            ``` methodSignature
            public Optional<String> getLifecycleStatusString()
            ```

            ::: block
            Get the string to be logged as an event, if an event should
            be logged.
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
-   [Enum Constants](#enum.constant.summary) \| 
-   Field \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Enum Constants](#enum.constant.detail) \| 
-   Field \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

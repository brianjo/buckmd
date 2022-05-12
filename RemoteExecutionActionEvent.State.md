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
[Package]{.packageLabelInType} [com.facebook.buck.remoteexecution.event](package-summary.html)
:::

## Enum RemoteExecutionActionEvent.State {#enum-remoteexecutionactionevent.state .title title="Enum RemoteExecutionActionEvent.State"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<[RemoteExecutionActionEvent.State](RemoteExecutionActionEvent.State.html "enum in com.facebook.buck.remoteexecution.event")\>

    -   -   com.facebook.buck.remoteexecution.event.RemoteExecutionActionEvent.State

::: description
-   

    All Implemented Interfaces:
    :   `Serializable`, `Comparable<RemoteExecutionActionEvent.State>`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [RemoteExecutionActionEvent](RemoteExecutionActionEvent.html "class in com.facebook.buck.remoteexecution.event")

    ------------------------------------------------------------------------

        public static enum RemoteExecutionActionEvent.State
        extends Enum<RemoteExecutionActionEvent.State>

    ::: block
    The current state of a Remote Execution Actions.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#enum.constant.summary}

        ### Enum Constant Summary

          Enum Constant              Description
          -------------------------- -------------
          `ACTION_CANCELLED`          
          `ACTION_FAILED`             
          `ACTION_SUCCEEDED`          
          `COMPUTING_ACTION`          
          `DELETING_STALE_OUTPUTS`    
          `EXECUTING`                 
          `MATERIALIZING_OUTPUTS`     
          `UPLOADING_ACTION`          
          `UPLOADING_INPUTS`          
          `WAITING`                   

          : Enum Constants[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `String`              | `getAbbreviateName()` | ::: block             |
        |                       |                       | Abbreviated name for  |
        |                       |                       | the current state.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static RemoteExecut  | `                     | ::: block             |
        | ionActionEvent.State` | valueOf​(String name)` | Returns the enum      |
        |                       |                       | constant of this type |
        |                       |                       | with the specified    |
        |                       |                       | name.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `values()`            | ::: block             |
        | static RemoteExecutio |                       | Returns an array      |
        | nActionEvent.State[]` |                       | containing the        |
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

        []{#WAITING}

        -   #### WAITING

                public static final RemoteExecutionActionEvent.State WAITING

        []{#COMPUTING_ACTION}

        -   #### COMPUTING_ACTION

                public static final RemoteExecutionActionEvent.State COMPUTING_ACTION

        []{#UPLOADING_INPUTS}

        -   #### UPLOADING_INPUTS

                public static final RemoteExecutionActionEvent.State UPLOADING_INPUTS

        []{#UPLOADING_ACTION}

        -   #### UPLOADING_ACTION

                public static final RemoteExecutionActionEvent.State UPLOADING_ACTION

        []{#EXECUTING}

        -   #### EXECUTING

                public static final RemoteExecutionActionEvent.State EXECUTING

        []{#DELETING_STALE_OUTPUTS}

        -   #### DELETING_STALE_OUTPUTS

                public static final RemoteExecutionActionEvent.State DELETING_STALE_OUTPUTS

        []{#MATERIALIZING_OUTPUTS}

        -   #### MATERIALIZING_OUTPUTS

                public static final RemoteExecutionActionEvent.State MATERIALIZING_OUTPUTS

        []{#ACTION_SUCCEEDED}

        -   #### ACTION_SUCCEEDED

                public static final RemoteExecutionActionEvent.State ACTION_SUCCEEDED

        []{#ACTION_FAILED}

        -   #### ACTION_FAILED

                public static final RemoteExecutionActionEvent.State ACTION_FAILED

        []{#ACTION_CANCELLED}

        -   #### ACTION_CANCELLED

                public static final RemoteExecutionActionEvent.State ACTION_CANCELLED
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#values()}

        -   #### values

            ``` methodSignature
            public static RemoteExecutionActionEvent.State[] values()
            ```

            ::: block
            Returns an array containing the constants of this enum type,
            in the order they are declared. This method may be used to
            iterate over the constants as follows:
                for (RemoteExecutionActionEvent.State c : RemoteExecutionActionEvent.State.values())
                    System.out.println(c);
            :::

            [Returns:]{.returnLabel}
            :   an array containing the constants of this enum type, in
                the order they are declared

        []{#valueOf(java.lang.String)}

        -   #### valueOf

            ``` methodSignature
            public static RemoteExecutionActionEvent.State valueOf​(String name)
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

        []{#getAbbreviateName()}

        -   #### getAbbreviateName

            ``` methodSignature
            public String getAbbreviateName()
            ```

            ::: block
            Abbreviated name for the current state.
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

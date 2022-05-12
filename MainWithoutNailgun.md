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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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

## Class MainWithoutNailgun {#class-mainwithoutnailgun .title title="Class MainWithoutNailgun"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cli.MainWithoutNailgun

::: description
-   

    ------------------------------------------------------------------------

        public class MainWithoutNailgun
        extends Object

    ::: block
    This is the main entry point for running buck without buckd.
    This main will take care of initializing all the state that buck
    needs given that the buck state is not stored. It will also take
    care of error handling and shutdown procedures given that we are not
    running as a nailgun server.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                                                   Field                 Description
          ------------------------------------------------------------------- --------------------- -------------
          `protected com.google.common.collect.ImmutableMap<String,​String>`   `clientEnvironment`    
          `protected Platform`                                                `platform`             
          `protected InputStream`                                             `stdIn`                

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor              Description
          ------------------------ -------------
          `MainWithoutNailgun()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `protected BuildId`   | `getBuildId()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protecte             | `getKno               |                       |
        | d MainRunner.KnownRul | wnRuleTypesFactory()` |                       |
        | eTypesFactoryFactory` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `main​(String[] args)` | ::: block             |
        |                       |                       | The entry point of a  |
        |                       |                       | buck command.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `prepareMainRu        |                       |
        | protected MainRunner` | nner​(BackgroundTaskMa |                       |
        |                       | nager bgTaskManager)` |                       |
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
    -   []{#field.detail}

        ### Field Detail

        []{#stdIn}

        -   #### stdIn

                protected final InputStream stdIn

        []{#clientEnvironment}

        -   #### clientEnvironment

                protected final com.google.common.collect.ImmutableMap<String,​String> clientEnvironment

        []{#platform}

        -   #### platform

                protected final Platform platform
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### MainWithoutNailgun

                public MainWithoutNailgun()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#main(java.lang.String[])}

        -   #### main

            ``` methodSignature
            public static void main​(String[] args)
            ```

            ::: block
            The entry point of a buck command.
            :::

            [Parameters:]{.paramLabel}
            :   `args` -

        []{#prepareMainRunner(com.facebook.buck.support.bgtasks.BackgroundTaskManager)}

        -   #### prepareMainRunner

            ``` methodSignature
            protected MainRunner prepareMainRunner​(BackgroundTaskManager bgTaskManager)
            ```

            [Returns:]{.returnLabel}
            :   an initialized
                [`MainRunner`](MainRunner.html "class in com.facebook.buck.cli")
                for running the buck command, with all the base state
                setup.

        []{#getKnownRuleTypesFactory()}

        -   #### getKnownRuleTypesFactory

            ``` methodSignature
            protected MainRunner.KnownRuleTypesFactoryFactory getKnownRuleTypesFactory()
            ```

            [Returns:]{.returnLabel}
            :   the
                [`MainRunner.KnownRuleTypesFactoryFactory`](MainRunner.KnownRuleTypesFactoryFactory.html "interface in com.facebook.buck.cli")
                for this command

        []{#getBuildId()}

        -   #### getBuildId

            ``` methodSignature
            protected BuildId getBuildId()
            ```

            [Returns:]{.returnLabel}
            :   the inferred
                [`BuildId`](../core/model/BuildId.html "class in com.facebook.buck.core.model")
                from the environment variable or create a new random
                [`BuildId`](../core/model/BuildId.html "class in com.facebook.buck.core.model")
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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

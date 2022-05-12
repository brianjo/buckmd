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

## Class MainWithNailgun {#class-mainwithnailgun .title title="Class MainWithNailgun"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cli.MainWithNailgun

::: description
-   

    ------------------------------------------------------------------------

        public class MainWithNailgun
        extends Object

    ::: block
    The Main entry point for Nailgun calls.
    This class maintains the state for statically storing daemon fields
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

          Constructor                                                   Description
          ------------------------------------------------------------- -------------
          `MainWithNailgun​(com.facebook.nailgun.NGContext ngContext)`    

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
        | `static void`         | `nailMai              | ::: block             |
        |                       | n​(com.facebook.nailgu | When running as a     |
        |                       | n.NGContext context)` | daemon in the NailGun |
        |                       |                       | server,               |
        |                       |                       | [`n                   |
        |                       |                       | ailMain(NGContext)`]( |
        |                       |                       | #nailMain(com.faceboo |
        |                       |                       | k.nailgun.NGContext)) |
        |                       |                       | is called instead of  |
        |                       |                       | [                     |
        |                       |                       | `MainRunner`](MainRun |
        |                       |                       | ner.html "class in co |
        |                       |                       | m.facebook.buck.cli") |
        |                       |                       | so that the given     |
        |                       |                       | context can be used   |
        |                       |                       | to listen for client  |
        |                       |                       | disconnections and    |
        |                       |                       | interrupt command     |
        |                       |                       | processing when they  |
        |                       |                       | occur.                |
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

        []{#<init>(com.facebook.nailgun.NGContext)}

        -   #### MainWithNailgun

                public MainWithNailgun​(com.facebook.nailgun.NGContext ngContext)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#nailMain(com.facebook.nailgun.NGContext)}

        -   #### nailMain

            ``` methodSignature
            public static void nailMain​(com.facebook.nailgun.NGContext context)
            ```

            ::: block
            When running as a daemon in the NailGun server,
            [`nailMain(NGContext)`](#nailMain(com.facebook.nailgun.NGContext))
            is called instead of
            [`MainRunner`](MainRunner.html "class in com.facebook.buck.cli")
            so that the given context can be used to listen for client
            disconnections and interrupt command processing when they
            occur.
            :::

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

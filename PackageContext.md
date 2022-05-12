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
[Package]{.packageLabelInType} [com.facebook.buck.skylark.packages](package-summary.html)
:::

## Class PackageContext {#class-packagecontext .title title="Class PackageContext"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.skylark.packages.PackageContext

::: description
-   

    ------------------------------------------------------------------------

        public abstract class PackageContext
        extends Object

    ::: block
    Exposes package information to Skylark functions.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor          Description
          -------------------- -------------
          `PackageContext()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `abstract com.goog    | `getEventHandler()`   |                       |
        | le.devtools.build.lib |                       |                       |
        | .events.EventHandler` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Globber`    | `getGlobber()`        | ::: block             |
        |                       |                       | Returns a globber     |
        |                       |                       | instance that can     |
        |                       |                       | resolve paths         |
        |                       |                       | relative to current   |
        |                       |                       | package.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getImpli             | ::: block             |
        | abstract com.google.c | citlyLoadedSymbols()` | Gets objects that     |
        | ommon.collect.Immutab |                       | were implciitly       |
        | leMap<String,​Object>` |                       | loaded                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ab                   | `ge                   | ::: block             |
        | stract com.google.dev | tPackageIdentifier()` | Returns a package     |
        | tools.build.lib.cmdli |                       | identifier of the     |
        | ne.PackageIdentifier` |                       | build file that is    |
        |                       |                       | being parsed.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstr                | `getRawConfig()`      | ::: block             |
        | act com.google.common |                       | Returns a raw map of  |
        | .collect.ImmutableMap |                       | configuration options |
        | <String,​com.google.co |                       | defined in            |
        | mmon.collect.Immutabl |                       | `.buckconfig` file    |
        | eMap<String,​String>>` |                       | and passed through a  |
        |                       |                       | `--config` command    |
        |                       |                       | line option.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `s                    | `of​(Globber glo       |                       |
        | tatic PackageContext` | bber,   Map<String,​?  |                       |
        |                       | extends com.google.co |                       |
        |                       | mmon.collect.Immutabl |                       |
        |                       | eMap<String,​String>>  |                       |
        |                       | rawConfig,   com.goog |                       |
        |                       | le.devtools.build.lib |                       |
        |                       | .cmdline.PackageIdent |                       |
        |                       | ifier packageIdentifi |                       |
        |                       | er,   com.google.devt |                       |
        |                       | ools.build.lib.events |                       |
        |                       | .EventHandler eventHa |                       |
        |                       | ndler,   Map<String,​? |                       |
        |                       |  extends Object> impl |                       |
        |                       | icitlyLoadedSymbols)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
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

        -   #### PackageContext

                public PackageContext()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getGlobber()}

        -   #### getGlobber

            ``` methodSignature
            public abstract Globber getGlobber()
            ```

            ::: block
            Returns a globber instance that can resolve paths relative
            to current package.
            :::

        []{#getRawConfig()}

        -   #### getRawConfig

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableMap<String,​com.google.common.collect.ImmutableMap<String,​String>> getRawConfig()
            ```

            ::: block
            Returns a raw map of configuration options defined in
            `.buckconfig` file and passed through a `--config` command
            line option.
            :::

        []{#getPackageIdentifier()}

        -   #### getPackageIdentifier

            ``` methodSignature
            public abstract com.google.devtools.build.lib.cmdline.PackageIdentifier getPackageIdentifier()
            ```

            ::: block
            Returns a package identifier of the build file that is being
            parsed.
            :::

        []{#getEventHandler()}

        -   #### getEventHandler

            ``` methodSignature
            public abstract com.google.devtools.build.lib.events.EventHandler getEventHandler()
            ```

            [Returns:]{.returnLabel}
            :   The event handler for reporting events during package
                parsing.

        []{#getImplicitlyLoadedSymbols()}

        -   #### getImplicitlyLoadedSymbols

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableMap<String,​Object> getImplicitlyLoadedSymbols()
            ```

            ::: block
            Gets objects that were implciitly loaded
            :::

        []{#of(com.facebook.buck.skylark.io.Globber,java.util.Map,com.google.devtools.build.lib.cmdline.PackageIdentifier,com.google.devtools.build.lib.events.EventHandler,java.util.Map)}

        -   #### of

            ``` methodSignature
            public static PackageContext of​(Globber globber,
                                            Map<String,​? extends com.google.common.collect.ImmutableMap<String,​String>> rawConfig,
                                            com.google.devtools.build.lib.cmdline.PackageIdentifier packageIdentifier,
                                            com.google.devtools.build.lib.events.EventHandler eventHandler,
                                            Map<String,​? extends Object> implicitlyLoadedSymbols)
            ```
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

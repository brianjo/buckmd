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
-   [Field](#field.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.core.plugin.impl](package-summary.html)
:::

## Class DefaultBuckPluginManager {#class-defaultbuckpluginmanager .title title="Class DefaultBuckPluginManager"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   org.pf4j.AbstractPluginManager

    -   -   org.pf4j.DefaultPluginManager

        -   -   com.facebook.buck.core.plugin.impl.DefaultBuckPluginManager

::: description
-   

    All Implemented Interfaces:
    :   `BuckPluginManager`, `org.pf4j.PluginManager`

    ------------------------------------------------------------------------

        public class DefaultBuckPluginManager
        extends org.pf4j.DefaultPluginManager
        implements BuckPluginManager
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.org.pf4j.DefaultPluginManager}

            ### Fields inherited from class org.pf4j.DefaultPluginManager

            `pluginClasspath`

        ```{=html}
        <!-- -->
        ```
        -   []{#fields.inherited.from.class.org.pf4j.AbstractPluginManager}

            ### Fields inherited from class org.pf4j.AbstractPluginManager

            `plugins`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                    Description
          ------------------------------ -------------
          `DefaultBuckPluginManager()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                     Method                             Description
          ----------------------------------------------------- ---------------------------------- -------------
          `protected org.pf4j.ExtensionFinder`                  `createExtensionFinder()`           
          `protected org.pf4j.CompoundPluginDescriptorFinder`   `createPluginDescriptorFinder()`    
          `protected org.pf4j.PluginLoader`                     `createPluginLoader()`              
          `protected org.pf4j.PluginRepository`                 `createPluginRepository()`          
          `protected org.pf4j.VersionManager`                   `createVersionManager()`            
          `<T> List<T>`                                         `getExtensions​(Class<T> type)`      

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.org.pf4j.DefaultPluginManager}

            ### Methods inherited from class org.pf4j.DefaultPluginManager

            `createExtensionFactory, createPluginClasspath, createPluginFactory, createPluginStatusProvider, initialize, loadPluginFromPath`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.org.pf4j.AbstractPluginManager}

            ### Methods inherited from class org.pf4j.AbstractPluginManager

            `addPluginStateListener, createPluginsRoot, deletePlugin, disablePlugin, enablePlugin, firePluginStateEvent, getExtensionClassNames, getExtensionFactory, getExtensions, getExtensions, getPlugin, getPluginClassLoader, getPluginClassLoaders, getPluginDescriptorFinder, getPluginFactory, getPluginLabel, getPluginLoader, getPlugins, getPlugins, getPluginsRoot, getResolvedPlugins, getRuntimeMode, getStartedPlugins, getSystemVersion, getUnresolvedPlugins, getVersion, getVersionManager, idForPath, isDevelopment, isExactVersionAllowed, isPluginDisabled, isPluginValid, loadPlugin, loadPlugins, removePluginStateListener, resolvePlugins, setExactVersionAllowed, setSystemVersion, startPlugin, startPlugins, stopPlugin, stopPlugins, unloadPlugin, validatePluginDescriptor, whichPlugin`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.org.pf4j.PluginManager}

            ### Methods inherited from interface org.pf4j.PluginManager

            `addPluginStateListener, deletePlugin, disablePlugin, enablePlugin, getExtensionClassNames, getExtensionFactory, getExtensions, getExtensions, getPlugin, getPluginClassLoader, getPlugins, getPlugins, getPluginsRoot, getResolvedPlugins, getRuntimeMode, getStartedPlugins, getSystemVersion, getUnresolvedPlugins, getVersionManager, loadPlugin, loadPlugins, removePluginStateListener, setSystemVersion, startPlugin, startPlugins, stopPlugin, stopPlugins, unloadPlugin, whichPlugin`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### DefaultBuckPluginManager

                public DefaultBuckPluginManager()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#createExtensionFinder()}

        -   #### createExtensionFinder

            ``` methodSignature
            protected org.pf4j.ExtensionFinder createExtensionFinder()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `createExtensionFinder` in
                class `org.pf4j.DefaultPluginManager`

        []{#createPluginDescriptorFinder()}

        -   #### createPluginDescriptorFinder

            ``` methodSignature
            protected org.pf4j.CompoundPluginDescriptorFinder createPluginDescriptorFinder()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `createPluginDescriptorFinder` in
                class `org.pf4j.DefaultPluginManager`

        []{#createPluginRepository()}

        -   #### createPluginRepository

            ``` methodSignature
            protected org.pf4j.PluginRepository createPluginRepository()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `createPluginRepository` in
                class `org.pf4j.DefaultPluginManager`

        []{#createPluginLoader()}

        -   #### createPluginLoader

            ``` methodSignature
            protected org.pf4j.PluginLoader createPluginLoader()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `createPluginLoader` in
                class `org.pf4j.DefaultPluginManager`

        []{#createVersionManager()}

        -   #### createVersionManager

            ``` methodSignature
            protected org.pf4j.VersionManager createVersionManager()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `createVersionManager` in
                class `org.pf4j.DefaultPluginManager`

        []{#getExtensions(java.lang.Class)}

        -   #### getExtensions

            ``` methodSignature
            public <T> List<T> getExtensions​(Class<T> type)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExtensions` in interface `org.pf4j.PluginManager`

            [Overrides:]{.overrideSpecifyLabel}
            :   `getExtensions` in
                class `org.pf4j.AbstractPluginManager`
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
-   [Field](#field.summary) \| 
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

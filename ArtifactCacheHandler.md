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
-   [Nested](#nested.class.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.httpserver](package-summary.html)
:::

## Class ArtifactCacheHandler {#class-artifactcachehandler .title title="Class ArtifactCacheHandler"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   org.eclipse.jetty.util.component.AbstractLifeCycle

    -   -   org.eclipse.jetty.util.component.ContainerLifeCycle

        -   -   org.eclipse.jetty.server.handler.AbstractHandler

            -   -   com.facebook.buck.httpserver.ArtifactCacheHandler

::: description
-   

    All Implemented Interfaces:
    :   `org.eclipse.jetty.server.Handler`,
        `org.eclipse.jetty.util.component.Container`,
        `org.eclipse.jetty.util.component.Destroyable`,
        `org.eclipse.jetty.util.component.Dumpable`,
        `org.eclipse.jetty.util.component.LifeCycle`

    ------------------------------------------------------------------------

        public class ArtifactCacheHandler
        extends org.eclipse.jetty.server.handler.AbstractHandler

    ::: block
    Implements a really simple cache server on top of the local
    dircache.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.org.eclipse.jetty.server.handler.AbstractHandler}

            ### Nested classes/interfaces inherited from class org.eclipse.jetty.server.handler.AbstractHandler

            `org.eclipse.jetty.server.handler.AbstractHandler.ErrorDispatchHandler`

        ```{=html}
        <!-- -->
        ```
        -   []{#nested.classes.inherited.from.class.org.eclipse.jetty.util.component.AbstractLifeCycle}

            ### Nested classes/interfaces inherited from class org.eclipse.jetty.util.component.AbstractLifeCycle

            `org.eclipse.jetty.util.component.AbstractLifeCycle.AbstractLifeCycleListener`

        ```{=html}
        <!-- -->
        ```
        -   []{#nested.classes.inherited.from.class.org.eclipse.jetty.util.component.Container}

            ### Nested classes/interfaces inherited from interface org.eclipse.jetty.util.component.Container

            `org.eclipse.jetty.util.component.Container.InheritedListener, org.eclipse.jetty.util.component.Container.Listener`

        ```{=html}
        <!-- -->
        ```
        -   []{#nested.classes.inherited.from.class.org.eclipse.jetty.util.component.LifeCycle}

            ### Nested classes/interfaces inherited from interface org.eclipse.jetty.util.component.LifeCycle

            `org.eclipse.jetty.util.component.LifeCycle.Listener`
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.org.eclipse.jetty.util.component.AbstractLifeCycle}

            ### Fields inherited from class org.eclipse.jetty.util.component.AbstractLifeCycle

            `FAILED, RUNNING, STARTED, STARTING, STOP_ON_FAILURE, STOPPED, STOPPING`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                   Description
          ------------------------------------------------------------- -------------
          `ArtifactCacheHandler​(ProjectFilesystem projectFilesystem)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                                                                                                                    Description
          ------------------- ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `void`              `handle​(String target,       org.eclipse.jetty.server.Request baseRequest,       javax.servlet.http.HttpServletRequest request,       javax.servlet.http.HttpServletResponse response)`    
          `void`              `setArtifactCache​(Optional<ArtifactCache> artifactCache)`                                                                                                                                  

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.org.eclipse.jetty.server.handler.AbstractHandler}

            ### Methods inherited from class org.eclipse.jetty.server.handler.AbstractHandler

            `destroy, doError, doStart, doStop, dumpThis, getServer, setServer`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.org.eclipse.jetty.util.component.ContainerLifeCycle}

            ### Methods inherited from class org.eclipse.jetty.util.component.ContainerLifeCycle

            `addBean, addBean, addBean, addEventListener, addManaged, contains, dump, dump, dump, dump, dump, dumpBeans, dumpObject, dumpStdErr, getBean, getBeans, getBeans, getContainedBeans, getContainedBeans, isManaged, manage, removeBean, removeBeans, removeEventListener, setBeans, setStopTimeout, start, stop, unmanage, updateBean, updateBean, updateBeans`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.org.eclipse.jetty.util.component.AbstractLifeCycle}

            ### Methods inherited from class org.eclipse.jetty.util.component.AbstractLifeCycle

            `addLifeCycleListener, getState, getState, getStopTimeout, isFailed, isRunning, isStarted, isStarting, isStopped, isStopping, removeLifeCycleListener, start, stop`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.org.eclipse.jetty.util.component.LifeCycle}

            ### Methods inherited from interface org.eclipse.jetty.util.component.LifeCycle

            `addLifeCycleListener, isFailed, isRunning, isStarted, isStarting, isStopped, isStopping, removeLifeCycleListener, start, stop`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### ArtifactCacheHandler

                public ArtifactCacheHandler​(ProjectFilesystem projectFilesystem)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#setArtifactCache(java.util.Optional)}

        -   #### setArtifactCache

            ``` methodSignature
            public void setArtifactCache​(Optional<ArtifactCache> artifactCache)
            ```

        []{#handle(java.lang.String,org.eclipse.jetty.server.Request,javax.servlet.http.HttpServletRequest,javax.servlet.http.HttpServletResponse)}

        -   #### handle

            ``` methodSignature
            public void handle​(String target,
                               org.eclipse.jetty.server.Request baseRequest,
                               javax.servlet.http.HttpServletRequest request,
                               javax.servlet.http.HttpServletResponse response)
                        throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `handle` in interface `org.eclipse.jetty.server.Handler`

            [Specified by:]{.overrideSpecifyLabel}
            :   `handle` in
                class `org.eclipse.jetty.server.handler.AbstractHandler`

            [Throws:]{.throwsLabel}
            :   `IOException`
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
-   [Nested](#nested.class.summary) \| 
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

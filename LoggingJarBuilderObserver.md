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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java](package-summary.html)
:::

## Class LoggingJarBuilderObserver {#class-loggingjarbuilderobserver .title title="Class LoggingJarBuilderObserver"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.LoggingJarBuilderObserver

::: description
-   

    All Implemented Interfaces:
    :   `JarBuilder.Observer`

    ------------------------------------------------------------------------

        public class LoggingJarBuilderObserver
        extends Object
        implements JarBuilder.Observer
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.util.zip.JarBuilder.Observer}

            ### Fields inherited from interface com.facebook.buck.util.zip.[JarBuilder.Observer](../../util/zip/JarBuilder.Observer.html "interface in com.facebook.buck.util.zip")

            `IGNORING`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                Description
          ---------------------------------------------------------------------------------------------------------- -------------
          `LoggingJarBuilderObserver​(JavacEventSink eventSink)`                                                       
          `LoggingJarBuilderObserver​(JavacEventSink eventSink,                          Level duplicatesLogLevel)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                               Description
          ------------------- ------------------------------------------------------------------------------------ -------------
          `void`              `onDuplicateEntry​(String jarFile,                 JarEntrySupplier entrySupplier)`    
          `void`              `onEntryOmitted​(String jarFile,               JarEntrySupplier entrySupplier)`        

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.jvm.java.JavacEventSink)}

        -   #### LoggingJarBuilderObserver

                public LoggingJarBuilderObserver​(JavacEventSink eventSink)

        []{#<init>(com.facebook.buck.jvm.java.JavacEventSink,java.util.logging.Level)}

        -   #### LoggingJarBuilderObserver

                public LoggingJarBuilderObserver​(JavacEventSink eventSink,
                                                 Level duplicatesLogLevel)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#onDuplicateEntry(java.lang.String,com.facebook.buck.util.zip.JarEntrySupplier)}

        -   #### onDuplicateEntry

            ``` methodSignature
            public void onDuplicateEntry​(String jarFile,
                                         JarEntrySupplier entrySupplier)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `onDuplicateEntry` in interface `JarBuilder.Observer`

        []{#onEntryOmitted(java.lang.String,com.facebook.buck.util.zip.JarEntrySupplier)}

        -   #### onEntryOmitted

            ``` methodSignature
            public void onEntryOmitted​(String jarFile,
                                       JarEntrySupplier entrySupplier)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `onEntryOmitted` in interface `JarBuilder.Observer`
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

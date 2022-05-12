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
[Package]{.packageLabelInType} [com.facebook.buck.skylark.io.impl](package-summary.html)
:::

## Class HybridGlobber {#class-hybridglobber .title title="Class HybridGlobber"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.skylark.io.impl.HybridGlobber

::: description
-   

    All Implemented Interfaces:
    :   `Globber`

    ------------------------------------------------------------------------

        public class HybridGlobber
        extends Object
        implements Globber

    ::: block
    A
    [`Globber`](../Globber.html "interface in com.facebook.buck.skylark.io")
    implementation that tries to use Watchman if it\'s available and
    falls back to a fallback globber, in case Watchman query cannot be
    fulfilled.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                              Description
          ---------------------------------------------------------------------------------------- -------------
          `HybridGlobber​(Globber fallbackGlobber,              WatchmanGlobber watchmanGlobber)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                            Description
          ------------------- ------------------------------------------------------------------------------------------------- -------------
          `Set<String>`       `run​(Collection<String> include,    Collection<String> exclude,    boolean excludeDirectories)`    

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

        []{#<init>(com.facebook.buck.skylark.io.Globber,com.facebook.buck.skylark.io.impl.WatchmanGlobber)}

        -   #### HybridGlobber

                public HybridGlobber​(Globber fallbackGlobber,
                                     WatchmanGlobber watchmanGlobber)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#run(java.util.Collection,java.util.Collection,boolean)}

        -   #### run

            ``` methodSignature
            public Set<String> run​(Collection<String> include,
                                   Collection<String> exclude,
                                   boolean excludeDirectories)
                            throws IOException,
                                   InterruptedException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `run` in interface `Globber`

            [Throws:]{.throwsLabel}
            :   `IOException`
            :   `InterruptedException`
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

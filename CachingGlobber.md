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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
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

## Class CachingGlobber {#class-cachingglobber .title title="Class CachingGlobber"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.skylark.io.impl.CachingGlobber

::: description
-   

    All Implemented Interfaces:
    :   `Globber`

    ------------------------------------------------------------------------

        @NotThreadSafe
        public class CachingGlobber
        extends Object
        implements Globber

    ::: block
    [`Globber`](../Globber.html "interface in com.facebook.buck.skylark.io")
    implementation that caches expanded paths from previous invocations
    and reuses them in case the glob with same
    [`GlobSpec`](../GlobSpec.html "class in com.facebook.buck.skylark.io")
    is requested again.
    Most of the packages usually do not perform identical glob
    invocations, but when complex macros are used, it\'s not uncommon to
    see repeated invocations of the same `glob` function.

    There is a more important reason to use consistent glob resolution
    while parsing the same package - caching. This approach guarantees
    that all `glob` invocations are expanded in the exact same way and
    as such all execution paths that rely on glob results will be
    consistent as well. In other words, the snippet: ``

           if glob(['foo']):
             print("A")
           else:
             print("B")
           if glob(['foo']):
             print("C")
           else:
             print("D")
         

    will always produce either `"AC"` or `"CD"` and never `"AD"` or
    `"BC"`.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                               Method                                                                                            Description
          --------------------------------------------------------------- ------------------------------------------------------------------------------------------------- -------------
          `com.google.common.collect.ImmutableList<GlobSpecWithResult>`   `createGlobManifest()`                                                                             
          `static CachingGlobber`                                         `of​(Globber globber)`                                                                              
          `Set<String>`                                                   `run​(Collection<String> include,    Collection<String> exclude,    boolean excludeDirectories)`    

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

        []{#createGlobManifest()}

        -   #### createGlobManifest

            ``` methodSignature
            public com.google.common.collect.ImmutableList<GlobSpecWithResult> createGlobManifest()
            ```

            [Returns:]{.returnLabel}
            :   Glob manifest that includes information about expanded
                paths for each requested
                [`GlobSpec`](../GlobSpec.html "class in com.facebook.buck.skylark.io").

        []{#of(com.facebook.buck.skylark.io.Globber)}

        -   #### of

            ``` methodSignature
            public static CachingGlobber of​(Globber globber)
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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

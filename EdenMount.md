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
[Package]{.packageLabelInType} [com.facebook.buck.edenfs](package-summary.html)
:::

## Class EdenMount {#class-edenmount .title title="Class EdenMount"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.edenfs.EdenMount

::: description
-   

    ------------------------------------------------------------------------

        public class EdenMount
        extends Object

    ::: block
    Utility to make requests to the Eden thrift API for an (Eden mount
    point, Buck project root) pair. The Buck project root must be
    contained by the Eden mount point.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type              Method                                                                                                Description
          ------------------------------ ----------------------------------------------------------------------------------------------------- -------------
          `static Optional<EdenMount>`   `createEdenMountForProjectRoot​(Path projectRoot,                              EdenClientPool pool)`    
          `Path`                         `getProjectRoot()`                                                                                     
          `Sha1HashCode`                 `getSha1​(Path entry)`                                                                                  
          `String`                       `toString()`                                                                                           

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#createEdenMountForProjectRoot(java.nio.file.Path,com.facebook.buck.edenfs.EdenClientPool)}

        -   #### createEdenMountForProjectRoot

            ``` methodSignature
            public static Optional<EdenMount> createEdenMountForProjectRoot​(Path projectRoot,
                                                                            EdenClientPool pool)
            ```

            [Returns:]{.returnLabel}
            :   an Eden mount point if `projectRoot` is backed by Eden
                or `null`.

        []{#getProjectRoot()}

        -   #### getProjectRoot

            ``` methodSignature
            public Path getProjectRoot()
            ```

            [Returns:]{.returnLabel}
            :   The root to the Buck project that this
                [`EdenMount`](EdenMount.html "class in com.facebook.buck.edenfs")
                represents.

        []{#getSha1(java.nio.file.Path)}

        -   #### getSha1

            ``` methodSignature
            public Sha1HashCode getSha1​(Path entry)
                                 throws com.facebook.eden.thrift.EdenError,
                                        IOException,
                                        com.facebook.thrift.TException
            ```

            [Parameters:]{.paramLabel}
            :   `entry` - is a path that is relative to
                [`getProjectRoot()`](#getProjectRoot()).

            [Throws:]{.throwsLabel}
            :   `com.facebook.eden.thrift.EdenError`
            :   `IOException`
            :   `com.facebook.thrift.TException`

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`
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

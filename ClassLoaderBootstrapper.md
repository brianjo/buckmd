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
[Package]{.packageLabelInType} [com.facebook.buck.cli.bootstrapper](package-summary.html)
:::

## Class ClassLoaderBootstrapper {#class-classloaderbootstrapper .title title="Class ClassLoaderBootstrapper"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cli.bootstrapper.ClassLoaderBootstrapper

::: description
-   

    ------------------------------------------------------------------------

        public final class ClassLoaderBootstrapper
        extends Object

    ::: block
    This class sets up a separate ClassLoader for most of Buck\'s
    implementation, leaving only the bare minimum bootstrapping classes
    (and a few classes for compatibility with library code that is not
    ClassLoader-aware) in the system ClassLoader. This is done so that
    annotation processors do not have their classpaths polluted with
    Buck\'s dependencies when Buck is compiling Java code in-process.
    Under JSR-199, when the Java compiler is run in-process it uses a
    ClassLoader that is a child of the system ClassLoader. In order for
    annotation processors to access the Compiler Tree API (which lives
    in tools.jar with the compiler itself), they must be loaded with a
    ClassLoader descended from the compiler\'s. If Buck used the system
    ClassLoader as a normal Java application would, this would result in
    annotation processors getting Buck\'s versions of Guava, Jackson,
    etc. instead of their own.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                     Description
          ------------------- -------------------------- -------------
          `static Class<?>`   `loadClass​(String name)`    
          `static void`       `main​(String[] args)`       

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
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

        []{#main(java.lang.String[])}

        -   #### main

            ``` methodSignature
            public static void main​(String[] args)
                             throws Exception
            ```

            [Throws:]{.throwsLabel}
            :   `Exception`

        []{#loadClass(java.lang.String)}

        -   #### loadClass

            ``` methodSignature
            public static Class<?> loadClass​(String name)
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
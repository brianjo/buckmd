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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java](package-summary.html)
:::

## Class JavaLibraryClasspathProvider {#class-javalibraryclasspathprovider .title title="Class JavaLibraryClasspathProvider"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.JavaLibraryClasspathProvider

::: description
-   

    ------------------------------------------------------------------------

        public class JavaLibraryClasspathProvider
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static com.google    | `get                  | ::: block             |
        | .common.collect.Immut | AllReachableJavaLibra | Return the classpath, |
        | ableSet<JavaLibrary>` | ries​(Iterable<? exten | including traversing  |
        |                       | ds BuildRule> rules)` | any provided_deps     |
        |                       |                       | edges and non-java    |
        |                       |                       | edges                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static com.google    | `g                    | ::: block             |
        | .common.collect.Immut | etClasspathDeps​(Itera | Include the classpath |
        | ableSet<JavaLibrary>` | ble<BuildRule> deps)` | entries from all      |
        |                       |                       | JavaLibraryRules that |
        |                       |                       | have a direct line of |
        |                       |                       | lineage to this rule  |
        |                       |                       | through other         |
        |                       |                       | JavaLibraryRules.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static com.googl     | `getClasspathsFromL   | ::: block             |
        | e.common.collect.Immu | ibraries​(Iterable<Jav | Given libraries that  |
        | tableSet<SourcePath>` | aLibrary> libraries)` | may contribute        |
        |                       |                       | classpaths, visit     |
        |                       |                       | them and collect the  |
        |                       |                       | classpaths.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static com.googl     | `g                    |                       |
        | e.common.collect.Immu | etOutputClasspathJars |                       |
        | tableSet<SourcePath>` | ​(JavaLibrary javaLibr |                       |
        |                       | aryRule,              |                       |
        |                       |           Optional<So |                       |
        |                       | urcePath> outputJar)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static com.google    | `getTransit           |                       |
        | .common.collect.Immut | iveClasspathDeps​(Java |                       |
        | ableSet<JavaLibrary>` | Library javaLibrary)` |                       |
        +-----------------------+-----------------------+-----------------------+

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

        []{#getOutputClasspathJars(com.facebook.buck.jvm.core.JavaLibrary,java.util.Optional)}

        -   #### getOutputClasspathJars

            ``` methodSignature
            public static com.google.common.collect.ImmutableSet<SourcePath> getOutputClasspathJars​(JavaLibrary javaLibraryRule,
                                                                                                    Optional<SourcePath> outputJar)
            ```

        []{#getTransitiveClasspathDeps(com.facebook.buck.jvm.core.JavaLibrary)}

        -   #### getTransitiveClasspathDeps

            ``` methodSignature
            public static com.google.common.collect.ImmutableSet<JavaLibrary> getTransitiveClasspathDeps​(JavaLibrary javaLibrary)
            ```

        []{#getClasspathDeps(java.lang.Iterable)}

        -   #### getClasspathDeps

            ``` methodSignature
            public static com.google.common.collect.ImmutableSet<JavaLibrary> getClasspathDeps​(Iterable<BuildRule> deps)
            ```

            ::: block
            Include the classpath entries from all JavaLibraryRules that
            have a direct line of lineage to this rule through other
            JavaLibraryRules. For example, in the following dependency
            graph:
                        A
                      /   \
                     B     C
                    / \   / \
                    D E   F G

                 

            If all of the nodes correspond to BuildRules that implement
            JavaLibraryRule except for B (suppose B is a Genrule), then
            A\'s classpath will include C, F, and G, but not D and E.
            This is because D and E are used to generate B, but do not
            contribute .class files to things that depend on B. However,
            if C depended on E as well as F and G, then E would be
            included in A\'s classpath.
            :::

        []{#getClasspathsFromLibraries(java.lang.Iterable)}

        -   #### getClasspathsFromLibraries

            ``` methodSignature
            public static com.google.common.collect.ImmutableSet<SourcePath> getClasspathsFromLibraries​(Iterable<JavaLibrary> libraries)
            ```

            ::: block
            Given libraries that may contribute classpaths, visit them
            and collect the classpaths.
            This is used to generate transitive classpaths from library
            discovered in a previous traversal.
            :::

        []{#getAllReachableJavaLibraries(java.lang.Iterable)}

        -   #### getAllReachableJavaLibraries

            ``` methodSignature
            public static com.google.common.collect.ImmutableSet<JavaLibrary> getAllReachableJavaLibraries​(Iterable<? extends BuildRule> rules)
            ```

            ::: block
            Return the classpath, including traversing any provided_deps
            edges and non-java edges
            :::
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

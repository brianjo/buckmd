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
[Package]{.packageLabelInType} [com.facebook.buck.io.file](package-summary.html)
:::

## Class FileFinder {#class-filefinder .title title="Class FileFinder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.io.file.FileFinder

::: description
-   

    ------------------------------------------------------------------------

        public class FileFinder
        extends Object

    ::: block
    Methods for finding files.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static com.g         | `combine​(Set<Stri     | ::: block             |
        | oogle.common.collect. | ng> prefixes,         | Combines prefixes,    |
        | ImmutableSet<String>` | String base,        S | base, and suffixes to |
        |                       | et<String> suffixes)` | create a set of file  |
        |                       |                       | names.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `s                    | `getOptionalFile​(Se   | ::: block             |
        | tatic Optional<Path>` | t<String> possibleNam | Tries to find a file  |
        |                       | es,                It | with one of a number  |
        |                       | erable<Path> searchPa | of possible names in  |
        |                       | ths,                j | a search path.        |
        |                       | ava.util.function.Pre | :::                   |
        |                       | dicate<Path> filter)` |                       |
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

        []{#combine(java.util.Set,java.lang.String,java.util.Set)}

        -   #### combine

            ``` methodSignature
            public static com.google.common.collect.ImmutableSet<String> combine​(Set<String> prefixes,
                                                                                 String base,
                                                                                 Set<String> suffixes)
            ```

            ::: block
            Combines prefixes, base, and suffixes to create a set of
            file names.
            :::

            [Parameters:]{.paramLabel}
            :   `prefixes` - set of prefixes. May be empty.
            :   `base` - base name. May be empty.
            :   `suffixes` - set of suffixes. May be empty.

            [Returns:]{.returnLabel}
            :   a set containing all combinations of prefix, base, and
                suffix.

        []{#getOptionalFile(java.util.Set,java.lang.Iterable,java.util.function.Predicate)}

        -   #### getOptionalFile

            ``` methodSignature
            public static Optional<Path> getOptionalFile​(Set<String> possibleNames,
                                                         Iterable<Path> searchPaths,
                                                         java.util.function.Predicate<Path> filter)
            ```

            ::: block
            Tries to find a file with one of a number of possible names
            in a search path.
            Returns the first match found. Search tries all paths in the
            search paths in order, looking for any matching names in
            each path.
            :::

            [Parameters:]{.paramLabel}
            :   `possibleNames` - file names to look for.
            :   `searchPaths` - directories to search.
            :   `filter` - additional check that discovered paths must
                pass to be eligible.

            [Returns:]{.returnLabel}
            :   returns the first match found, if any.
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

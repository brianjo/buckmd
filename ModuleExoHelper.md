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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.android.exopackage](package-summary.html)
:::

## Class ModuleExoHelper {#class-moduleexohelper .title title="Class ModuleExoHelper"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.exopackage.ModuleExoHelper

::: description
-   

    ------------------------------------------------------------------------

        public class ModuleExoHelper
        extends Object

    ::: block
    An ExoHelper which provides a mapping of host source path to device
    install path for modular dex files when exopackage-for-modules is
    enabled
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field               Description
          ------------------- ------------------- -------------
          `static Path`       `MODULAR_DEX_DIR`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                       Method                     Description
          ------------------------------------------------------- -------------------------- -------------
          `com.google.common.collect.ImmutableMap<Path,​Path>`     `getFilesToInstall()`       
          `com.google.common.collect.ImmutableMap<Path,​String>`   `getMetadataToInstall()`    

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
    -   []{#field.detail}

        ### Field Detail

        []{#MODULAR_DEX_DIR}

        -   #### MODULAR_DEX_DIR

                public static final Path MODULAR_DEX_DIR
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getFilesToInstall()}

        -   #### getFilesToInstall

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<Path,​Path> getFilesToInstall()
                                                                                      throws IOException
            ```

            [Returns:]{.returnLabel}
            :   the list of modular dex files which are installable for
                this build The returned map contains entries of the form
                destination_file_path =\> local_src_file_path

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getMetadataToInstall()}

        -   #### getMetadataToInstall

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<Path,​String> getMetadataToInstall()
                                                                                           throws IOException
            ```

            [Returns:]{.returnLabel}

            :   metadata contents for each module, containing hashes and
                canary class names along with a top level metadata file
                describing the full set of modular jars. The per-module
                metadata files contain comment lines beginning with a
                \'.\' and entry lines which each describe a jar
                belonging to the module with the format: \"file_path
                file_hash\"

                The top level metadata file has one line per jar with
                the following format: \"file_name module_name\" and
                provides a top-level listing of all jars included in the
                build along with a mapping back to the module name where
                they came from

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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

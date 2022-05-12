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
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.io.filesystem.impl](package-summary.html)
:::

## Class DefaultProjectFilesystemFactory {#class-defaultprojectfilesystemfactory .title title="Class DefaultProjectFilesystemFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.io.filesystem.impl.DefaultProjectFilesystemFactory

::: description
-   

    All Implemented Interfaces:
    :   `ProjectFilesystemFactory`

    ------------------------------------------------------------------------

        public class DefaultProjectFilesystemFactory
        extends Object
        implements ProjectFilesystemFactory
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                  Description
          ------------------- ---------------------- -------------
          `static String`     `BUCK_BUCKD_DIR_KEY`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                           Description
          ------------------------------------- -------------
          `DefaultProjectFilesystemFactory()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type            Method                                                                                                                                                                                                                                                                              Description
          ---------------------------- ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `DefaultProjectFilesystem`   `createOrThrow​(CanonicalCellName cellName,              AbsPath path,              boolean buckOutIncludeTargetCofigHash)`                                                                                                                                                           
          `DefaultProjectFilesystem`   `createProjectFilesystem​(CanonicalCellName cellName,                        AbsPath root,                        boolean buckOutIncludeTargetCofigHash)`                                                                                                                             
          `DefaultProjectFilesystem`   `createProjectFilesystem​(CanonicalCellName cellName,                        AbsPath root,                        Config config,                        boolean buckOutIncludeTargetConfigHash)`                                                                                      
          `DefaultProjectFilesystem`   `createProjectFilesystem​(CanonicalCellName cellName,                        AbsPath root,                        Config config,                        Optional<EmbeddedCellBuckOutInfo> embeddedCellBuckOutInfo,                        boolean buckOutIncludeTargetConfigHash)`    
          `static WindowsFS`           `getWindowsFSInstance()`                                                                                                                                                                                                                                                             

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
    -   []{#field.detail}

        ### Field Detail

        []{#BUCK_BUCKD_DIR_KEY}

        -   #### BUCK_BUCKD_DIR_KEY

                public static final String BUCK_BUCKD_DIR_KEY

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.io.filesystem.impl.DefaultProjectFilesystemFactory.BUCK_BUCKD_DIR_KEY)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### DefaultProjectFilesystemFactory

                public DefaultProjectFilesystemFactory()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getWindowsFSInstance()}

        -   #### getWindowsFSInstance

            ``` methodSignature
            @Nullable
            public static WindowsFS getWindowsFSInstance()
            ```

            [Returns:]{.returnLabel}
            :   the WindowsFS singleton.

        []{#createProjectFilesystem(com.facebook.buck.core.cell.name.CanonicalCellName,com.facebook.buck.core.filesystems.AbsPath,com.facebook.buck.util.config.Config,java.util.Optional,boolean)}

        -   #### createProjectFilesystem

            ``` methodSignature
            public DefaultProjectFilesystem createProjectFilesystem​(CanonicalCellName cellName,
                                                                    AbsPath root,
                                                                    Config config,
                                                                    Optional<EmbeddedCellBuckOutInfo> embeddedCellBuckOutInfo,
                                                                    boolean buckOutIncludeTargetConfigHash)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `createProjectFilesystem` in
                interface `ProjectFilesystemFactory`

        []{#createProjectFilesystem(com.facebook.buck.core.cell.name.CanonicalCellName,com.facebook.buck.core.filesystems.AbsPath,com.facebook.buck.util.config.Config,boolean)}

        -   #### createProjectFilesystem

            ``` methodSignature
            public DefaultProjectFilesystem createProjectFilesystem​(CanonicalCellName cellName,
                                                                    AbsPath root,
                                                                    Config config,
                                                                    boolean buckOutIncludeTargetConfigHash)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `createProjectFilesystem` in
                interface `ProjectFilesystemFactory`

        []{#createProjectFilesystem(com.facebook.buck.core.cell.name.CanonicalCellName,com.facebook.buck.core.filesystems.AbsPath,boolean)}

        -   #### createProjectFilesystem

            ``` methodSignature
            public DefaultProjectFilesystem createProjectFilesystem​(CanonicalCellName cellName,
                                                                    AbsPath root,
                                                                    boolean buckOutIncludeTargetCofigHash)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `createProjectFilesystem` in
                interface `ProjectFilesystemFactory`

        []{#createOrThrow(com.facebook.buck.core.cell.name.CanonicalCellName,com.facebook.buck.core.filesystems.AbsPath,boolean)}

        -   #### createOrThrow

            ``` methodSignature
            public DefaultProjectFilesystem createOrThrow​(CanonicalCellName cellName,
                                                          AbsPath path,
                                                          boolean buckOutIncludeTargetCofigHash)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `createOrThrow` in interface `ProjectFilesystemFactory`
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
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

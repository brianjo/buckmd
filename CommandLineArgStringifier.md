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

-   [Overview](../../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../../index-all.html)
-   [Help](../../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.actions.lib.args](package-summary.html)
:::

## Class CommandLineArgStringifier {#class-commandlineargstringifier .title title="Class CommandLineArgStringifier"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.rules.actions.lib.args.CommandLineArgStringifier

::: description
-   

    ------------------------------------------------------------------------

        public class CommandLineArgStringifier
        extends Object

    ::: block
    Helper methods to convert / validate objects that are command line
    arguments for actions
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                                                               Description
          ------------------- ------------------------------------------------------------------------------------------------------------------------------------ -------------
          `static String`     `asString​(ArtifactFilesystem filesystem,         boolean absolute,         CommandLineArgs.ArgAndFormatString argAndFormatString)`    
          `static String`     `asString​(ArtifactFilesystem filesystem,         boolean absolute,         Object object)`                                            

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

        []{#asString(com.facebook.buck.core.artifact.ArtifactFilesystem,boolean,com.facebook.buck.core.rules.actions.lib.args.CommandLineArgs.ArgAndFormatString)}

        -   #### asString

            ``` methodSignature
            public static String asString​(ArtifactFilesystem filesystem,
                                          boolean absolute,
                                          CommandLineArgs.ArgAndFormatString argAndFormatString)
            ```

            [Parameters:]{.paramLabel}
            :   `filesystem` - the filesystem to use to stringify
                [`Artifact`](../../../../artifact/Artifact.html "interface in com.facebook.buck.core.artifact")s
            :   `absolute` - If the path returned should be absolute.
                This can be necessary for functions like
                [`ProcessBuilder.start()`](http://docs.oracle.com/javase/7/docs/api/java/lang/ProcessBuilder.html?is-external=true#start() "class or interface in java.lang"){.externalLink}.
                On windows it does not do path resolution properly for
                relative paths, even if the `directory` is set so an
                absolute path must be provided.
            :   `argAndFormatString` - the object to stringify and the
                format string to apply after initial stringification

            [Returns:]{.returnLabel}
            :   the string representation of an argument to pass to a
                command line application in an action

        []{#asString(com.facebook.buck.core.artifact.ArtifactFilesystem,boolean,java.lang.Object)}

        -   #### asString

            ``` methodSignature
            public static String asString​(ArtifactFilesystem filesystem,
                                          boolean absolute,
                                          Object object)
                                   throws CommandLineArgException
            ```

            [Parameters:]{.paramLabel}
            :   `filesystem` - the filesystem to use to stringify
                [`Artifact`](../../../../artifact/Artifact.html "interface in com.facebook.buck.core.artifact")s
            :   `absolute` - If the path returned should be absolute.
                This can be necessary for functions like
                [`ProcessBuilder.start()`](http://docs.oracle.com/javase/7/docs/api/java/lang/ProcessBuilder.html?is-external=true#start() "class or interface in java.lang"){.externalLink}.
                On windows it does not do path resolution properly for
                relative paths, even if the `directory` is set so an
                absolute path must be provided.
            :   `object` - the object to stringify

            [Returns:]{.returnLabel}
            :   the string representation of an argument to pass to a
                command line application in an action

            [Throws:]{.throwsLabel}
            :   `CommandLineArgException`
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

-   [Overview](../../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../../index-all.html)
-   [Help](../../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../../allclasses.html)

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

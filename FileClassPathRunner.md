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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java.runner](package-summary.html)
:::

## Class FileClassPathRunner {#class-fileclasspathrunner .title title="Class FileClassPathRunner"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.runner.FileClassPathRunner

::: description
-   

    ------------------------------------------------------------------------

        public class FileClassPathRunner
        extends Object

    ::: block
    This class handles extra large classpaths by allowing the client to
    pass the classpath via file specified by `buck.classpath_file`. This
    is to sidestep commandline length limits.
    There are 3 modes:

    -   Java 8 or older launched: We manually add the entries from
        \`buck.classpath_file\` to the system classloader.
    -   Java 9 or newer launched, and Buck is aware of this: We rely on
        \`@argfile\` support in newer versions of \`java\` to pass in
        our long \`-classpath\` argument. Here, the JVM adds all the
        classpath entries itself.
    -   Java 9 or newer launched, and Buck isn\'t aware of this: We
        create a new classloader and add entries from
        \`buck.classpath_file\` manually. This approach has problems,
        e.g. classloading for in-process Java compilation does not work
        for Buck\'s own tests, but is provided to support cases where
        the version of \`java\` on the path is 9+, but we\'re targeting
        8- for the target under test.

    Note: this class only depends on classes present in the JRE, since
    we don\'t want to have to push more things on to the classpath when
    using it.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                           Description
          ------------------- ------------------------------- -------------
          `static String`     `CLASSPATH_FILE_PROPERTY`        
          `static String`     `TESTRUNNER_CLASSES_PROPERTY`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                  Description
          ------------------- ----------------------- -------------
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
    -   []{#field.detail}

        ### Field Detail

        []{#CLASSPATH_FILE_PROPERTY}

        -   #### CLASSPATH_FILE_PROPERTY

                public static final String CLASSPATH_FILE_PROPERTY

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.jvm.java.runner.FileClassPathRunner.CLASSPATH_FILE_PROPERTY)

        []{#TESTRUNNER_CLASSES_PROPERTY}

        -   #### TESTRUNNER_CLASSES_PROPERTY

                public static final String TESTRUNNER_CLASSES_PROPERTY

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.jvm.java.runner.FileClassPathRunner.TESTRUNNER_CLASSES_PROPERTY)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#main(java.lang.String[])}

        -   #### main

            ``` methodSignature
            public static void main​(String[] args)
                             throws IOException,
                                    ReflectiveOperationException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`
            :   `ReflectiveOperationException`
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

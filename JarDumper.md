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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java](package-summary.html)
:::

## Class JarDumper {#class-jardumper .title title="Class JarDumper"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.JarDumper

::: description
-   

    ------------------------------------------------------------------------

        public class JarDumper
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor     Description
          --------------- -------------
          `JarDumper()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `List<String>`        | `dump​(Path jarPath)`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `java.util.s          | `dumpEnt              |                       |
        | tream.Stream<String>` | ry​(JarFile file,      |                       |
        |                       |      JarEntry entry)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `prot                 | `isTextF              |                       |
        | ected static boolean` | ile​(String fileName)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `JarDumper`           | `setAs                | ::: block             |
        |                       | mFlags​(int asmFlags)` | Sets the flags that   |
        |                       |                       | are passed to ASM\'s  |
        |                       |                       | `ClassReader` when    |
        |                       |                       | dumping class files.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### JarDumper

                public JarDumper()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#setAsmFlags(int)}

        -   #### setAsmFlags

            ``` methodSignature
            public JarDumper setAsmFlags​(int asmFlags)
            ```

            ::: block
            Sets the flags that are passed to ASM\'s `ClassReader` when
            dumping class files. See
            `ClassReader.accept(ClassVisitor, int)`;
            :::

            [Parameters:]{.paramLabel}

            `asmFlags` -

            [Returns:]{.returnLabel}

        []{#dump(java.nio.file.Path)}

        -   #### dump

            ``` methodSignature
            public List<String> dump​(Path jarPath)
                              throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#dumpEntry(java.util.jar.JarFile,java.util.jar.JarEntry)}

        -   #### dumpEntry

            ``` methodSignature
            public java.util.stream.Stream<String> dumpEntry​(JarFile file,
                                                             JarEntry entry)
            ```

        []{#isTextFile(java.lang.String)}

        -   #### isTextFile

            ``` methodSignature
            protected static boolean isTextFile​(String fileName)
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

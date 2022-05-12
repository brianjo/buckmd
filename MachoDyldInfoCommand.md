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
[Package]{.packageLabelInType} [com.facebook.buck.cxx.toolchain.objectfile](package-summary.html)
:::

## Class MachoDyldInfoCommand {#class-machodyldinfocommand .title title="Class MachoDyldInfoCommand"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.toolchain.objectfile.MachoDyldInfoCommand

::: description
-   

    ------------------------------------------------------------------------

        public abstract class MachoDyldInfoCommand
        extends Object

    ::: block
    Represents the LC_DYLD_INFO/LC_DYLD_INFO_ONLY command. For
    reference, see \"struct dyld_info_command\" at
    https://opensource.apple.com/source/xnu/xnu-1699.32.7/EXTERNAL_HEADERS/mach-o/loader.h
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                Description
          -------------------------- -------------
          `MachoDyldInfoCommand()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                      Description
          ------------------- --------------------------- -------------
          `abstract int`      `getBindInfoOffset()`        
          `abstract int`      `getBindInfoSize()`          
          `abstract int`      `getCommand()`               
          `abstract int`      `getCommandSize()`           
          `abstract int`      `getExportInfoOffset()`      
          `abstract int`      `getExportInfoSize()`        
          `abstract int`      `getLazyBindInfoOffset()`    
          `abstract int`      `getLazyBindInfoSize()`      
          `abstract int`      `getRebaseInfoOffset()`      
          `abstract int`      `getRebaseInfoSize()`        
          `abstract int`      `getWeakBindInfoOffset()`    
          `abstract int`      `getWeakBindInfoSize()`      

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

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

        -   #### MachoDyldInfoCommand

                public MachoDyldInfoCommand()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getCommand()}

        -   #### getCommand

            ``` methodSignature
            public abstract int getCommand()
            ```

        []{#getCommandSize()}

        -   #### getCommandSize

            ``` methodSignature
            public abstract int getCommandSize()
            ```

        []{#getRebaseInfoOffset()}

        -   #### getRebaseInfoOffset

            ``` methodSignature
            public abstract int getRebaseInfoOffset()
            ```

        []{#getRebaseInfoSize()}

        -   #### getRebaseInfoSize

            ``` methodSignature
            public abstract int getRebaseInfoSize()
            ```

        []{#getBindInfoOffset()}

        -   #### getBindInfoOffset

            ``` methodSignature
            public abstract int getBindInfoOffset()
            ```

        []{#getBindInfoSize()}

        -   #### getBindInfoSize

            ``` methodSignature
            public abstract int getBindInfoSize()
            ```

        []{#getWeakBindInfoOffset()}

        -   #### getWeakBindInfoOffset

            ``` methodSignature
            public abstract int getWeakBindInfoOffset()
            ```

        []{#getWeakBindInfoSize()}

        -   #### getWeakBindInfoSize

            ``` methodSignature
            public abstract int getWeakBindInfoSize()
            ```

        []{#getLazyBindInfoOffset()}

        -   #### getLazyBindInfoOffset

            ``` methodSignature
            public abstract int getLazyBindInfoOffset()
            ```

        []{#getLazyBindInfoSize()}

        -   #### getLazyBindInfoSize

            ``` methodSignature
            public abstract int getLazyBindInfoSize()
            ```

        []{#getExportInfoOffset()}

        -   #### getExportInfoOffset

            ``` methodSignature
            public abstract int getExportInfoOffset()
            ```

        []{#getExportInfoSize()}

        -   #### getExportInfoSize

            ``` methodSignature
            public abstract int getExportInfoSize()
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

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

## Class MachoSymTabCommand {#class-machosymtabcommand .title title="Class MachoSymTabCommand"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.toolchain.objectfile.MachoSymTabCommand

::: description
-   

    ------------------------------------------------------------------------

        public abstract class MachoSymTabCommand
        extends Object

    ::: block
    Represents the LC_SYMTAB command. For reference, see \"struct
    symtab_command\" at
    https://opensource.apple.com/source/xnu/xnu-1699.32.7/EXTERNAL_HEADERS/mach-o/loader.h
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor              Description
          ------------------------ -------------
          `MachoSymTabCommand()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                              Description
          ------------------- ----------------------------------- -------------
          `abstract int`      `getCommand()`                       
          `abstract int`      `getCommandSize()`                   
          `abstract int`      `getNumberOfSymbolTableEntries()`    
          `abstract int`      `getStringTableOffset()`             
          `abstract int`      `getStringTableSize()`               
          `abstract int`      `getSymbolTableOffset()`             

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

        -   #### MachoSymTabCommand

                public MachoSymTabCommand()
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

        []{#getSymbolTableOffset()}

        -   #### getSymbolTableOffset

            ``` methodSignature
            public abstract int getSymbolTableOffset()
            ```

        []{#getNumberOfSymbolTableEntries()}

        -   #### getNumberOfSymbolTableEntries

            ``` methodSignature
            public abstract int getNumberOfSymbolTableEntries()
            ```

        []{#getStringTableOffset()}

        -   #### getStringTableOffset

            ``` methodSignature
            public abstract int getStringTableOffset()
            ```

        []{#getStringTableSize()}

        -   #### getStringTableSize

            ``` methodSignature
            public abstract int getStringTableSize()
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

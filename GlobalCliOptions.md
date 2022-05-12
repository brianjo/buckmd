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
[Package]{.packageLabelInType} [com.facebook.buck.support.cli.args](package-summary.html)
:::

## Class GlobalCliOptions {#class-globalclioptions .title title="Class GlobalCliOptions"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.support.cli.args.GlobalCliOptions

::: description
-   

    ------------------------------------------------------------------------

        public class GlobalCliOptions
        extends Object

    ::: block
    Contains CLI options that are common to all of the commands.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                                     Description
          ------------------- ----------------------------------------- -------------
          `static String`     `COMMAND_ARGS_FILE_HELP`                   
          `static String`     `COMMAND_ARGS_FILE_LONG_ARG`               
          `static String`     `CONFIG_FILE_LONG_ARG`                     
          `static String`     `CONFIG_LONG_ARG`                          
          `static String`     `EXCLUDE_INCOMPATIBLE_TARGETS_LONG_ARG`    
          `static String`     `HELP_LONG_ARG`                            
          `static String`     `HOST_PLATFORM_LONG_ARG`                   
          `static String`     `NO_CACHE_LONG_ARG`                        
          `static String`     `NUM_THREADS_LONG_ARG`                     
          `static String`     `OUTPUT_TEST_EVENTS_TO_FILE_LONG_ARG`      
          `static String`     `PROFILE_PARSER_LONG_ARG`                  
          `static String`     `REUSE_CURRENT_CONFIG_ARG`                 
          `static String`     `SKYLARK_PROFILE_LONG_ARG`                 
          `static String`     `TARGET_PLATFORMS_LONG_ARG`                
          `static String`     `VERBOSE_LONG_ARG`                         
          `static String`     `VERBOSE_SHORT_ARG`                        

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor            Description
          ---------------------- -------------
          `GlobalCliOptions()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                    Description
          ------------------- ------------------------------------------------------------------------- -------------
          `static boolean`    `isGlobalOption​(String name)`                                              
          `static boolean`    `isGlobalOption​(org.kohsuke.args4j.spi.OptionHandler<?> optionHandler)`    

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

        []{#HELP_LONG_ARG}

        -   #### HELP_LONG_ARG

                public static final String HELP_LONG_ARG

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.support.cli.args.GlobalCliOptions.HELP_LONG_ARG)

        []{#NO_CACHE_LONG_ARG}

        -   #### NO_CACHE_LONG_ARG

                public static final String NO_CACHE_LONG_ARG

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.support.cli.args.GlobalCliOptions.NO_CACHE_LONG_ARG)

        []{#OUTPUT_TEST_EVENTS_TO_FILE_LONG_ARG}

        -   #### OUTPUT_TEST_EVENTS_TO_FILE_LONG_ARG

                public static final String OUTPUT_TEST_EVENTS_TO_FILE_LONG_ARG

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.support.cli.args.GlobalCliOptions.OUTPUT_TEST_EVENTS_TO_FILE_LONG_ARG)

        []{#PROFILE_PARSER_LONG_ARG}

        -   #### PROFILE_PARSER_LONG_ARG

                public static final String PROFILE_PARSER_LONG_ARG

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.support.cli.args.GlobalCliOptions.PROFILE_PARSER_LONG_ARG)

        []{#NUM_THREADS_LONG_ARG}

        -   #### NUM_THREADS_LONG_ARG

                public static final String NUM_THREADS_LONG_ARG

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.support.cli.args.GlobalCliOptions.NUM_THREADS_LONG_ARG)

        []{#CONFIG_LONG_ARG}

        -   #### CONFIG_LONG_ARG

                public static final String CONFIG_LONG_ARG

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.support.cli.args.GlobalCliOptions.CONFIG_LONG_ARG)

        []{#CONFIG_FILE_LONG_ARG}

        -   #### CONFIG_FILE_LONG_ARG

                public static final String CONFIG_FILE_LONG_ARG

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.support.cli.args.GlobalCliOptions.CONFIG_FILE_LONG_ARG)

        []{#SKYLARK_PROFILE_LONG_ARG}

        -   #### SKYLARK_PROFILE_LONG_ARG

                public static final String SKYLARK_PROFILE_LONG_ARG

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.support.cli.args.GlobalCliOptions.SKYLARK_PROFILE_LONG_ARG)

        []{#VERBOSE_LONG_ARG}

        -   #### VERBOSE_LONG_ARG

                public static final String VERBOSE_LONG_ARG

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.support.cli.args.GlobalCliOptions.VERBOSE_LONG_ARG)

        []{#VERBOSE_SHORT_ARG}

        -   #### VERBOSE_SHORT_ARG

                public static final String VERBOSE_SHORT_ARG

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.support.cli.args.GlobalCliOptions.VERBOSE_SHORT_ARG)

        []{#HOST_PLATFORM_LONG_ARG}

        -   #### HOST_PLATFORM_LONG_ARG

                public static final String HOST_PLATFORM_LONG_ARG

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.support.cli.args.GlobalCliOptions.HOST_PLATFORM_LONG_ARG)

        []{#TARGET_PLATFORMS_LONG_ARG}

        -   #### TARGET_PLATFORMS_LONG_ARG

                public static final String TARGET_PLATFORMS_LONG_ARG

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.support.cli.args.GlobalCliOptions.TARGET_PLATFORMS_LONG_ARG)

        []{#EXCLUDE_INCOMPATIBLE_TARGETS_LONG_ARG}

        -   #### EXCLUDE_INCOMPATIBLE_TARGETS_LONG_ARG

                public static final String EXCLUDE_INCOMPATIBLE_TARGETS_LONG_ARG

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.support.cli.args.GlobalCliOptions.EXCLUDE_INCOMPATIBLE_TARGETS_LONG_ARG)

        []{#REUSE_CURRENT_CONFIG_ARG}

        -   #### REUSE_CURRENT_CONFIG_ARG

                public static final String REUSE_CURRENT_CONFIG_ARG

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.support.cli.args.GlobalCliOptions.REUSE_CURRENT_CONFIG_ARG)

        []{#COMMAND_ARGS_FILE_LONG_ARG}

        -   #### COMMAND_ARGS_FILE_LONG_ARG

                public static final String COMMAND_ARGS_FILE_LONG_ARG

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.support.cli.args.GlobalCliOptions.COMMAND_ARGS_FILE_LONG_ARG)

        []{#COMMAND_ARGS_FILE_HELP}

        -   #### COMMAND_ARGS_FILE_HELP

                public static final String COMMAND_ARGS_FILE_HELP

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.support.cli.args.GlobalCliOptions.COMMAND_ARGS_FILE_HELP)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### GlobalCliOptions

                public GlobalCliOptions()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#isGlobalOption(org.kohsuke.args4j.spi.OptionHandler)}

        -   #### isGlobalOption

            ``` methodSignature
            public static boolean isGlobalOption​(org.kohsuke.args4j.spi.OptionHandler<?> optionHandler)
            ```

        []{#isGlobalOption(java.lang.String)}

        -   #### isGlobalOption

            ``` methodSignature
            public static boolean isGlobalOption​(String name)
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

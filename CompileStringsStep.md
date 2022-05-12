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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.android](package-summary.html)
:::

## Class CompileStringsStep {#class-compilestringsstep .title title="Class CompileStringsStep"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.CompileStringsStep

::: description
-   

    All Implemented Interfaces:
    :   `Step`

    ------------------------------------------------------------------------

        public class CompileStringsStep
        extends Object
        implements Step

    ::: block
    This
    [`Step`](../step/Step.html "interface in com.facebook.buck.step")
    takes a list of string resource files (strings.xml), groups them by
    locales, and for each locale generates a file with all the string
    resources for that locale. Strings.xml files without a resource
    qualifier are mapped to the \"en\" locale.
    A typical strings.xml file looks like:

         <?xml version="1.0" encoding="utf-8"?>
         <resources>
           <string name="resource_name1">I am a string.</string>
           <string name="resource_name2">I am another string.</string>
           <plurals name="time_hours_ago">
             <item quantity="one">1 minute ago</item>
             <item quantity="other">%d minutes ago</item>
           </plurals>
           <string-array name="logging_levels">
             <item>Default</item>
             <item>Verbose</item>
             <item>Debug</item>
           </string-array>
         </resources>

         

    For more information on the xml file format, refer to: [String
    Resources - Android
    Developers](http://developer.android.com/guide/topics/resources/string-resource.html)

    So for each supported locale in a project, this step goes through
    all such xml files for that locale, and builds a map of resource
    name to resource value, where resource value is either:

    1.  a string
    2.  a map of plurals
    3.  a list of strings

    and dumps this map into the output file. See
    [`StringResources`](StringResources.html "class in com.facebook.buck.android")
    for the file format.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `Com                              | ::: block                         |
        | pileStringsStep​(ProjectFilesystem | Note: The ordering of files in    |
        |  filesystem,                   co | the input list determines which   |
        | m.google.common.collect.Immutable | resource value ends up in the     |
        | List<Path> stringFiles,           | output .fbstr file, in the event  |
        |          Path rDotTxtFile,        | of multiple xml files of a locale |
        |             java.util.function.Fu | sharing the same string resource  |
        | nction<String,​Path> pathBuilder)` | name - file that appears first in |
        |                                   | the list wins.                    |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+

        : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static void`         | `b                    | ::: block             |
        |                       | uildResourceNameToIdM | Parses the R.txt file |
        |                       | ap​(ProjectFilesystem  | generated by aapt,    |
        |                       | filesystem,           | looks for resources   |
        |                       |                Path p | of type `string`,     |
        |                       | athToRDotTxtFile,     | `  plurals` and       |
        |                       |                       | `array`, and builds a |
        |                       | Map<String,​Integer> s | map of resource names |
        |                       | tringResourceNameToId | to their              |
        |                       | Map,                  | corresponding ids.    |
        |                       |         Map<String,​In | :::                   |
        |                       | teger> pluralsResourc |                       |
        |                       | eNameToIdMap,         |                       |
        |                       |                  Map< |                       |
        |                       | String,​Integer> array |                       |
        |                       | ResourceNameToIdMap)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `StepExecutionResult` | `execute​(Execu        |                       |
        |                       | tionContext context)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getDescription​(Execu |                       |
        |                       | tionContext context)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getShortName()`      |                       |
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

        []{#<init>(com.facebook.buck.io.filesystem.ProjectFilesystem,com.google.common.collect.ImmutableList,java.nio.file.Path,java.util.function.Function)}

        -   #### CompileStringsStep

                public CompileStringsStep​(ProjectFilesystem filesystem,
                                          com.google.common.collect.ImmutableList<Path> stringFiles,
                                          Path rDotTxtFile,
                                          java.util.function.Function<String,​Path> pathBuilder)

            ::: block
            Note: The ordering of files in the input list determines
            which resource value ends up in the output .fbstr file, in
            the event of multiple xml files of a locale sharing the same
            string resource name - file that appears first in the list
            wins.
            :::

            [Parameters:]{.paramLabel}
            :   `stringFiles` - Set containing paths to strings.xml
                files matching
                [`GetStringsFilesStep.STRINGS_FILE_PATH`](GetStringsFilesStep.html#STRINGS_FILE_PATH)
            :   `rDotTxtFile` - Path to the R.txt file generated by
                aapt.
            :   `pathBuilder` - Builds a path to store a .fbstr file at.
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#execute(com.facebook.buck.core.build.execution.context.ExecutionContext)}

        -   #### execute

            ``` methodSignature
            public StepExecutionResult execute​(ExecutionContext context)
                                        throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `execute` in interface `Step`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#buildResourceNameToIdMap(com.facebook.buck.io.filesystem.ProjectFilesystem,java.nio.file.Path,java.util.Map,java.util.Map,java.util.Map)}

        -   #### buildResourceNameToIdMap

            ``` methodSignature
            public static void buildResourceNameToIdMap​(ProjectFilesystem filesystem,
                                                        Path pathToRDotTxtFile,
                                                        Map<String,​Integer> stringResourceNameToIdMap,
                                                        Map<String,​Integer> pluralsResourceNameToIdMap,
                                                        Map<String,​Integer> arrayResourceNameToIdMap)
                                                 throws IOException
            ```

            ::: block
            Parses the R.txt file generated by aapt, looks for resources
            of type `string`, `  plurals` and `array`, and builds a map
            of resource names to their corresponding ids.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getShortName()}

        -   #### getShortName

            ``` methodSignature
            public String getShortName()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getShortName` in interface `Step`

            [Returns:]{.returnLabel}
            :   a short name/description for the command, such as
                \"javac\". Should fit on one line.

        []{#getDescription(com.facebook.buck.core.build.execution.context.ExecutionContext)}

        -   #### getDescription

            ``` methodSignature
            public String getDescription​(ExecutionContext context)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDescription` in interface `Step`
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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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

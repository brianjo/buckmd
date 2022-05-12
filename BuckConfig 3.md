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
[Package]{.packageLabelInType} [com.facebook.buck.core.config](package-summary.html)
:::

## Class BuckConfig {#class-buckconfig .title title="Class BuckConfig"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.config.BuckConfig

::: description
-   

    ------------------------------------------------------------------------

        public class BuckConfig
        extends Object

    ::: block
    Structured representation of data read from a `.buckconfig` file.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                          Description
          -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `BuckConfig​(Config config,           ProjectFilesystem projectFilesystem,           Architecture architecture,           Platform platform,           com.google.common.collect.ImmutableMap<String,​String> environment,           java.util.function.Function<String,​UnconfiguredBuildTarget> buildTargetParser)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Path`                | `che                  |                       |
        |                       | ckPathExistsAndResolv |                       |
        |                       | e​(String pathString,  |                       |
        |                       |                       |                       |
        |                       |     String errorMsg)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `equals​(Object obj)`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Architecture`        | `getArchitecture()`   |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Boolean>`   | `getBoolean​(String se |                       |
        |                       | ctionName,            |                       |
        |                       | String propertyName)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getB                 |                       |
        |                       | ooleanValue​(String se |                       |
        |                       | ctionName,            |                       |
        |                       |      String propertyN |                       |
        |                       | ame,                b |                       |
        |                       | oolean defaultValue)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `O                    | `getBuildT            |                       |
        | ptional<BuildTarget>` | arget​(String section, |                       |
        |                       |                String |                       |
        |                       |  field,               |                       |
        |                       |  TargetConfiguration  |                       |
        |                       | targetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuildTarget`         | `getBu                |                       |
        |                       | ildTargetForFullyQual |                       |
        |                       | ifiedTarget​(String ta |                       |
        |                       | rget,                 |                       |
        |                       |                       |                       |
        |                       |  TargetConfiguration  |                       |
        |                       | targetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Config`              | `getConfig()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.c         | `getEntriesForSec     |                       |
        | ommon.collect.Immutab | tion​(String section)` |                       |
        | leMap<String,​String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `<T extends           | `getEn                |                       |
        |  Enum<T>>Optional<T>` | um​(String section,    |                       |
        |                       |      String field,    |                       |
        |                       |      Class<T> clazz)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.c         | `getEnvironment()`    |                       |
        | ommon.collect.Immutab |                       |                       |
        | leMap<String,​String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `<T extends E         | `get                  | ::: block             |
        | num<T>>Map<T,​Double>` | ExperimentGroups​(Stri | Returns the           |
        |                       | ng section,           | probabilities for     |
        |                       |           String fiel | each group in an      |
        |                       | d,                    | experiment.           |
        |                       |  Class<T> enumClass)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ProjectFilesystem`   | `getFilesystem()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Float>`     | `getFloat​(String      |                       |
        |                       | sectionName,          |                       |
        |                       | String propertyName)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `getFullyQu           |                       |
        | common.collect.Immuta | alifiedBuildTargets​(S |                       |
        | bleList<BuildTarget>` | tring section,        |                       |
        |                       |                       |                       |
        |                       |   String key,         |                       |
        |                       |                       |                       |
        |                       |  TargetConfiguration  |                       |
        |                       | targetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `OptionalInt`         | `getInteger​(String se |                       |
        |                       | ctionName,            |                       |
        |                       | String propertyName)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getListWitho         |                       |
        | ogle.common.collect.I | utComments​(String sec |                       |
        | mmutableList<String>` | tion,                 |                       |
        |                       |        String field)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getListW             |                       |
        | ogle.common.collect.I | ithoutComments​(String |                       |
        | mmutableList<String>` |  section,             |                       |
        |                       |            String fie |                       |
        |                       | ld,                   |                       |
        |                       |      char splitChar)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getLocalhost()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Long>`      | `getLong​(String       |                       |
        |                       |  sectionName,         |                       |
        |                       | String propertyName)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.c         | `g                    |                       |
        | ommon.collect.Immutab | etMap​(String section, |                       |
        | leMap<String,​String>` |        String field)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `O                    | `get                  |                       |
        | ptional<BuildTarget>` | MaybeBuildTarget​(Stri |                       |
        |                       | ng section,           |                       |
        |                       |           String fiel |                       |
        |                       | d,                    |                       |
        |                       |  TargetConfiguration  |                       |
        |                       | targetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Unco        | `getMaybeU            |                       |
        | nfiguredBuildTarget>` | nconfiguredBuildTarge |                       |
        |                       | t​(String section,     |                       |
        |                       |                       |                       |
        |                       |        String field)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<com.goo     | `getOpti              |                       |
        | gle.common.collect.Im | onalListWithoutCommen |                       |
        | mutableList<String>>` | ts​(String section,    |                       |
        |                       |                       |                       |
        |                       |        String field)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<com.goo     | `getOptional          |                       |
        | gle.common.collect.Im | ListWithoutComments​(S |                       |
        | mutableList<String>>` | tring section,        |                       |
        |                       |                       |                       |
        |                       |    String field,      |                       |
        |                       |                       |                       |
        |                       |      char splitChar)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<com.g       | `                     |                       |
        | oogle.common.collect. | getOptionalPathList​(S |                       |
        | ImmutableList<Path>>` | tring section,        |                       |
        |                       |              String f |                       |
        |                       | ield,                 |                       |
        |                       |     boolean resolve)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `<T> T`               | `getOrThrow​(String    |                       |
        |                       |  section,           S |                       |
        |                       | tring field,          |                       |
        |                       |   Optional<T> value)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Path>`      | `getPat               |                       |
        |                       | h​(String sectionName, |                       |
        |                       |         String name)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Path>`      | `getPath​(String secti |                       |
        |                       | onName,        String |                       |
        |                       |  name,        boolean |                       |
        |                       |  isCellRootRelative)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `PathSourcePath`      | `getPathS             |                       |
        |                       | ourcePath​(Path path)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `PathSourcePath`      | `getP                 |                       |
        |                       | athSourcePath​(Path pa |                       |
        |                       | th,                   |                       |
        |                       | String errorMessage)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Platform`            | `getPlatform()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `g                    |                       |
        |                       | etRawValue​(String sec |                       |
        |                       | tionName,             |                       |
        |                       | String propertyName)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuildTarget`         | `getRequiredB         |                       |
        |                       | uildTarget​(String sec |                       |
        |                       | tion,                 |                       |
        |                       |        String field,  |                       |
        |                       |                       |                       |
        |                       |  TargetConfiguration  |                       |
        |                       | targetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getRequiredPath​(Str  |                       |
        |                       | ing section,          |                       |
        |                       |        String field)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `O                    | `getSection           |                       |
        | ptional<com.google.co | ​(String sectionName)` |                       |
        | mmon.collect.Immutabl |                       |                       |
        | eMap<String,​String>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.g                | `getSections()`       |                       |
        | oogle.common.collect. |                       |                       |
        | ImmutableSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getSou               |                       |
        | Optional<SourcePath>` | rcePath​(String sectio |                       |
        |                       | n,              Strin |                       |
        |                       | g field,              |                       |
        |                       |  TargetConfiguration  |                       |
        |                       | targetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Unc                  | `ge                   |                       |
        | onfiguredBuildTarget` | tUnconfiguredBuildTar |                       |
        |                       | getForFullyQualifiedT |                       |
        |                       | arget​(String target)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<URI>`       | `g                    |                       |
        |                       | etUrl​(String section, |                       |
        |                       |        String field)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getValue​(String      |                       |
        |                       | sectionName,          |                       |
        |                       | String propertyName)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `<T extends Conf      | `g                    | ::: block             |
        | igView<BuckConfig>>T` | etView​(Class<T> cls)` | Get a                 |
        |                       |                       | [`ConfigView`         |
        |                       |                       | ](ConfigView.html "in |
        |                       |                       | terface in com.facebo |
        |                       |                       | ok.buck.core.config") |
        |                       |                       | of this config.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `hasUserDefinedVal    |                       |
        |                       | ue​(String sectionName |                       |
        |                       | ,                     |                       |
        |                       | String propertyName)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `resolveNonNullP      |                       |
        |                       | athOutsideTheProjectF |                       |
        |                       | ilesystem​(Path path)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `resolvePathThatMa    |                       |
        |                       | yBeOutsideTheProjectF |                       |
        |                       | ilesystem​(Path path)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuckConfig`          | `withBuildTargetPa    | ::: block             |
        |                       | rser​(java.util.functi | Returns a clone of    |
        |                       | on.Function<String,​Un | the current config    |
        |                       | configuredBuildTarget | with a the argument   |
        |                       | > buildTargetParser)` | CellPathResolver.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.util.config.Config,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.util.environment.Architecture,com.facebook.buck.util.environment.Platform,com.google.common.collect.ImmutableMap,java.util.function.Function)}

        -   #### BuckConfig

                public BuckConfig​(Config config,
                                  ProjectFilesystem projectFilesystem,
                                  Architecture architecture,
                                  Platform platform,
                                  com.google.common.collect.ImmutableMap<String,​String> environment,
                                  java.util.function.Function<String,​UnconfiguredBuildTarget> buildTargetParser)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#withBuildTargetParser(java.util.function.Function)}

        -   #### withBuildTargetParser

            ``` methodSignature
            public BuckConfig withBuildTargetParser​(java.util.function.Function<String,​UnconfiguredBuildTarget> buildTargetParser)
            ```

            ::: block
            Returns a clone of the current config with a the argument
            CellPathResolver.
            :::

        []{#getView(java.lang.Class)}

        -   #### getView

            ``` methodSignature
            public <T extends ConfigView<BuckConfig>> T getView​(Class<T> cls)
            ```

            ::: block
            Get a
            [`ConfigView`](ConfigView.html "interface in com.facebook.buck.core.config")
            of this config.
            :::

            [Type Parameters:]{.paramLabel}
            :   `T` - Type of the config view.

            [Parameters:]{.paramLabel}
            :   `cls` - Class of the config view.

        []{#getArchitecture()}

        -   #### getArchitecture

            ``` methodSignature
            public Architecture getArchitecture()
            ```

        []{#getEntriesForSection(java.lang.String)}

        -   #### getEntriesForSection

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​String> getEntriesForSection​(String section)
            ```

        []{#getListWithoutComments(java.lang.String,java.lang.String)}

        -   #### getListWithoutComments

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getListWithoutComments​(String section,
                                                                                          String field)
            ```

        []{#getListWithoutComments(java.lang.String,java.lang.String,char)}

        -   #### getListWithoutComments

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getListWithoutComments​(String section,
                                                                                          String field,
                                                                                          char splitChar)
            ```

        []{#getOptionalListWithoutComments(java.lang.String,java.lang.String)}

        -   #### getOptionalListWithoutComments

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableList<String>> getOptionalListWithoutComments​(String section,
                                                                                                            String field)
            ```

        []{#getOptionalListWithoutComments(java.lang.String,java.lang.String,char)}

        -   #### getOptionalListWithoutComments

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableList<String>> getOptionalListWithoutComments​(String section,
                                                                                                            String field,
                                                                                                            char splitChar)
            ```

        []{#getOptionalPathList(java.lang.String,java.lang.String,boolean)}

        -   #### getOptionalPathList

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableList<Path>> getOptionalPathList​(String section,
                                                                                               String field,
                                                                                               boolean resolve)
            ```

        []{#getUnconfiguredBuildTargetForFullyQualifiedTarget(java.lang.String)}

        -   #### getUnconfiguredBuildTargetForFullyQualifiedTarget

            ``` methodSignature
            public UnconfiguredBuildTarget getUnconfiguredBuildTargetForFullyQualifiedTarget​(String target)
            ```

        []{#getBuildTargetForFullyQualifiedTarget(java.lang.String,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getBuildTargetForFullyQualifiedTarget

            ``` methodSignature
            public BuildTarget getBuildTargetForFullyQualifiedTarget​(String target,
                                                                     TargetConfiguration targetConfiguration)
            ```

        []{#getFullyQualifiedBuildTargets(java.lang.String,java.lang.String,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getFullyQualifiedBuildTargets

            ``` methodSignature
            public com.google.common.collect.ImmutableList<BuildTarget> getFullyQualifiedBuildTargets​(String section,
                                                                                                      String key,
                                                                                                      TargetConfiguration targetConfiguration)
            ```

        []{#getBuildTarget(java.lang.String,java.lang.String,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getBuildTarget

            ``` methodSignature
            public Optional<BuildTarget> getBuildTarget​(String section,
                                                        String field,
                                                        TargetConfiguration targetConfiguration)
            ```

            [Returns:]{.returnLabel}
            :   the parsed BuildTarget in the given section and field,
                if set.

        []{#getMaybeBuildTarget(java.lang.String,java.lang.String,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getMaybeBuildTarget

            ``` methodSignature
            public Optional<BuildTarget> getMaybeBuildTarget​(String section,
                                                             String field,
                                                             TargetConfiguration targetConfiguration)
            ```

            [Returns:]{.returnLabel}

            :   the parsed BuildTarget in the given section and field,
                if set and a valid build target.

                This is useful if you use getTool to get the target, if
                any, but allow filesystem references.

        []{#getMaybeUnconfiguredBuildTarget(java.lang.String,java.lang.String)}

        -   #### getMaybeUnconfiguredBuildTarget

            ``` methodSignature
            public Optional<UnconfiguredBuildTarget> getMaybeUnconfiguredBuildTarget​(String section,
                                                                                     String field)
            ```

            [Returns:]{.returnLabel}

            :   the parsed UnconfiguredBuildTarget in the given section
                and field, if set and a valid build target.

                This is useful if you use getTool to get the target, if
                any, but allow filesystem references.

        []{#getRequiredBuildTarget(java.lang.String,java.lang.String,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getRequiredBuildTarget

            ``` methodSignature
            public BuildTarget getRequiredBuildTarget​(String section,
                                                      String field,
                                                      TargetConfiguration targetConfiguration)
            ```

            [Returns:]{.returnLabel}
            :   the parsed BuildTarget in the given section and field.

        []{#getEnum(java.lang.String,java.lang.String,java.lang.Class)}

        -   #### getEnum

            ``` methodSignature
            public <T extends Enum<T>> Optional<T> getEnum​(String section,
                                                           String field,
                                                           Class<T> clazz)
            ```

        []{#getSourcePath(java.lang.String,java.lang.String,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getSourcePath

            ``` methodSignature
            public Optional<SourcePath> getSourcePath​(String section,
                                                      String field,
                                                      TargetConfiguration targetConfiguration)
            ```

            [Returns:]{.returnLabel}
            :   a
                [`SourcePath`](../sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")
                identified by a \@{link BuildTarget} or
                [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
                reference by the given section:field, if set.

        []{#getPathSourcePath(java.nio.file.Path)}

        -   #### getPathSourcePath

            ``` methodSignature
            public PathSourcePath getPathSourcePath​(Path path)
            ```

            [Returns:]{.returnLabel}
            :   a
                [`SourcePath`](../sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")
                identified by a
                [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}.

        []{#getPathSourcePath(java.nio.file.Path,java.lang.String)}

        -   #### getPathSourcePath

            ``` methodSignature
            public PathSourcePath getPathSourcePath​(Path path,
                                                    String errorMessage)
            ```

            [Parameters:]{.paramLabel}
            :   `errorMessage` - the error message to throw if path is
                not found

            [Returns:]{.returnLabel}
            :   a
                [`SourcePath`](../sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")
                identified by a
                [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}.

        []{#resolvePathThatMayBeOutsideTheProjectFilesystem(java.nio.file.Path)}

        -   #### resolvePathThatMayBeOutsideTheProjectFilesystem

            ``` methodSignature
            public Path resolvePathThatMayBeOutsideTheProjectFilesystem​(Path path)
            ```

        []{#resolveNonNullPathOutsideTheProjectFilesystem(java.nio.file.Path)}

        -   #### resolveNonNullPathOutsideTheProjectFilesystem

            ``` methodSignature
            public Path resolveNonNullPathOutsideTheProjectFilesystem​(Path path)
            ```

        []{#getLocalhost()}

        -   #### getLocalhost

            ``` methodSignature
            public String getLocalhost()
            ```

        []{#getPlatform()}

        -   #### getPlatform

            ``` methodSignature
            public Platform getPlatform()
            ```

        []{#hasUserDefinedValue(java.lang.String,java.lang.String)}

        -   #### hasUserDefinedValue

            ``` methodSignature
            public boolean hasUserDefinedValue​(String sectionName,
                                               String propertyName)
            ```

        []{#getSection(java.lang.String)}

        -   #### getSection

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableMap<String,​String>> getSection​(String sectionName)
            ```

        []{#getValue(java.lang.String,java.lang.String)}

        -   #### getValue

            ``` methodSignature
            public Optional<String> getValue​(String sectionName,
                                             String propertyName)
            ```

            [Returns:]{.returnLabel}
            :   the string value for the config settings, where present
                empty values are `      Optional.empty()`.

        []{#getRawValue(java.lang.String,java.lang.String)}

        -   #### getRawValue

            ``` methodSignature
            public Optional<String> getRawValue​(String sectionName,
                                                String propertyName)
            ```

            [Returns:]{.returnLabel}
            :   the string value for the config settings, where present
                empty values are `      Optional[]`.

        []{#getInteger(java.lang.String,java.lang.String)}

        -   #### getInteger

            ``` methodSignature
            public OptionalInt getInteger​(String sectionName,
                                          String propertyName)
            ```

        []{#getLong(java.lang.String,java.lang.String)}

        -   #### getLong

            ``` methodSignature
            public Optional<Long> getLong​(String sectionName,
                                          String propertyName)
            ```

        []{#getFloat(java.lang.String,java.lang.String)}

        -   #### getFloat

            ``` methodSignature
            public Optional<Float> getFloat​(String sectionName,
                                            String propertyName)
            ```

        []{#getBoolean(java.lang.String,java.lang.String)}

        -   #### getBoolean

            ``` methodSignature
            public Optional<Boolean> getBoolean​(String sectionName,
                                                String propertyName)
            ```

        []{#getBooleanValue(java.lang.String,java.lang.String,boolean)}

        -   #### getBooleanValue

            ``` methodSignature
            public boolean getBooleanValue​(String sectionName,
                                           String propertyName,
                                           boolean defaultValue)
            ```

        []{#getUrl(java.lang.String,java.lang.String)}

        -   #### getUrl

            ``` methodSignature
            public Optional<URI> getUrl​(String section,
                                        String field)
            ```

        []{#getMap(java.lang.String,java.lang.String)}

        -   #### getMap

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​String> getMap​(String section,
                                                                                      String field)
            ```

        []{#getExperimentGroups(java.lang.String,java.lang.String,java.lang.Class)}

        -   #### getExperimentGroups

            ``` methodSignature
            public <T extends Enum<T>> Map<T,​Double> getExperimentGroups​(String section,
                                                                               String field,
                                                                               Class<T> enumClass)
            ```

            ::: block
            Returns the probabilities for each group in an experiment.
            :::

        []{#getOrThrow(java.lang.String,java.lang.String,java.util.Optional)}

        -   #### getOrThrow

            ``` methodSignature
            public <T> T getOrThrow​(String section,
                                    String field,
                                    Optional<T> value)
            ```

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(Object obj)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `Object`

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `Object`

        []{#getEnvironment()}

        -   #### getEnvironment

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​String> getEnvironment()
            ```

        []{#getPath(java.lang.String,java.lang.String)}

        -   #### getPath

            ``` methodSignature
            public Optional<Path> getPath​(String sectionName,
                                          String name)
            ```

            [Returns:]{.returnLabel}
            :   the path for the given section and property.

        []{#getRequiredPath(java.lang.String,java.lang.String)}

        -   #### getRequiredPath

            ``` methodSignature
            public Path getRequiredPath​(String section,
                                        String field)
            ```

        []{#getPath(java.lang.String,java.lang.String,boolean)}

        -   #### getPath

            ``` methodSignature
            public Optional<Path> getPath​(String sectionName,
                                          String name,
                                          boolean isCellRootRelative)
            ```

        []{#checkPathExistsAndResolve(java.lang.String,java.lang.String)}

        -   #### checkPathExistsAndResolve

            ``` methodSignature
            public Path checkPathExistsAndResolve​(String pathString,
                                                  String errorMsg)
            ```

        []{#getSections()}

        -   #### getSections

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<String> getSections()
            ```

        []{#getConfig()}

        -   #### getConfig

            ``` methodSignature
            public Config getConfig()
            ```

        []{#getFilesystem()}

        -   #### getFilesystem

            ``` methodSignature
            public ProjectFilesystem getFilesystem()
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

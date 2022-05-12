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

## Class AndroidBuildConfig {#class-androidbuildconfig .title title="Class AndroidBuildConfig"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.core.rules.impl.AbstractBuildRuleWithDeclaredAndExtraDeps](../core/rules/impl/AbstractBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

        -   -   com.facebook.buck.android.AndroidBuildConfig

::: description
-   

    All Implemented Interfaces:
    :   `BuildEngineAction`, `AllowsNonAnnotatedFields`,
        `HasDeclaredAndExtraDeps`, `BuildRule`, `HasNameAndType`,
        `Comparable<BuildRule>`

    ------------------------------------------------------------------------

        public class AndroidBuildConfig
        extends AbstractBuildRuleWithDeclaredAndExtraDeps

    ::: block
    [`BuildRule`](../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
    that can generate a `BuildConfig.java` file and compile it so it can
    be used as a Java library.
    This rule functions as a `java_library` that can be used as a
    dependency of an `  android_library`, but whose implementation may
    be swapped out by the `android_binary` that transitively includes
    the `android_build_config`. Specifically, its compile-time
    implementation will use non-constant-expression (see JLS 15.28),
    placeholder values (because they cannot be inlined) for the purposes
    of compilation that will be swapped out with final, production
    values (that can be inlined) when building the final APK. Consider
    the following example:

         android_build_config(
           name = 'build_config',
           package = 'com.example.pkg',
         )

         # The .java files in this library may contain references to the boolean
         # com.example.pkg.BuildConfig.DEBUG because :build_config is in the deps.
         android_library(
           name = 'mylib',
           srcs = glob(['src/**/*.java']),
           deps = [
             ':build_config',
           ],
         )

         android_binary(
           name = 'debug',
           package_type = 'DEBUG',
           keystore =  '//keystores:debug',
           manifest = 'AndroidManifest.xml',
           target = 'Google Inc.:Google APIs:19',
           deps = [
             ':mylib',
           ],
         )

         android_binary(
           name = 'release',
           package_type = 'RELEASE',
           keystore =  '//keystores:release',
           manifest = 'AndroidManifest.xml',
           target = 'Google Inc.:Google APIs:19',
           deps = [
             ':mylib',
           ],
         )
         

    The `:mylib` rule will be compiled against a version of
    `BuildConfig.java` whose contents are:
         package com.example.pkg;
         public class BuildConfig {
           private BuildConfig() {}
           public static final boolean DEBUG = !Boolean.parseBoolean(null);
         }
         

    Note that the value is not a constant expression, so it cannot be
    inlined by `javac`. When building `:debug` and `:release`, the
    `BuildConfig.class` file that `  :mylib` was compiled against will
    not be included in the APK as the other transitive Java deps of the
    `android_binary` will. The `BuildConfig.class` will be replaced with
    one that corresponds to the value of the `package_type` argument to
    the `android_binary` rule. For example, `:debug` will include a
    `BuildConfig.class` file that is compiled from:
         package com.example.pkg;
         public class BuildConfig {
           private BuildConfig() {}
           public static final boolean DEBUG = true;
         }
         

    whereas `:release` will include a `BuildConfig.class` file that is
    compiled from:
         package com.example.pkg;
         public class BuildConfig {
           private BuildConfig() {}
           public static final boolean DEBUG = false;
         }
         

    This swap happens before ProGuard is run as part of building the
    APK, so it will be able to exploit the \"final-ness\" of the `DEBUG`
    constant in any whole-program optimization that it performs.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                                                                                                                                                                                                                                                                                                                                             Description
          -------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `protected `   `AndroidBuildConfig​(BuildTarget buildTarget,                   ProjectFilesystem projectFilesystem,                   BuildRuleParams buildRuleParams,                   String javaPackage,                   BuildConfigFields defaultValues,                   Optional<SourcePath> valuesFile,                   boolean useConstantExpressions)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                 Method                                                                                  Description
          ------------------------------------------------- --------------------------------------------------------------------------------------- -------------
          `BuildConfigFields`                               `getBuildConfigFields()`                                                                 
          `com.google.common.collect.ImmutableList<Step>`   `getBuildSteps​(BuildContext context,              BuildableContext buildableContext)`    
          `String`                                          `getJavaPackage()`                                                                       
          `SourcePath`                                      `getSourcePathToOutput()`                                                                
          `boolean`                                         `isUseConstantExpressions()`                                                             

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.AbstractBuildRuleWithDeclaredAndExtraDeps}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[AbstractBuildRuleWithDeclaredAndExtraDeps](../core/rules/impl/AbstractBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

            `deprecatedGetExtraDeps, getBuildDeps, getDeclaredDeps, getTargetGraphOnlyDeps`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.AbstractBuildRule}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[AbstractBuildRule](../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

            `equals, getBuildTarget, getDependencies, getProjectFilesystem, getSourcePathOutputs, getType, hasBuildSteps, hashCode, injectFields, isCacheable, toString, updateBuildRuleResolver`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.BuildRule}

            ### Methods inherited from interface com.facebook.buck.core.rules.[BuildRule](../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")

            `compareTo, getFullyQualifiedName, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams,java.lang.String,com.facebook.buck.rules.coercer.BuildConfigFields,java.util.Optional,boolean)}

        -   #### AndroidBuildConfig

                protected AndroidBuildConfig​(BuildTarget buildTarget,
                                             ProjectFilesystem projectFilesystem,
                                             BuildRuleParams buildRuleParams,
                                             String javaPackage,
                                             BuildConfigFields defaultValues,
                                             Optional<SourcePath> valuesFile,
                                             boolean useConstantExpressions)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBuildSteps(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.core.build.buildable.context.BuildableContext)}

        -   #### getBuildSteps

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Step> getBuildSteps​(BuildContext context,
                                                                               BuildableContext buildableContext)
            ```

        []{#getSourcePathToOutput()}

        -   #### getSourcePathToOutput

            ``` methodSignature
            public SourcePath getSourcePathToOutput()
            ```

        []{#getJavaPackage()}

        -   #### getJavaPackage

            ``` methodSignature
            public String getJavaPackage()
            ```

        []{#isUseConstantExpressions()}

        -   #### isUseConstantExpressions

            ``` methodSignature
            public boolean isUseConstantExpressions()
            ```

        []{#getBuildConfigFields()}

        -   #### getBuildConfigFields

            ``` methodSignature
            public BuildConfigFields getBuildConfigFields()
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

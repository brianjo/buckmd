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
-   [Nested](#nested.class.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.core.test.rule](package-summary.html)
:::

## Class ExternalTestRunnerTestSpec {#class-externaltestrunnertestspec .title title="Class ExternalTestRunnerTestSpec"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.test.rule.ExternalTestRunnerTestSpec

::: description
-   

    All Implemented Interfaces:
    :   `ExternalTestSpec`,
        `com.fasterxml.jackson.databind.JsonSerializable`

    ------------------------------------------------------------------------

        public abstract class ExternalTestRunnerTestSpec
        extends Object
        implements ExternalTestSpec

    ::: block
    A JSON-serializable structure that gets passed to external test
    runners.
    NOTE: We\'re relying on the fact we\'re using POJOs here and that
    all the sub-types are JSON-serializable already. Be careful that we
    don\'t break serialization when adding item here.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                                  Description
          ------------------- -------------------------------------- -------------
          `static class `     `ExternalTestRunnerTestSpec.Builder`    

          : Nested Classes[ ]{.tabEnd}

        -   []{#nested.classes.inherited.from.class.com.fasterxml.jackson.databind.JsonSerializable}

            ### Nested classes/interfaces inherited from interface com.fasterxml.jackson.databind.JsonSerializable

            `com.fasterxml.jackson.databind.JsonSerializable.Base`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                      Description
          -------------------------------- -------------
          `ExternalTestRunnerTestSpec()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                                                              Method                                                                                                                                                                                                                                                       Description
          -------------------------------------------------------------------------------------------------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `static ExternalTestRunnerTestSpec.Builder`                                                                    `builder()`                                                                                                                                                                                                                                                   
          `abstract com.google.common.collect.ImmutableSet<Path>`                                                        `getAdditionalCoverageTargets()`                                                                                                                                                                                                                              
          `abstract com.google.common.collect.ImmutableList<String>`                                                     `getCommand()`                                                                                                                                                                                                                                                
          `abstract com.google.common.collect.ImmutableList<String>`                                                     `getContacts()`                                                                                                                                                                                                                                               
          `abstract Path`                                                                                                `getCwd()`                                                                                                                                                                                                                                                    
          `abstract com.google.common.collect.ImmutableMap<String,​String>`                                               `getEnv()`                                                                                                                                                                                                                                                    
          `abstract com.google.common.collect.ImmutableList<String>`                                                     `getLabels()`                                                                                                                                                                                                                                                 
          `abstract com.google.common.collect.ImmutableList<Pair<Float,​com.google.common.collect.ImmutableSet<Path>>>`   `getNeededCoverage()`                                                                                                                                                                                                                                         
          `abstract com.google.common.collect.ImmutableSet<Path>`                                                        `getRequiredPaths()`                                                                                                                                                                                                                                          
          `abstract BuildTarget`                                                                                         `getTarget()`                                                                                                                                                                                                                                                 
          `abstract String`                                                                                              `getType()`                                                                                                                                                                                                                                                   
          `void`                                                                                                         `serialize​(com.fasterxml.jackson.core.JsonGenerator jsonGenerator,          com.fasterxml.jackson.databind.SerializerProvider serializerProvider)`                                                                                                            
          `void`                                                                                                         `serializeWithType​(com.fasterxml.jackson.core.JsonGenerator jsonGenerator,                  com.fasterxml.jackson.databind.SerializerProvider serializerProvider,                  com.fasterxml.jackson.databind.jsontype.TypeSerializer typeSerializer)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
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

        -   #### ExternalTestRunnerTestSpec

                public ExternalTestRunnerTestSpec()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getTarget()}

        -   #### getTarget

            ``` methodSignature
            public abstract BuildTarget getTarget()
            ```

            [Returns:]{.returnLabel}
            :   the build target of this rule.

        []{#getType()}

        -   #### getType

            ``` methodSignature
            public abstract String getType()
            ```

            [Returns:]{.returnLabel}
            :   a test-specific type string which classifies the test
                class, so the external runner knows how to parse the
                output.

        []{#getCommand()}

        -   #### getCommand

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<String> getCommand()
            ```

            [Returns:]{.returnLabel}
            :   the command the external test runner must invoke to run
                the test.

        []{#getCwd()}

        -   #### getCwd

            ``` methodSignature
            public abstract Path getCwd()
            ```

            [Returns:]{.returnLabel}
            :   the directory from which the external runner should
                invoke the command.

        []{#getNeededCoverage()}

        -   #### getNeededCoverage

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<Pair<Float,​com.google.common.collect.ImmutableSet<Path>>> getNeededCoverage()
            ```

            [Returns:]{.returnLabel}
            :   coverage threshold and list of source path to be passed
                the test command for test coverage.

        []{#getAdditionalCoverageTargets()}

        -   #### getAdditionalCoverageTargets

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSet<Path> getAdditionalCoverageTargets()
            ```

            [Returns:]{.returnLabel}
            :   a list of source path to be passed the test command for
                calculating additional test coverage.

        []{#getEnv()}

        -   #### getEnv

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableMap<String,​String> getEnv()
            ```

            [Returns:]{.returnLabel}
            :   environment variables the external test runner should
                provide for the test command.

        []{#getLabels()}

        -   #### getLabels

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<String> getLabels()
            ```

            [Returns:]{.returnLabel}
            :   test labels.

        []{#getContacts()}

        -   #### getContacts

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<String> getContacts()
            ```

            [Returns:]{.returnLabel}
            :   test contacts.

        []{#getRequiredPaths()}

        -   #### getRequiredPaths

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSet<Path> getRequiredPaths()
            ```

            [Returns:]{.returnLabel}
            :   the set of files and directories (may include symlinks
                or symlink-trees) which \*must\* be materialized in
                order to run this test. This is used by external test
                runners that wish to distribute tests to other machines.
                Some examples of what my contained include: java_tests:
                runtime classpath, android_instrumentation_test:
                test_apk and apk_under_test paths, python_tests:
                location of python files if style=inplace

        []{#serialize(com.fasterxml.jackson.core.JsonGenerator,com.fasterxml.jackson.databind.SerializerProvider)}

        -   #### serialize

            ``` methodSignature
            public void serialize​(com.fasterxml.jackson.core.JsonGenerator jsonGenerator,
                                  com.fasterxml.jackson.databind.SerializerProvider serializerProvider)
                           throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `serialize` in interface `ExternalTestSpec`

            [Specified by:]{.overrideSpecifyLabel}
            :   `serialize` in
                interface `com.fasterxml.jackson.databind.JsonSerializable`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#serializeWithType(com.fasterxml.jackson.core.JsonGenerator,com.fasterxml.jackson.databind.SerializerProvider,com.fasterxml.jackson.databind.jsontype.TypeSerializer)}

        -   #### serializeWithType

            ``` methodSignature
            public void serializeWithType​(com.fasterxml.jackson.core.JsonGenerator jsonGenerator,
                                          com.fasterxml.jackson.databind.SerializerProvider serializerProvider,
                                          com.fasterxml.jackson.databind.jsontype.TypeSerializer typeSerializer)
                                   throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `serializeWithType` in interface `ExternalTestSpec`

            [Specified by:]{.overrideSpecifyLabel}
            :   `serializeWithType` in
                interface `com.fasterxml.jackson.databind.JsonSerializable`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static ExternalTestRunnerTestSpec.Builder builder()
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
-   [Nested](#nested.class.summary) \| 
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

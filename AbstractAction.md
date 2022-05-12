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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.actions](package-summary.html)
:::

## Class AbstractAction {#class-abstractaction .title title="Class AbstractAction"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.rules.actions.AbstractAction

::: description
-   

    All Implemented Interfaces:
    :   `BuildEngineAction`, `Action`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `CopyAction`, `RunAction`, `WriteAction`

    ------------------------------------------------------------------------

        public abstract class AbstractAction
        extends Object
        implements Action

    ::: block
    Base implementation of an
    [`Action`](Action.html "interface in com.facebook.buck.core.rules.actions")
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                                                          Field       Description
          -------------------------------------------------------------------------- ----------- -------------
          `protected com.google.common.collect.ImmutableSortedSet<Artifact>`         `inputs`     
          `protected com.google.common.collect.ImmutableSortedSet<OutputArtifact>`   `outputs`    
          `protected BuildTarget`                                                    `owner`      

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                                                                                                                                                                                                                                  Description
          -------------- -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `protected `   `AbstractAction​(ActionRegistry registry,               com.google.common.collect.ImmutableSortedSet<Artifact> inputs,               com.google.common.collect.ImmutableSortedSet<OutputArtifact> outputs,               String shortName)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                Method                     Description
          ---------------------------------------------------------------- -------------------------- -------------
          `BuildTarget`                                                    `getBuildTarget()`          
          `com.google.common.collect.ImmutableSet<BuildTarget>`            `getDependencies()`         
          `String`                                                         `getID()`                   
          `com.google.common.collect.ImmutableSortedSet<Artifact>`         `getInputs()`               
          `com.google.common.collect.ImmutableSortedSet<OutputArtifact>`   `getOutputs()`              
          `BuildTarget`                                                    `getOwner()`                
          `String`                                                         `getShortName()`            
          `com.google.common.collect.ImmutableSortedSet<SourcePath>`       `getSourcePathOutputs()`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.actions.Action}

            ### Methods inherited from interface com.facebook.buck.core.rules.actions.[Action](Action.html "interface in com.facebook.buck.core.rules.actions")

            `execute, isCacheable, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#owner}

        -   #### owner

                protected final BuildTarget owner

        []{#inputs}

        -   #### inputs

                protected final com.google.common.collect.ImmutableSortedSet<Artifact> inputs

        []{#outputs}

        -   #### outputs

                protected final com.google.common.collect.ImmutableSortedSet<OutputArtifact> outputs
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.rules.actions.ActionRegistry,com.google.common.collect.ImmutableSortedSet,com.google.common.collect.ImmutableSortedSet,java.lang.String)}

        -   #### AbstractAction

                protected AbstractAction​(ActionRegistry registry,
                                         com.google.common.collect.ImmutableSortedSet<Artifact> inputs,
                                         com.google.common.collect.ImmutableSortedSet<OutputArtifact> outputs,
                                         String shortName)

            [Parameters:]{.paramLabel}
            :   `registry` - the
                [`DefaultActionRegistry`](DefaultActionRegistry.html "class in com.facebook.buck.core.rules.actions")
                to registry this action for.
            :   `inputs` - the input
                [`Artifact`](../../artifact/Artifact.html "interface in com.facebook.buck.core.artifact")
                for this
                [`Action`](Action.html "interface in com.facebook.buck.core.rules.actions").
                They can be either outputs of other
                [`Action`](Action.html "interface in com.facebook.buck.core.rules.actions")s
                or be source files
            :   `outputs` - the outputs for this
                [`Action`](Action.html "interface in com.facebook.buck.core.rules.actions")
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getOwner()}

        -   #### getOwner

            ``` methodSignature
            public final BuildTarget getOwner()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getOwner` in interface `Action`

            [Returns:]{.returnLabel}
            :   the build target of the rule analysis that created of
                this action

        []{#getInputs()}

        -   #### getInputs

            ``` methodSignature
            public final com.google.common.collect.ImmutableSortedSet<Artifact> getInputs()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getInputs` in interface `Action`

            [Returns:]{.returnLabel}
            :   the set of inputs required to complete this action

        []{#getOutputs()}

        -   #### getOutputs

            ``` methodSignature
            public final com.google.common.collect.ImmutableSortedSet<OutputArtifact> getOutputs()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getOutputs` in interface `Action`

            [Returns:]{.returnLabel}
            :   the set of outputs this action generates

        []{#getSourcePathOutputs()}

        -   #### getSourcePathOutputs

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<SourcePath> getSourcePathOutputs()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourcePathOutputs` in interface `Action`

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourcePathOutputs` in interface `BuildEngineAction`

            [Returns:]{.returnLabel}
            :   the set of outputs this
                [`BuildEngineAction`](../../build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action")
                builds. This is here for legacy as BuildRules deal with
                [`SourcePath`](../../sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")

        []{#getShortName()}

        -   #### getShortName

            ``` methodSignature
            public final String getShortName()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getShortName` in interface `Action`

            [Returns:]{.returnLabel}
            :   a name for this action to be printed to console when
                executing and for logging purposes

        []{#getID()}

        -   #### getID

            ``` methodSignature
            public final String getID()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getID` in interface `Action`

            [Returns:]{.returnLabel}
            :   the short name of this action as an ID

        []{#getBuildTarget()}

        -   #### getBuildTarget

            ``` methodSignature
            public BuildTarget getBuildTarget()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildTarget` in interface `BuildEngineAction`

            [Returns:]{.returnLabel}
            :   the
                [`BuildTarget`](../../model/BuildTarget.html "class in com.facebook.buck.core.model")
                of the rule corresponding to this action

        []{#getDependencies()}

        -   #### getDependencies

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<BuildTarget> getDependencies()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDependencies` in interface `BuildEngineAction`

            [Returns:]{.returnLabel}
            :   a set of dependencies required for this
                [`BuildEngineAction`](../../build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action")
                to build, as identified by the
                [`BuildTarget`](../../model/BuildTarget.html "class in com.facebook.buck.core.model").
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

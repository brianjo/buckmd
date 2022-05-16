/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.rules} /\*\*\*/ {template .soyweb} {call buck.header} {param title:
\'Adding Custom Rules to Buck\' /} {param navid: \'extending_rules\' /}
{param description} This isn\'t currently possible at this time unless
you fork Buck. If you do fork Buck, this is how you can add new rules.
Once you\'ve followed these steps, we\'d love a pull request! {/param}
{/call}

::: {.{css .overview}}
As of the writing of this document, the only official way to add rules
to Buck is to fork the project and modify the source. We will, at some
point, construct a beautiful and elegant extensions API. Until then,
you\'ll want to have the documentation of our internal{sp}
[API](%7BROOT%7Djavadoc/) handy, and then\...

Start by editing `KnownBuildRuleTypes`. You\'ll need to edit
{sp}`createBuilder()` and find the block where there are a large number
of calls to `builder.register()`.

``` {.prettyprint .lang-java}
  builder.register(new YourDescription());
```

What is `YourDescription`? It\'s an implementation of the
[`Description`](https://buck.build/javadoc/com/facebook/buck/core/description/Description.html)
{sp}interface. This interface serves three roles in Buck:

1.  It provides the name for the rule type, eg. `java_library`
2.  It makes clear the parameters which are accepted by a rule
3.  It acts as a factory of
    [`BuildRule`](https://buck.build/javadoc/com/facebook/buck/rules/BuildRule.html)
    {sp}instances.

### Defining Rule Parameters

This is done by implementing
{sp}`Description.createUnpopulatedConstructorArg()`. This should return
a java object, the public fields of which are the camelCased names of
the parameters used by the rule in BUCK files. When referenced in BUCK
files, the field name is snake_cased. That is \"someParam\" would become
\"some_param\".

You may use primitives, enums, generic types, collections (including
generic collections), and custom types for the fields of the constructor
arg. If you are using a custom type which Buck does not know how to
marshal from JSON, then you must implement a
[`TypeCoercer`](https://buck.build/javadoc/com/facebook/buck/rules/coercer/TypeCoercer.html).
How to do this is beyond the scope of this doc.

Note: if a parameter might either be a local file or an output of a
{sp}`BuildRule`, then you can use a
[`SourcePath`](https://buck.build/javadoc/com/facebook/buck/rules/SourcePath.html)
to represent that parameter.

If a parmater is considered to be optional, then the field should be
declared using Guava\'s `Optional` class (eg.
`public Optional<String> name;`)

### Constructing new BuildRule instances

When Buck needs to construct a `BuildRule` it will call
{sp}`Description.createBuildRule()`, passing in a populated constructor
arg. Collection types on that arg will have been instantiated with an
empty collection, even if they are declared as being optional.

The `createBuildRule` method is responsible for returning an
instantiated `BuildRule` that can be used to construct whatever it is
that we\'re adding this build rule for. The current instances typically
inherit from
[`AbstractBuildRule`](https://buck.build/javadoc/com/facebook/buck/rules/AbstractBuildRule.html),
and we suggest you do so too.

The created `BuildRule` will be registered with the
{sp}`BuildRuleResolver` automatically. There are, however, plenty of
cases where a `BuildRule` will want to depend on existing functionality
that\'s already expressed as a {sp}`BuildRule`. In this case, it\'s fine
to create that intermediate rule in the `createBuildRule()` method, add
it to the resolver, and then add that newly created rule as a dependency
of the one ultimately returned from the method. The only caveat: each
rule must have its own, unique, `BuildTarget`, which is the name by
which it\'s referred to in the action graph.

You are strongly encouraged to delay doing any work in your
{sp}`BuildRule` until the `getBuildSteps()`{sp} method. In particular,
don\'t do any work other than assigning fields in the constructor! The
exception to this is working out the path to the output of your rule.

You can think of a `Description` as a factory of {sp}`BuildRule`
instances. Similarly, you can think of a {sp}`BuildRule` as a factory of
[`Step`s](https://buck.build/javadoc/com/facebook/buck/step/Step.html)
{sp}that must be executed in order to create a specific output. Unlike
rules, steps are executed sequentially in the order in which they are
returned.

### Ensuring Your Rule Is Rebuilt Correctly

If your rule extends `AbstractBuildRule`, then it\'s enough to simply
annotate any field on that rule that contributes to its uniqueness with
[`@AddToRuleKey`](https://buck.build/javadoc/com/facebook/buck/rules/AddToRuleKey.html).
This is used by Buck to calculate the rule key, which, if the value
changes between builds, will cause Buck to re-execute your
{sp}`BuildRule`.

Another tip for ensuring your rule rebuilds correctly between builds is
to ensure that the output directory is cleaned each time. Commonly,
you\'ll see the first steps of a rule are something like:

``` {.prettyprint .lang-java}
  // a "gen" path is where the ultimate outputs of a rule live.
  Path outputDir = BuildTargets.getGenPath(target, "%s-output");

  // Or, if the path to the output has been calculated in the constructor
  // Path outputDir = outputPath.getParent();

  steps.add(new MakeCleanDirectoryStep(outputDir));
```

In your IDE, take a look at the key interfaces and classes to discover
more about what you can do within Buck:

-   [`Description`](https://buck.build/javadoc/com/facebook/buck/rules/Description.html)
-   [`AbstractBuildRule`](https://buck.build/javadoc/com/facebook/buck/rules/AbstractBuildRule.html)
-   [`Step`](https://buck.build/javadoc/com/facebook/buck/step/Step.html)
:::

// close overview {call buck.footer} {param navid: \'extending_rules\'
/} {/call} {/template}

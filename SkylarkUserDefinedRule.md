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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.core.starlark.rule](package-summary.html)
:::

## Class SkylarkUserDefinedRule {#class-skylarkuserdefinedrule .title title="Class SkylarkUserDefinedRule"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.google.devtools.build.lib.syntax.BaseFunction

    -   -   com.facebook.buck.core.starlark.rule.SkylarkUserDefinedRule

::: description
-   

    All Implemented Interfaces:
    :   `com.google.devtools.build.lib.packages.SkylarkExportable`,
        `com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable`,
        `com.google.devtools.build.lib.skylarkinterface.SkylarkValue`,
        `com.google.devtools.build.lib.syntax.StarlarkFunction`

    ------------------------------------------------------------------------

        public class SkylarkUserDefinedRule
        extends com.google.devtools.build.lib.syntax.BaseFunction
        implements com.google.devtools.build.lib.packages.SkylarkExportable

    ::: block
    The `BaseFunction` that is returned by \`rule()\`. Accepts
    user-specified parameters, and adds invocations to the parse
    context. Type checking is done with coercion later; it is not
    checked in this class.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.google.devtools.build.lib.syntax.BaseFunction}

            ### Fields inherited from class com.google.devtools.build.lib.syntax.BaseFunction

            `enforcedArgumentTypes, location, objectType, paramDoc, signature`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `protected Object`    | `call​(Object[] ar     |                       |
        |                       | gs,     com.google.de |                       |
        |                       | vtools.build.lib.synt |                       |
        |                       | ax.FuncallExpression  |                       |
        |                       | ast,     com.google.d |                       |
        |                       | evtools.build.lib.syn |                       |
        |                       | tax.Environment env)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `export​(com           |                       |
        |                       | .google.devtools.buil |                       |
        |                       | d.lib.cmdline.Label e |                       |
        |                       | xtensionLabel,        |                       |
        |                       | String exportedName)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common.   | `getAllParamInfo()`   | ::: block             |
        | collect.ImmutableMap< |                       | Get ParamInfo objects |
        | String,​ParamInfo<?>>` |                       | for all of the        |
        |                       |                       | [`At                  |
        |                       |                       | tribute`](attr/Attrib |
        |                       |                       | ute.html "class in co |
        |                       |                       | m.facebook.buck.core. |
        |                       |                       | starlark.rule.attr")s |
        |                       |                       | provided to this      |
        |                       |                       | instance              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common.   | `getAttrs()`          | ::: block             |
        | collect.ImmutableMap< |                       | The attributes that   |
        | String,​Attribute<?>>` |                       | this function accepts |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getExportedName()`   | ::: block             |
        |                       |                       | Get the exported name |
        |                       |                       | of the function       |
        |                       |                       | within an extension   |
        |                       |                       | file.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Set<String>`         | `getHidden            |                       |
        |                       | ImplicitAttributes()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `co                   | `getLabel()`          | ::: block             |
        | m.google.devtools.bui |                       | Get the string        |
        | ld.lib.cmdline.Label` |                       | representation of the |
        |                       |                       | label of extension    |
        |                       |                       | file.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getName()`           | ::: block             |
        |                       |                       | Ensure that we only   |
        |                       |                       | get our name after    |
        |                       |                       | this function has     |
        |                       |                       | been exported         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isExported()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Sk            | `of​(com.goog          | ::: block             |
        | ylarkUserDefinedRule` | le.devtools.build.lib | Create an instance of |
        |                       | .events.Location loca | [`SkylarkUserDefine   |
        |                       | tion,   com.google.de | dRule`](SkylarkUserDe |
        |                       | vtools.build.lib.synt | finedRule.html "class |
        |                       | ax.BaseFunction imple |  in com.facebook.buck |
        |                       | mentation,   com.goog | .core.starlark.rule") |
        |                       | le.common.collect.Imm | :::                   |
        |                       | utableMap<String,​Attr |                       |
        |                       | ibute<?>> implicitAtt |                       |
        |                       | ributes,   Set<String |                       |
        |                       | > hiddenImplicitAttri |                       |
        |                       | butes,   Map<String,​A |                       |
        |                       | ttributeHolder> attrs |                       |
        |                       | ,   boolean inferRunI |                       |
        |                       | nfo,   boolean test)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `shouldBeTestRule()`  | ::: block             |
        |                       |                       | Whether this rule is  |
        |                       |                       | expected to be a test |
        |                       |                       | rule or not           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `                     | ::: block             |
        |                       | shouldInferRunInfo()` | Whether RunInfo       |
        |                       |                       | should be inferred    |
        |                       |                       | for this rule         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          | ::: block             |
        |                       |                       | Override the built-in |
        |                       |                       | signature printer, as |
        |                       |                       | it prints out \'\*\'  |
        |                       |                       | unconditionally if    |
        |                       |                       | all arguments are     |
        |                       |                       | kwargs                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.google.devtools.build.lib.syntax.BaseFunction}

            ### Methods inherited from class com.google.devtools.build.lib.syntax.BaseFunction

            `call, callWithArgArray, canonicalizeArguments, configure, configure, getArgArraySize, getEnforcedArgumentTypes, getFullName, getLocation, getObjectType, getObjectTypeString, getOrCreateChildEnvironment, getParamDoc, getShortSignature, getSignature, hasSelfArgument, isConfigured, isImmutable, printTypeString, processArguments, repr`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable}

            ### Methods inherited from interface com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable

            `debugPrint, repr, str`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.google.devtools.build.lib.skylarkinterface.SkylarkValue}

            ### Methods inherited from interface com.google.devtools.build.lib.skylarkinterface.SkylarkValue

            `isHashable, isImmutable`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#call(java.lang.Object[],com.google.devtools.build.lib.syntax.FuncallExpression,com.google.devtools.build.lib.syntax.Environment)}

        -   #### call

            ``` methodSignature
            protected Object call​(Object[] args,
                                  @Nullable
                                  com.google.devtools.build.lib.syntax.FuncallExpression ast,
                                  com.google.devtools.build.lib.syntax.Environment env)
                           throws com.google.devtools.build.lib.syntax.EvalException,
                                  InterruptedException
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `call` in
                class `com.google.devtools.build.lib.syntax.BaseFunction`

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`
            :   `InterruptedException`

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            ::: block
            Override the built-in signature printer, as it prints out
            \'\*\' unconditionally if all arguments are kwargs
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in
                class `com.google.devtools.build.lib.syntax.BaseFunction`

        []{#of(com.google.devtools.build.lib.events.Location,com.google.devtools.build.lib.syntax.BaseFunction,com.google.common.collect.ImmutableMap,java.util.Set,java.util.Map,boolean,boolean)}

        -   #### of

            ``` methodSignature
            public static SkylarkUserDefinedRule of​(com.google.devtools.build.lib.events.Location location,
                                                    com.google.devtools.build.lib.syntax.BaseFunction implementation,
                                                    com.google.common.collect.ImmutableMap<String,​Attribute<?>> implicitAttributes,
                                                    Set<String> hiddenImplicitAttributes,
                                                    Map<String,​AttributeHolder> attrs,
                                                    boolean inferRunInfo,
                                                    boolean test)
                                             throws com.google.devtools.build.lib.syntax.EvalException
            ```

            ::: block
            Create an instance of
            [`SkylarkUserDefinedRule`](SkylarkUserDefinedRule.html "class in com.facebook.buck.core.starlark.rule")
            :::

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`

        []{#getName()}

        -   #### getName

            ``` methodSignature
            public String getName()
            ```

            ::: block
            Ensure that we only get our name after this function has
            been exported
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `getName` in
                class `com.google.devtools.build.lib.syntax.BaseFunction`

        []{#getLabel()}

        -   #### getLabel

            ``` methodSignature
            public com.google.devtools.build.lib.cmdline.Label getLabel()
            ```

            ::: block
            Get the string representation of the label of extension
            file. Only may be called after calling
            [`export(Label, String)`](#export(com.google.devtools.build.lib.cmdline.Label,java.lang.String))
            :::

            [Returns:]{.returnLabel}

        []{#getExportedName()}

        -   #### getExportedName

            ``` methodSignature
            public String getExportedName()
            ```

            ::: block
            Get the exported name of the function within an extension
            file. Only may be called after calling
            [`export(Label, String)`](#export(com.google.devtools.build.lib.cmdline.Label,java.lang.String))
            :::

        []{#shouldInferRunInfo()}

        -   #### shouldInferRunInfo

            ``` methodSignature
            public boolean shouldInferRunInfo()
            ```

            ::: block
            Whether RunInfo should be inferred for this rule
            :::

        []{#shouldBeTestRule()}

        -   #### shouldBeTestRule

            ``` methodSignature
            public boolean shouldBeTestRule()
            ```

            ::: block
            Whether this rule is expected to be a test rule or not
            :::

        []{#isExported()}

        -   #### isExported

            ``` methodSignature
            public boolean isExported()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isExported` in
                interface `com.google.devtools.build.lib.packages.SkylarkExportable`

        []{#export(com.google.devtools.build.lib.cmdline.Label,java.lang.String)}

        -   #### export

            ``` methodSignature
            public void export​(com.google.devtools.build.lib.cmdline.Label extensionLabel,
                               String exportedName)
                        throws com.google.devtools.build.lib.syntax.EvalException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `export` in
                interface `com.google.devtools.build.lib.packages.SkylarkExportable`

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`

        []{#getAttrs()}

        -   #### getAttrs

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​Attribute<?>> getAttrs()
            ```

            ::: block
            The attributes that this function accepts
            :::

        []{#getAllParamInfo()}

        -   #### getAllParamInfo

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​ParamInfo<?>> getAllParamInfo()
            ```

            ::: block
            Get ParamInfo objects for all of the
            [`Attribute`](attr/Attribute.html "class in com.facebook.buck.core.starlark.rule.attr")s
            provided to this instance
            :::

        []{#getHiddenImplicitAttributes()}

        -   #### getHiddenImplicitAttributes

            ``` methodSignature
            public Set<String> getHiddenImplicitAttributes()
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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::

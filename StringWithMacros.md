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
[Package]{.packageLabelInType} [com.facebook.buck.rules.macros](package-summary.html)
:::

## Class StringWithMacros {#class-stringwithmacros .title title="Class StringWithMacros"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.macros.StringWithMacros

::: description
-   

    All Implemented Interfaces:
    :   `StringMatcher`, `TargetTranslatable<StringWithMacros>`

    ------------------------------------------------------------------------

        public abstract class StringWithMacros
        extends Object
        implements TargetTranslatable<StringWithMacros>, StringMatcher

    ::: block
    A class representing a string containing ordered, embedded, strongly
    typed macros.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `boolean`             | `equals​(Object obj)`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `format               |                       |
        |                       | ​(java.util.function.F |                       |
        |                       | unction<? super Macro |                       |
        |                       | Container,​? extends C |                       |
        |                       | harSequence> mapper)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.com       | `getMacros()`         |                       |
        | mon.collect.Immutable |                       |                       |
        | List<MacroContainer>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract com.goog    | `getParts()`          | ::: block             |
        | le.common.collect.Imm |                       | The components of the |
        | utableList<Either<Str |                       | macro string.         |
        | ing,​MacroContainer>>` |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `<T> c                | `map​(jav              |                       |
        | om.google.common.coll | a.util.function.Funct |                       |
        | ect.ImmutableList<T>` | ion<? super String,​?  |                       |
        |                       | extends T> stringMapp |                       |
        |                       | er,    java.util.func |                       |
        |                       | tion.Function<? super |                       |
        |                       |  MacroContainer,​? ext |                       |
        |                       | ends T> macroMapper)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `StringWithMacros`    | `mapStrings​(java.util |                       |
        |                       | .function.Function<St |                       |
        |                       | ring,​String> mapper)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `matches​(String s)`   |                       |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `of​(com.google.comm   | ::: block             |
        | tic StringWithMacros` | on.collect.ImmutableL | String with macros is |
        |                       | ist<Either<String,​Mac | a sequence of strings |
        |                       | roContainer>> parts)` | and macros.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `ofConstantStrin      | ::: block             |
        | tic StringWithMacros` | g​(String singlePart)` | Create a string with  |
        |                       |                       | macros with a single  |
        |                       |                       | string without macros |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Option               | `translateTargets     |                       |
        | al<StringWithMacros>` | ​(CellNameResolver cel |                       |
        |                       | lPathResolver,        |                       |
        |                       |           BaseName ta |                       |
        |                       | rgetBaseName,         |                       |
        |                       |          TargetNodeTr |                       |
        |                       | anslator translator)` |                       |
        +-----------------------+-----------------------+-----------------------+

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

            `clone, finalize, getClass, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getParts()}

        -   #### getParts

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<Either<String,​MacroContainer>> getParts()
            ```

            ::: block
            The components of the macro string. Each part is either a
            plain string or a macro.
            :::

        []{#of(com.google.common.collect.ImmutableList)}

        -   #### of

            ``` methodSignature
            public static StringWithMacros of​(com.google.common.collect.ImmutableList<Either<String,​MacroContainer>> parts)
            ```

            ::: block
            String with macros is a sequence of strings and macros.
            Create it.
            :::

        []{#ofConstantString(java.lang.String)}

        -   #### ofConstantString

            ``` methodSignature
            public static StringWithMacros ofConstantString​(String singlePart)
            ```

            ::: block
            Create a string with macros with a single string without
            macros
            :::

        []{#getMacros()}

        -   #### getMacros

            ``` methodSignature
            public com.google.common.collect.ImmutableList<MacroContainer> getMacros()
            ```

            [Returns:]{.returnLabel}
            :   the list of all
                [`Macro`](Macro.html "interface in com.facebook.buck.rules.macros")s
                in the macro string.

        []{#map(java.util.function.Function,java.util.function.Function)}

        -   #### map

            ``` methodSignature
            public <T> com.google.common.collect.ImmutableList<T> map​(java.util.function.Function<? super String,​? extends T> stringMapper,
                                                                      java.util.function.Function<? super MacroContainer,​? extends T> macroMapper)
            ```

        []{#format(java.util.function.Function)}

        -   #### format

            ``` methodSignature
            public String format​(java.util.function.Function<? super MacroContainer,​? extends CharSequence> mapper)
            ```

            [Returns:]{.returnLabel}
            :   format the macro string into a
                [`String`](http://docs.oracle.com/javase/7/docs/api/java/lang/String.html?is-external=true "class or interface in java.lang"){.externalLink},
                using `mapper` to stringify the embedded
                [`Macro`](Macro.html "interface in com.facebook.buck.rules.macros")s.

        []{#mapStrings(java.util.function.Function)}

        -   #### mapStrings

            ``` methodSignature
            public StringWithMacros mapStrings​(java.util.function.Function<String,​String> mapper)
            ```

            [Returns:]{.returnLabel}
            :   a new
                [`StringWithMacros`](StringWithMacros.html "class in com.facebook.buck.rules.macros")
                with the string components transformed by
                `      mapper`.

        []{#translateTargets(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.core.model.BaseName,com.facebook.buck.versions.TargetNodeTranslator)}

        -   #### translateTargets

            ``` methodSignature
            public Optional<StringWithMacros> translateTargets​(CellNameResolver cellPathResolver,
                                                               BaseName targetBaseName,
                                                               TargetNodeTranslator translator)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `translateTargets` in
                interface `TargetTranslatable<StringWithMacros>`

            [Returns:]{.returnLabel}
            :   if any changes are required, return the translated
                object.

        []{#matches(java.lang.String)}

        -   #### matches

            ``` methodSignature
            public boolean matches​(String s)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `matches` in interface `StringMatcher`

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(Object obj)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `Object`

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `Object`
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

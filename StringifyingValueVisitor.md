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
[Package]{.packageLabelInType} [com.facebook.buck.rules.modern.impl](package-summary.html)
:::

## Class StringifyingValueVisitor {#class-stringifyingvaluevisitor .title title="Class StringifyingValueVisitor"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.modern.impl.StringifyingValueVisitor

::: description
-   

    All Implemented Interfaces:
    :   `ValueVisitor<RuntimeException>`

    ------------------------------------------------------------------------

        public class StringifyingValueVisitor
        extends Object
        implements ValueVisitor<RuntimeException>

    ::: block
    A ValueVisitor that can be used to construct a String representation
    of an object.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                                                   Description
          ------------------- ------------------------------------------------------- -------------
          `static class `     `StringifyingValueVisitor.ExcludeFromStringification`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                    Description
          ------------------------------ -------------
          `StringifyingValueVisitor()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                 Method                                                                                                                                                           Description
          --------------------------------- ---------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `String`                          `getValue()`                                                                                                                                                      
          `void`                            `visitBoolean​(Boolean value)`                                                                                                                                     
          `void`                            `visitByte​(Byte value)`                                                                                                                                           
          `void`                            `visitCharacter​(Character value)`                                                                                                                                 
          `void`                            `visitDouble​(Double value)`                                                                                                                                       
          `<T extends AddsToRuleKey>void`   `visitDynamic​(T value,             ClassInfo<T> classInfo)`                                                                                                       
          `<T> void`                        `visitField​(Field field,           T value,           ValueTypeInfo<T> valueTypeInfo,           List<Class<? extends CustomFieldBehaviorTag>> customBehavior)`    
          `void`                            `visitFloat​(Float value)`                                                                                                                                         
          `void`                            `visitInteger​(Integer value)`                                                                                                                                     
          `<T> void`                        `visitList​(com.google.common.collect.ImmutableList<T> value,          ValueTypeInfo<T> innerType)`                                                                
          `void`                            `visitLong​(Long value)`                                                                                                                                           
          `<K,​V>void`                       `visitMap​(com.google.common.collect.ImmutableMap<K,​V> value,         ValueTypeInfo<K> keyType,         ValueTypeInfo<V> valueType)`                               
          `<T> void`                        `visitNullable​(T value,              ValueTypeInfo<T> inner)`                                                                                                     
          `<T> void`                        `visitOptional​(Optional<T> value,              ValueTypeInfo<T> innerType)`                                                                                       
          `void`                            `visitOutputPath​(OutputPath value)`                                                                                                                               
          `void`                            `visitPath​(Path path)`                                                                                                                                            
          `<T> void`                        `visitSet​(com.google.common.collect.ImmutableSet<T> value,         ValueTypeInfo<T> innerType)`                                                                   
          `void`                            `visitShort​(Short value)`                                                                                                                                         
          `<K,​V>void`                       `visitSortedMap​(com.google.common.collect.ImmutableSortedMap<K,​V> value,               ValueTypeInfo<K> keyType,               ValueTypeInfo<V> valueType)`       
          `<T> void`                        `visitSortedSet​(com.google.common.collect.ImmutableSortedSet<T> value,               ValueTypeInfo<T> innerType)`                                                 
          `void`                            `visitSourcePath​(SourcePath value)`                                                                                                                               
          `void`                            `visitString​(String value)`                                                                                                                                       
          `void`                            `visitTargetConfiguration​(TargetConfiguration value)`                                                                                                             

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
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

        []{#<init>()}

        -   #### StringifyingValueVisitor

                public StringifyingValueVisitor()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#visitOutputPath(com.facebook.buck.rules.modern.OutputPath)}

        -   #### visitOutputPath

            ``` methodSignature
            public void visitOutputPath​(OutputPath value)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `visitOutputPath` in
                interface `ValueVisitor<RuntimeException>`

        []{#visitSourcePath(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### visitSourcePath

            ``` methodSignature
            public void visitSourcePath​(SourcePath value)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `visitSourcePath` in
                interface `ValueVisitor<RuntimeException>`

        []{#visitField(java.lang.reflect.Field,java.lang.Object,com.facebook.buck.rules.modern.ValueTypeInfo,java.util.List)}
        []{#visitField(java.lang.reflect.Field,T,com.facebook.buck.rules.modern.ValueTypeInfo,java.util.List)}

        -   #### visitField

            ``` methodSignature
            public <T> void visitField​(Field field,
                                       T value,
                                       ValueTypeInfo<T> valueTypeInfo,
                                       List<Class<? extends CustomFieldBehaviorTag>> customBehavior)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `visitField` in
                interface `ValueVisitor<RuntimeException>`

        []{#visitSet(com.google.common.collect.ImmutableSet,com.facebook.buck.rules.modern.ValueTypeInfo)}

        -   #### visitSet

            ``` methodSignature
            public <T> void visitSet​(com.google.common.collect.ImmutableSet<T> value,
                                     ValueTypeInfo<T> innerType)
                              throws RuntimeException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `visitSet` in interface `ValueVisitor<RuntimeException>`

            [Throws:]{.throwsLabel}
            :   `RuntimeException`

        []{#visitSortedSet(com.google.common.collect.ImmutableSortedSet,com.facebook.buck.rules.modern.ValueTypeInfo)}

        -   #### visitSortedSet

            ``` methodSignature
            public <T> void visitSortedSet​(com.google.common.collect.ImmutableSortedSet<T> value,
                                           ValueTypeInfo<T> innerType)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `visitSortedSet` in
                interface `ValueVisitor<RuntimeException>`

        []{#visitMap(com.google.common.collect.ImmutableMap,com.facebook.buck.rules.modern.ValueTypeInfo,com.facebook.buck.rules.modern.ValueTypeInfo)}

        -   #### visitMap

            ``` methodSignature
            public <K,​V> void visitMap​(com.google.common.collect.ImmutableMap<K,​V> value,
                                             ValueTypeInfo<K> keyType,
                                             ValueTypeInfo<V> valueType)
                                      throws RuntimeException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `visitMap` in interface `ValueVisitor<RuntimeException>`

            [Throws:]{.throwsLabel}
            :   `RuntimeException`

        []{#visitSortedMap(com.google.common.collect.ImmutableSortedMap,com.facebook.buck.rules.modern.ValueTypeInfo,com.facebook.buck.rules.modern.ValueTypeInfo)}

        -   #### visitSortedMap

            ``` methodSignature
            public <K,​V> void visitSortedMap​(com.google.common.collect.ImmutableSortedMap<K,​V> value,
                                                   ValueTypeInfo<K> keyType,
                                                   ValueTypeInfo<V> valueType)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `visitSortedMap` in
                interface `ValueVisitor<RuntimeException>`

        []{#visitList(com.google.common.collect.ImmutableList,com.facebook.buck.rules.modern.ValueTypeInfo)}

        -   #### visitList

            ``` methodSignature
            public <T> void visitList​(com.google.common.collect.ImmutableList<T> value,
                                      ValueTypeInfo<T> innerType)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `visitList` in
                interface `ValueVisitor<RuntimeException>`

        []{#visitOptional(java.util.Optional,com.facebook.buck.rules.modern.ValueTypeInfo)}

        -   #### visitOptional

            ``` methodSignature
            public <T> void visitOptional​(Optional<T> value,
                                          ValueTypeInfo<T> innerType)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `visitOptional` in
                interface `ValueVisitor<RuntimeException>`

        []{#visitNullable(java.lang.Object,com.facebook.buck.rules.modern.ValueTypeInfo)}
        []{#visitNullable(T,com.facebook.buck.rules.modern.ValueTypeInfo)}

        -   #### visitNullable

            ``` methodSignature
            public <T> void visitNullable​(@Nullable
                                          T value,
                                          ValueTypeInfo<T> inner)
                                   throws RuntimeException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `visitNullable` in
                interface `ValueVisitor<RuntimeException>`

            [Throws:]{.throwsLabel}
            :   `RuntimeException`

        []{#visitDynamic(com.facebook.buck.core.rulekey.AddsToRuleKey,com.facebook.buck.rules.modern.ClassInfo)}
        []{#visitDynamic(T,com.facebook.buck.rules.modern.ClassInfo)}

        -   #### visitDynamic

            ``` methodSignature
            public <T extends AddsToRuleKey> void visitDynamic​(T value,
                                                               ClassInfo<T> classInfo)
                                                        throws RuntimeException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `visitDynamic` in
                interface `ValueVisitor<RuntimeException>`

            [Throws:]{.throwsLabel}
            :   `RuntimeException`

        []{#visitString(java.lang.String)}

        -   #### visitString

            ``` methodSignature
            public void visitString​(String value)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `visitString` in
                interface `ValueVisitor<RuntimeException>`

        []{#visitCharacter(java.lang.Character)}

        -   #### visitCharacter

            ``` methodSignature
            public void visitCharacter​(Character value)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `visitCharacter` in
                interface `ValueVisitor<RuntimeException>`

        []{#visitBoolean(java.lang.Boolean)}

        -   #### visitBoolean

            ``` methodSignature
            public void visitBoolean​(Boolean value)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `visitBoolean` in
                interface `ValueVisitor<RuntimeException>`

        []{#visitByte(java.lang.Byte)}

        -   #### visitByte

            ``` methodSignature
            public void visitByte​(Byte value)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `visitByte` in
                interface `ValueVisitor<RuntimeException>`

        []{#visitShort(java.lang.Short)}

        -   #### visitShort

            ``` methodSignature
            public void visitShort​(Short value)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `visitShort` in
                interface `ValueVisitor<RuntimeException>`

        []{#visitInteger(java.lang.Integer)}

        -   #### visitInteger

            ``` methodSignature
            public void visitInteger​(Integer value)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `visitInteger` in
                interface `ValueVisitor<RuntimeException>`

        []{#visitLong(java.lang.Long)}

        -   #### visitLong

            ``` methodSignature
            public void visitLong​(Long value)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `visitLong` in
                interface `ValueVisitor<RuntimeException>`

        []{#visitFloat(java.lang.Float)}

        -   #### visitFloat

            ``` methodSignature
            public void visitFloat​(Float value)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `visitFloat` in
                interface `ValueVisitor<RuntimeException>`

        []{#visitDouble(java.lang.Double)}

        -   #### visitDouble

            ``` methodSignature
            public void visitDouble​(Double value)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `visitDouble` in
                interface `ValueVisitor<RuntimeException>`

        []{#visitTargetConfiguration(com.facebook.buck.core.model.TargetConfiguration)}

        -   #### visitTargetConfiguration

            ``` methodSignature
            public void visitTargetConfiguration​(TargetConfiguration value)
                                          throws RuntimeException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `visitTargetConfiguration` in
                interface `ValueVisitor<RuntimeException>`

            [Throws:]{.throwsLabel}
            :   `RuntimeException`

        []{#getValue()}

        -   #### getValue

            ``` methodSignature
            public String getValue()
            ```

        []{#visitPath(java.nio.file.Path)}

        -   #### visitPath

            ``` methodSignature
            public void visitPath​(Path path)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `visitPath` in
                interface `ValueVisitor<RuntimeException>`
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

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
[Package]{.packageLabelInType} [com.facebook.buck.rules.modern](package-summary.html)
:::

## Interface ValueVisitor\<E extends [Exception](http://docs.oracle.com/javase/7/docs/api/java/lang/Exception.html?is-external=true "class or interface in java.lang"){.externalLink}\> {#interface-valuevisitore-extends-exception .title title="Interface ValueVisitor"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `AbstractValueVisitor`, `DepsComputingVisitor`,
        `OutputPathVisitor`, `StringifyingValueVisitor`

    ------------------------------------------------------------------------

        public interface ValueVisitor<E extends Exception>

    ::: block
    A ValueVisitor can be used to visit all the values referenced from a
    Buildable. This can be used for things like deriving all the inputs
    or outputs.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                 Method                                                                                                                                                           Description
          --------------------------------- ---------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
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
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#visitList(com.google.common.collect.ImmutableList,com.facebook.buck.rules.modern.ValueTypeInfo)}

        -   #### visitList

            ``` methodSignature
            <T> void visitList​(com.google.common.collect.ImmutableList<T> value,
                               ValueTypeInfo<T> innerType)
                        throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#visitSet(com.google.common.collect.ImmutableSet,com.facebook.buck.rules.modern.ValueTypeInfo)}

        -   #### visitSet

            ``` methodSignature
            <T> void visitSet​(com.google.common.collect.ImmutableSet<T> value,
                              ValueTypeInfo<T> innerType)
                       throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#visitSortedSet(com.google.common.collect.ImmutableSortedSet,com.facebook.buck.rules.modern.ValueTypeInfo)}

        -   #### visitSortedSet

            ``` methodSignature
            <T> void visitSortedSet​(com.google.common.collect.ImmutableSortedSet<T> value,
                                    ValueTypeInfo<T> innerType)
                             throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#visitMap(com.google.common.collect.ImmutableMap,com.facebook.buck.rules.modern.ValueTypeInfo,com.facebook.buck.rules.modern.ValueTypeInfo)}

        -   #### visitMap

            ``` methodSignature
            <K,​V> void visitMap​(com.google.common.collect.ImmutableMap<K,​V> value,
                                      ValueTypeInfo<K> keyType,
                                      ValueTypeInfo<V> valueType)
                               throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#visitSortedMap(com.google.common.collect.ImmutableSortedMap,com.facebook.buck.rules.modern.ValueTypeInfo,com.facebook.buck.rules.modern.ValueTypeInfo)}

        -   #### visitSortedMap

            ``` methodSignature
            <K,​V> void visitSortedMap​(com.google.common.collect.ImmutableSortedMap<K,​V> value,
                                            ValueTypeInfo<K> keyType,
                                            ValueTypeInfo<V> valueType)
                                     throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#visitNullable(java.lang.Object,com.facebook.buck.rules.modern.ValueTypeInfo)}
        []{#visitNullable(T,com.facebook.buck.rules.modern.ValueTypeInfo)}

        -   #### visitNullable

            ``` methodSignature
            <T> void visitNullable​(@Nullable
                                   T value,
                                   ValueTypeInfo<T> inner)
                            throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#visitOptional(java.util.Optional,com.facebook.buck.rules.modern.ValueTypeInfo)}

        -   #### visitOptional

            ``` methodSignature
            <T> void visitOptional​(Optional<T> value,
                                   ValueTypeInfo<T> innerType)
                            throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#visitOutputPath(com.facebook.buck.rules.modern.OutputPath)}

        -   #### visitOutputPath

            ``` methodSignature
            void visitOutputPath​(OutputPath value)
                          throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#visitSourcePath(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### visitSourcePath

            ``` methodSignature
            void visitSourcePath​(SourcePath value)
                          throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#visitField(java.lang.reflect.Field,java.lang.Object,com.facebook.buck.rules.modern.ValueTypeInfo,java.util.List)}
        []{#visitField(java.lang.reflect.Field,T,com.facebook.buck.rules.modern.ValueTypeInfo,java.util.List)}

        -   #### visitField

            ``` methodSignature
            <T> void visitField​(Field field,
                                T value,
                                ValueTypeInfo<T> valueTypeInfo,
                                List<Class<? extends CustomFieldBehaviorTag>> customBehavior)
                         throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#visitDynamic(com.facebook.buck.core.rulekey.AddsToRuleKey,com.facebook.buck.rules.modern.ClassInfo)}
        []{#visitDynamic(T,com.facebook.buck.rules.modern.ClassInfo)}

        -   #### visitDynamic

            ``` methodSignature
            <T extends AddsToRuleKey> void visitDynamic​(T value,
                                                        ClassInfo<T> classInfo)
                                                 throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#visitPath(java.nio.file.Path)}

        -   #### visitPath

            ``` methodSignature
            void visitPath​(Path path)
                    throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#visitString(java.lang.String)}

        -   #### visitString

            ``` methodSignature
            void visitString​(String value)
                      throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#visitCharacter(java.lang.Character)}

        -   #### visitCharacter

            ``` methodSignature
            void visitCharacter​(Character value)
                         throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#visitBoolean(java.lang.Boolean)}

        -   #### visitBoolean

            ``` methodSignature
            void visitBoolean​(Boolean value)
                       throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#visitByte(java.lang.Byte)}

        -   #### visitByte

            ``` methodSignature
            void visitByte​(Byte value)
                    throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#visitShort(java.lang.Short)}

        -   #### visitShort

            ``` methodSignature
            void visitShort​(Short value)
                     throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#visitInteger(java.lang.Integer)}

        -   #### visitInteger

            ``` methodSignature
            void visitInteger​(Integer value)
                       throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#visitLong(java.lang.Long)}

        -   #### visitLong

            ``` methodSignature
            void visitLong​(Long value)
                    throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#visitFloat(java.lang.Float)}

        -   #### visitFloat

            ``` methodSignature
            void visitFloat​(Float value)
                     throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#visitDouble(java.lang.Double)}

        -   #### visitDouble

            ``` methodSignature
            void visitDouble​(Double value)
                      throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#visitTargetConfiguration(com.facebook.buck.core.model.TargetConfiguration)}

        -   #### visitTargetConfiguration

            ``` methodSignature
            void visitTargetConfiguration​(TargetConfiguration value)
                                   throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`
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

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

## Class AbstractValueVisitor\<E extends [Exception](http://docs.oracle.com/javase/7/docs/api/java/lang/Exception.html?is-external=true "class or interface in java.lang"){.externalLink}\> {#class-abstractvaluevisitore-extends-exception .title title="Class AbstractValueVisitor"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.modern.impl.AbstractValueVisitor\<E\>

::: description
-   

    All Implemented Interfaces:
    :   `ValueVisitor<E>`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `DepsComputingVisitor`, `OutputPathVisitor`

    ------------------------------------------------------------------------

        public abstract class AbstractValueVisitor<E extends Exception>
        extends Object
        implements ValueVisitor<E>

    ::: block
    An abstract implementation of ValueVisitor used for implementations
    that only care about some underlying non-composed types.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                Description
          -------------------------- -------------
          `AbstractValueVisitor()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
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
          `<T> void`                        `visitSet​(com.google.common.collect.ImmutableSet<T> value,         ValueTypeInfo<T> innerType)`                                                                   
          `void`                            `visitShort​(Short value)`                                                                                                                                         
          `protected abstract void`         `visitSimple​(Object value)`                                                                                                                                       
          `<K,​V>void`                       `visitSortedMap​(com.google.common.collect.ImmutableSortedMap<K,​V> value,               ValueTypeInfo<K> keyType,               ValueTypeInfo<V> valueType)`       
          `<T> void`                        `visitSortedSet​(com.google.common.collect.ImmutableSortedSet<T> value,               ValueTypeInfo<T> innerType)`                                                 
          `void`                            `visitString​(String value)`                                                                                                                                       
          `void`                            `visitTargetConfiguration​(TargetConfiguration value)`                                                                                                             

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.rules.modern.ValueVisitor}

            ### Methods inherited from interface com.facebook.buck.rules.modern.[ValueVisitor](../ValueVisitor.html "interface in com.facebook.buck.rules.modern")

            `visitOutputPath, visitPath, visitSourcePath`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### AbstractValueVisitor

                public AbstractValueVisitor()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#visitList(com.google.common.collect.ImmutableList,com.facebook.buck.rules.modern.ValueTypeInfo)}

        -   #### visitList

            ``` methodSignature
            public <T> void visitList​(com.google.common.collect.ImmutableList<T> value,
                                      ValueTypeInfo<T> innerType)
                               throws E extends Exception
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `visitList` in
                interface `ValueVisitor<E extends Exception>`

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#visitSet(com.google.common.collect.ImmutableSet,com.facebook.buck.rules.modern.ValueTypeInfo)}

        -   #### visitSet

            ``` methodSignature
            public <T> void visitSet​(com.google.common.collect.ImmutableSet<T> value,
                                     ValueTypeInfo<T> innerType)
                              throws E extends Exception
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `visitSet` in
                interface `ValueVisitor<E extends Exception>`

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#visitSortedSet(com.google.common.collect.ImmutableSortedSet,com.facebook.buck.rules.modern.ValueTypeInfo)}

        -   #### visitSortedSet

            ``` methodSignature
            public <T> void visitSortedSet​(com.google.common.collect.ImmutableSortedSet<T> value,
                                           ValueTypeInfo<T> innerType)
                                    throws E extends Exception
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `visitSortedSet` in
                interface `ValueVisitor<E extends Exception>`

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#visitMap(com.google.common.collect.ImmutableMap,com.facebook.buck.rules.modern.ValueTypeInfo,com.facebook.buck.rules.modern.ValueTypeInfo)}

        -   #### visitMap

            ``` methodSignature
            public <K,​V> void visitMap​(com.google.common.collect.ImmutableMap<K,​V> value,
                                             ValueTypeInfo<K> keyType,
                                             ValueTypeInfo<V> valueType)
                                      throws E extends Exception
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `visitMap` in
                interface `ValueVisitor<E extends Exception>`

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#visitSortedMap(com.google.common.collect.ImmutableSortedMap,com.facebook.buck.rules.modern.ValueTypeInfo,com.facebook.buck.rules.modern.ValueTypeInfo)}

        -   #### visitSortedMap

            ``` methodSignature
            public <K,​V> void visitSortedMap​(com.google.common.collect.ImmutableSortedMap<K,​V> value,
                                                   ValueTypeInfo<K> keyType,
                                                   ValueTypeInfo<V> valueType)
                                            throws E extends Exception
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `visitSortedMap` in
                interface `ValueVisitor<E extends Exception>`

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#visitOptional(java.util.Optional,com.facebook.buck.rules.modern.ValueTypeInfo)}

        -   #### visitOptional

            ``` methodSignature
            public <T> void visitOptional​(Optional<T> value,
                                          ValueTypeInfo<T> innerType)
                                   throws E extends Exception
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `visitOptional` in
                interface `ValueVisitor<E extends Exception>`

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#visitNullable(java.lang.Object,com.facebook.buck.rules.modern.ValueTypeInfo)}
        []{#visitNullable(T,com.facebook.buck.rules.modern.ValueTypeInfo)}

        -   #### visitNullable

            ``` methodSignature
            public <T> void visitNullable​(@Nullable
                                          T value,
                                          ValueTypeInfo<T> inner)
                                   throws E extends Exception
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `visitNullable` in
                interface `ValueVisitor<E extends Exception>`

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#visitField(java.lang.reflect.Field,java.lang.Object,com.facebook.buck.rules.modern.ValueTypeInfo,java.util.List)}
        []{#visitField(java.lang.reflect.Field,T,com.facebook.buck.rules.modern.ValueTypeInfo,java.util.List)}

        -   #### visitField

            ``` methodSignature
            public <T> void visitField​(Field field,
                                       T value,
                                       ValueTypeInfo<T> valueTypeInfo,
                                       List<Class<? extends CustomFieldBehaviorTag>> customBehavior)
                                throws E extends Exception
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `visitField` in
                interface `ValueVisitor<E extends Exception>`

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#visitDynamic(com.facebook.buck.core.rulekey.AddsToRuleKey,com.facebook.buck.rules.modern.ClassInfo)}
        []{#visitDynamic(T,com.facebook.buck.rules.modern.ClassInfo)}

        -   #### visitDynamic

            ``` methodSignature
            public <T extends AddsToRuleKey> void visitDynamic​(T value,
                                                               ClassInfo<T> classInfo)
                                                        throws E extends Exception
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `visitDynamic` in
                interface `ValueVisitor<E extends Exception>`

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#visitSimple(java.lang.Object)}

        -   #### visitSimple

            ``` methodSignature
            protected abstract void visitSimple​(Object value)
                                         throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#visitString(java.lang.String)}

        -   #### visitString

            ``` methodSignature
            public void visitString​(String value)
                             throws E extends Exception
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `visitString` in
                interface `ValueVisitor<E extends Exception>`

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#visitCharacter(java.lang.Character)}

        -   #### visitCharacter

            ``` methodSignature
            public void visitCharacter​(Character value)
                                throws E extends Exception
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `visitCharacter` in
                interface `ValueVisitor<E extends Exception>`

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#visitBoolean(java.lang.Boolean)}

        -   #### visitBoolean

            ``` methodSignature
            public void visitBoolean​(Boolean value)
                              throws E extends Exception
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `visitBoolean` in
                interface `ValueVisitor<E extends Exception>`

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#visitByte(java.lang.Byte)}

        -   #### visitByte

            ``` methodSignature
            public void visitByte​(Byte value)
                           throws E extends Exception
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `visitByte` in
                interface `ValueVisitor<E extends Exception>`

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#visitShort(java.lang.Short)}

        -   #### visitShort

            ``` methodSignature
            public void visitShort​(Short value)
                            throws E extends Exception
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `visitShort` in
                interface `ValueVisitor<E extends Exception>`

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#visitInteger(java.lang.Integer)}

        -   #### visitInteger

            ``` methodSignature
            public void visitInteger​(Integer value)
                              throws E extends Exception
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `visitInteger` in
                interface `ValueVisitor<E extends Exception>`

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#visitLong(java.lang.Long)}

        -   #### visitLong

            ``` methodSignature
            public void visitLong​(Long value)
                           throws E extends Exception
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `visitLong` in
                interface `ValueVisitor<E extends Exception>`

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#visitFloat(java.lang.Float)}

        -   #### visitFloat

            ``` methodSignature
            public void visitFloat​(Float value)
                            throws E extends Exception
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `visitFloat` in
                interface `ValueVisitor<E extends Exception>`

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#visitDouble(java.lang.Double)}

        -   #### visitDouble

            ``` methodSignature
            public void visitDouble​(Double value)
                             throws E extends Exception
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `visitDouble` in
                interface `ValueVisitor<E extends Exception>`

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#visitTargetConfiguration(com.facebook.buck.core.model.TargetConfiguration)}

        -   #### visitTargetConfiguration

            ``` methodSignature
            public void visitTargetConfiguration​(TargetConfiguration value)
                                          throws E extends Exception
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `visitTargetConfiguration` in
                interface `ValueVisitor<E extends Exception>`

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

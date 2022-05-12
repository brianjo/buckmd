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

## Interface ValueCreator\<E extends [Exception](http://docs.oracle.com/javase/7/docs/api/java/lang/Exception.html?is-external=true "class or interface in java.lang"){.externalLink}\> {#interface-valuecreatore-extends-exception .title title="Interface ValueCreator"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        public interface ValueCreator<E extends Exception>

    ::: block
    A ValueCreator can be used to create the values referenced from a
    Buildable. This is similar to ValueVisitor but returns a value
    instead of taking one. Used for deserialization.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                          Method                                                                                   Description
          ---------------------------------------------------------- ---------------------------------------------------------------------------------------- -------------
          `Boolean`                                                  `createBoolean()`                                                                         
          `Byte`                                                     `createByte()`                                                                            
          `Character`                                                `createCharacter()`                                                                       
          `Double`                                                   `createDouble()`                                                                          
          `AddsToRuleKey`                                            `createDynamic()`                                                                         
          `Float`                                                    `createFloat()`                                                                           
          `Integer`                                                  `createInteger()`                                                                         
          `<T> com.google.common.collect.ImmutableList<T>`           `createList​(ValueTypeInfo<T> innerType)`                                                  
          `Long`                                                     `createLong()`                                                                            
          `<K,​V>com.google.common.collect.ImmutableMap<K,​V>`         `createMap​(ValueTypeInfo<K> keyType,          ValueTypeInfo<V> valueType)`                
          `<T> T`                                                    `createNullable​(ValueTypeInfo<T> inner)`                                                  
          `<T> Optional<T>`                                          `createOptional​(ValueTypeInfo<T> innerType)`                                              
          `OutputPath`                                               `createOutputPath()`                                                                      
          `Path`                                                     `createPath()`                                                                            
          `<T> com.google.common.collect.ImmutableSet<T>`            `createSet​(ValueTypeInfo<T> innerType)`                                                   
          `Short`                                                    `createShort()`                                                                           
          `<K,​V>com.google.common.collect.ImmutableSortedMap<K,​V>`   `createSortedMap​(ValueTypeInfo<K> keyType,                ValueTypeInfo<V> valueType)`    
          `<T> com.google.common.collect.ImmutableSortedSet<T>`      `createSortedSet​(ValueTypeInfo<T> innerType)`                                             
          `SourcePath`                                               `createSourcePath()`                                                                      
          `<T> T`                                                    `createSpecial​(Class<T> valueClass,              Object... args)`                         
          `String`                                                   `createString()`                                                                          
          `TargetConfiguration`                                      `createTargetConfiguration()`                                                             

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

        []{#createDynamic()}

        -   #### createDynamic

            ``` methodSignature
            AddsToRuleKey createDynamic()
                                 throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#createList(com.facebook.buck.rules.modern.ValueTypeInfo)}

        -   #### createList

            ``` methodSignature
            <T> com.google.common.collect.ImmutableList<T> createList​(ValueTypeInfo<T> innerType)
                                                               throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#createSet(com.facebook.buck.rules.modern.ValueTypeInfo)}

        -   #### createSet

            ``` methodSignature
            <T> com.google.common.collect.ImmutableSet<T> createSet​(ValueTypeInfo<T> innerType)
                                                             throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#createSortedSet(com.facebook.buck.rules.modern.ValueTypeInfo)}

        -   #### createSortedSet

            ``` methodSignature
            <T> com.google.common.collect.ImmutableSortedSet<T> createSortedSet​(ValueTypeInfo<T> innerType)
                                                                         throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#createMap(com.facebook.buck.rules.modern.ValueTypeInfo,com.facebook.buck.rules.modern.ValueTypeInfo)}

        -   #### createMap

            ``` methodSignature
            <K,​V> com.google.common.collect.ImmutableMap<K,​V> createMap​(ValueTypeInfo<K> keyType,
                                                                                    ValueTypeInfo<V> valueType)
                                                                             throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#createSortedMap(com.facebook.buck.rules.modern.ValueTypeInfo,com.facebook.buck.rules.modern.ValueTypeInfo)}

        -   #### createSortedMap

            ``` methodSignature
            <K,​V> com.google.common.collect.ImmutableSortedMap<K,​V> createSortedMap​(ValueTypeInfo<K> keyType,
                                                                                                ValueTypeInfo<V> valueType)
                                                                                         throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#createNullable(com.facebook.buck.rules.modern.ValueTypeInfo)}

        -   #### createNullable

            ``` methodSignature
            @Nullable
            <T> T createNullable​(ValueTypeInfo<T> inner)
                          throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#createOptional(com.facebook.buck.rules.modern.ValueTypeInfo)}

        -   #### createOptional

            ``` methodSignature
            <T> Optional<T> createOptional​(ValueTypeInfo<T> innerType)
                                    throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#createOutputPath()}

        -   #### createOutputPath

            ``` methodSignature
            OutputPath createOutputPath()
                                 throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#createSourcePath()}

        -   #### createSourcePath

            ``` methodSignature
            SourcePath createSourcePath()
                                 throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#createPath()}

        -   #### createPath

            ``` methodSignature
            Path createPath()
                     throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#createString()}

        -   #### createString

            ``` methodSignature
            String createString()
                         throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#createCharacter()}

        -   #### createCharacter

            ``` methodSignature
            Character createCharacter()
                               throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#createBoolean()}

        -   #### createBoolean

            ``` methodSignature
            Boolean createBoolean()
                           throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#createByte()}

        -   #### createByte

            ``` methodSignature
            Byte createByte()
                     throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#createShort()}

        -   #### createShort

            ``` methodSignature
            Short createShort()
                       throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#createInteger()}

        -   #### createInteger

            ``` methodSignature
            Integer createInteger()
                           throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#createLong()}

        -   #### createLong

            ``` methodSignature
            Long createLong()
                     throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#createFloat()}

        -   #### createFloat

            ``` methodSignature
            Float createFloat()
                       throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#createDouble()}

        -   #### createDouble

            ``` methodSignature
            Double createDouble()
                         throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#createTargetConfiguration()}

        -   #### createTargetConfiguration

            ``` methodSignature
            TargetConfiguration createTargetConfiguration()
                                                   throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#createSpecial(java.lang.Class,java.lang.Object...)}

        -   #### createSpecial

            ``` methodSignature
            <T> T createSpecial​(Class<T> valueClass,
                                Object... args)
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

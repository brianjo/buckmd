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
[Package]{.packageLabelInType} [com.facebook.buck.util.concurrent](package-summary.html)
:::

## Class LinkedBlockingStack\<E\> {#class-linkedblockingstacke .title title="Class LinkedBlockingStack"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.concurrent.LinkedBlockingStack\<E\>

::: description
-   

    [Type Parameters:]{.paramLabel}
    :   `E` - Type of contained elements.

    ```{=html}
    <!-- -->
    ```

    All Implemented Interfaces:
    :   `Iterable<E>`, `Collection<E>`, `BlockingQueue<E>`, `Queue<E>`

    ------------------------------------------------------------------------

        public class LinkedBlockingStack<E>
        extends Object
        implements BlockingQueue<E>

    ::: block
    An implementation of
    [`BlockingQueue`](http://docs.oracle.com/javase/7/docs/api/java/util/concurrent/BlockingQueue.html?is-external=true "class or interface in java.util.concurrent"){.externalLink}
    interface returning elements in LIFO order.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor               Description
          ------------------------- -------------
          `LinkedBlockingStack()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                Description
          ------------------- --------------------------------------------------------------------- -------------
          `boolean`           `add​(E element)`                                                       
          `boolean`           `addAll​(Collection<? extends E> collection)`                           
          `void`              `clear()`                                                              
          `boolean`           `contains​(Object object)`                                              
          `boolean`           `containsAll​(Collection<?> collection)`                                
          `int`               `drainTo​(Collection<? super E> collection)`                            
          `int`               `drainTo​(Collection<? super E> collection,        int maxElements)`    
          `E`                 `element()`                                                            
          `boolean`           `isEmpty()`                                                            
          `Iterator<E>`       `iterator()`                                                           
          `boolean`           `offer​(E element)`                                                     
          `boolean`           `offer​(E element,      long timeout,      TimeUnit unit)`              
          `E`                 `peek()`                                                               
          `E`                 `poll()`                                                               
          `E`                 `poll​(long timeout,     TimeUnit unit)`                                
          `void`              `put​(E element)`                                                       
          `int`               `remainingCapacity()`                                                  
          `E`                 `remove()`                                                             
          `boolean`           `remove​(Object object)`                                                
          `boolean`           `removeAll​(Collection<?> collection)`                                  
          `boolean`           `retainAll​(Collection<?> collection)`                                  
          `int`               `size()`                                                               
          `E`                 `take()`                                                               
          `Object[]`          `toArray()`                                                            
          `<T> T[]`           `toArray​(T[] array)`                                                   

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
        -   []{#methods.inherited.from.class.java.util.Collection}

            ### Methods inherited from interface java.util.[Collection](http://docs.oracle.com/javase/7/docs/api/java/util/Collection.html?is-external=true "class or interface in java.util"){.externalLink}

            `equals, hashCode, parallelStream, removeIf, spliterator, stream, toArray`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Iterable}

            ### Methods inherited from interface java.lang.[Iterable](http://docs.oracle.com/javase/7/docs/api/java/lang/Iterable.html?is-external=true "class or interface in java.lang"){.externalLink}

            `forEach`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### LinkedBlockingStack

                public LinkedBlockingStack()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#add(java.lang.Object)} []{#add(E)}

        -   #### add

            ``` methodSignature
            public boolean add​(E element)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `add` in interface `BlockingQueue<E>`

            [Specified by:]{.overrideSpecifyLabel}
            :   `add` in interface `Collection<E>`

            [Specified by:]{.overrideSpecifyLabel}
            :   `add` in interface `Queue<E>`

        []{#offer(java.lang.Object)} []{#offer(E)}

        -   #### offer

            ``` methodSignature
            public boolean offer​(E element)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `offer` in interface `BlockingQueue<E>`

            [Specified by:]{.overrideSpecifyLabel}
            :   `offer` in interface `Queue<E>`

        []{#remove()}

        -   #### remove

            ``` methodSignature
            public E remove()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `remove` in interface `Queue<E>`

        []{#poll()}

        -   #### poll

            ``` methodSignature
            public E poll()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `poll` in interface `Queue<E>`

        []{#element()}

        -   #### element

            ``` methodSignature
            public E element()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `element` in interface `Queue<E>`

        []{#peek()}

        -   #### peek

            ``` methodSignature
            public E peek()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `peek` in interface `Queue<E>`

        []{#put(java.lang.Object)} []{#put(E)}

        -   #### put

            ``` methodSignature
            public void put​(E element)
                     throws InterruptedException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `put` in interface `BlockingQueue<E>`

            [Throws:]{.throwsLabel}
            :   `InterruptedException`

        []{#offer(java.lang.Object,long,java.util.concurrent.TimeUnit)}
        []{#offer(E,long,java.util.concurrent.TimeUnit)}

        -   #### offer

            ``` methodSignature
            public boolean offer​(E element,
                                 long timeout,
                                 TimeUnit unit)
                          throws InterruptedException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `offer` in interface `BlockingQueue<E>`

            [Throws:]{.throwsLabel}
            :   `InterruptedException`

        []{#take()}

        -   #### take

            ``` methodSignature
            public E take()
                   throws InterruptedException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `take` in interface `BlockingQueue<E>`

            [Throws:]{.throwsLabel}
            :   `InterruptedException`

        []{#poll(long,java.util.concurrent.TimeUnit)}

        -   #### poll

            ``` methodSignature
            public E poll​(long timeout,
                          TimeUnit unit)
                   throws InterruptedException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `poll` in interface `BlockingQueue<E>`

            [Throws:]{.throwsLabel}
            :   `InterruptedException`

        []{#remainingCapacity()}

        -   #### remainingCapacity

            ``` methodSignature
            public int remainingCapacity()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `remainingCapacity` in interface `BlockingQueue<E>`

        []{#remove(java.lang.Object)}

        -   #### remove

            ``` methodSignature
            public boolean remove​(Object object)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `remove` in interface `BlockingQueue<E>`

            [Specified by:]{.overrideSpecifyLabel}
            :   `remove` in interface `Collection<E>`

        []{#addAll(java.util.Collection)}

        -   #### addAll

            ``` methodSignature
            public boolean addAll​(Collection<? extends E> collection)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `addAll` in interface `Collection<E>`

        []{#clear()}

        -   #### clear

            ``` methodSignature
            public void clear()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `clear` in interface `Collection<E>`

        []{#retainAll(java.util.Collection)}

        -   #### retainAll

            ``` methodSignature
            public boolean retainAll​(Collection<?> collection)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `retainAll` in interface `Collection<E>`

        []{#removeAll(java.util.Collection)}

        -   #### removeAll

            ``` methodSignature
            public boolean removeAll​(Collection<?> collection)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `removeAll` in interface `Collection<E>`

        []{#containsAll(java.util.Collection)}

        -   #### containsAll

            ``` methodSignature
            public boolean containsAll​(Collection<?> collection)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `containsAll` in interface `Collection<E>`

        []{#size()}

        -   #### size

            ``` methodSignature
            public int size()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `size` in interface `Collection<E>`

        []{#isEmpty()}

        -   #### isEmpty

            ``` methodSignature
            public boolean isEmpty()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isEmpty` in interface `Collection<E>`

        []{#contains(java.lang.Object)}

        -   #### contains

            ``` methodSignature
            public boolean contains​(Object object)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `contains` in interface `BlockingQueue<E>`

            [Specified by:]{.overrideSpecifyLabel}
            :   `contains` in interface `Collection<E>`

        []{#iterator()}

        -   #### iterator

            ``` methodSignature
            public Iterator<E> iterator()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `iterator` in interface `Collection<E>`

            [Specified by:]{.overrideSpecifyLabel}
            :   `iterator` in interface `Iterable<E>`

        []{#toArray()}

        -   #### toArray

            ``` methodSignature
            public Object[] toArray()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `toArray` in interface `Collection<E>`

        []{#toArray(java.lang.Object[])} []{#toArray(T[])}

        -   #### toArray

            ``` methodSignature
            public <T> T[] toArray​(T[] array)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `toArray` in interface `Collection<E>`

        []{#drainTo(java.util.Collection)}

        -   #### drainTo

            ``` methodSignature
            public int drainTo​(Collection<? super E> collection)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `drainTo` in interface `BlockingQueue<E>`

        []{#drainTo(java.util.Collection,int)}

        -   #### drainTo

            ``` methodSignature
            public int drainTo​(Collection<? super E> collection,
                               int maxElements)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `drainTo` in interface `BlockingQueue<E>`
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

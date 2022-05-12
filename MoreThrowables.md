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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.util](package-summary.html)
:::

## Class MoreThrowables {#class-morethrowables .title title="Class MoreThrowables"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.MoreThrowables

::: description
-   

    ------------------------------------------------------------------------

        public class MoreThrowables
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static Throwable`    | `getInitialCause​(     | ::: block             |
        |                       | Throwable throwable)` | If throwable has a    |
        |                       |                       | non-empty cause,      |
        |                       |                       | returns throwable at  |
        |                       |                       | the bottom of the     |
        |                       |                       | stack.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `getThrowableOrigin​(  | ::: block             |
        |                       | Throwable throwable)` | Returns string        |
        |                       |                       | representing class,   |
        |                       |                       | method, filename and  |
        |                       |                       | line number that      |
        |                       |                       | throwable was thrown  |
        |                       |                       | from                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `propagateIfInterru   | ::: block             |
        |                       | pt​(Throwable thrown)` | Propagates an         |
        |                       |                       | [`InterruptedExceptio |
        |                       |                       | n`](http://docs.oracl |
        |                       |                       | e.com/javase/7/docs/a |
        |                       |                       | pi/java/lang/Interrup |
        |                       |                       | tedException.html?is- |
        |                       |                       | external=true "class  |
        |                       |                       | or interface in java. |
        |                       |                       | lang"){.externalLink} |
        |                       |                       | masquerading as       |
        |                       |                       | another `Throwable`.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static <X ex         | `throwIfAnyC          | ::: block             |
        | tends Throwable>void` | auseInstanceOf​(Throwa | Traverse exception    |
        |                       | ble throwable,        | chain by recursively  |
        |                       |                    Cl | calling `getCause()`  |
        |                       | ass<X> declaredType)` | and throws it if      |
        |                       |                       | there is any          |
        |                       |                       | exception found which |
        |                       |                       | is an instance of     |
        |                       |                       | `declaredType`.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static <X ex         | `throwIfInitialCause  | ::: block             |
        | tends Throwable>void` | InstanceOf​(Throwable  | Traverse exception    |
        |                       | throwable,            | chain by recursively  |
        |                       |                    Cl | calling `getCause()`  |
        |                       | ass<X> declaredType)` | and throws it if      |
        |                       |                       | initial exception     |
        |                       |                       | (the one at the       |
        |                       |                       | bottom of the stack)  |
        |                       |                       | is an instance of     |
        |                       |                       | `declaredType`.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
::: {.section role="region"}
[]{#method.detail}

### Method Detail

[]{#propagateIfInterrupt(java.lang.Throwable)}

-   #### propagateIfInterrupt

    ``` methodSignature
    public static void propagateIfInterrupt​(Throwable thrown)
                                     throws InterruptedException
    ```

    ::: block
    Propagates an
    [`InterruptedException`](http://docs.oracle.com/javase/7/docs/api/java/lang/InterruptedException.html?is-external=true "class or interface in java.lang"){.externalLink}
    masquerading as another `Throwable`.
    :::

    [Throws:]{.throwsLabel}
    :   `InterruptedException`

[]{#getInitialCause(java.lang.Throwable)}

-   #### getInitialCause

    ``` methodSignature
    public static Throwable getInitialCause​(Throwable throwable)
    ```

    ::: block
    If throwable has a non-empty cause, returns throwable at the bottom
    of the stack.
    :::

[]{#getThrowableOrigin(java.lang.Throwable)}

-   #### getThrowableOrigin

    ``` methodSignature
    public static String getThrowableOrigin​(Throwable throwable)
    ```

    ::: block
    Returns string representing class, method, filename and line number
    that throwable was thrown from
    :::

[]{#throwIfAnyCauseInstanceOf(java.lang.Throwable,java.lang.Class)}

#### throwIfAnyCauseInstanceOf

``` methodSignature
public static <X extends Throwable> void throwIfAnyCauseInstanceOf​(Throwable throwable,
                                                                   Class<X> declaredType)
                                                            throws X extends Throwable
```

::: block
Traverse exception chain by recursively calling `getCause()` and throws
it if there is any exception found which is an instance of
`declaredType`. Example usage:

       try {
         future.get()
       } catch (ExecutionException) {
         MoreThrowables.throwIfAnyCauseInstanceOf(t, BarException.class);
       }

    Throws:
    X extends Throwable








    throwIfInitialCauseInstanceOf
    public static <X extends Throwable> void throwIfInitialCauseInstanceOf​(Throwable throwable,
                                                                           Class<X> declaredType)
                                                                    throws X extends Throwable

::: block
Traverse exception chain by recursively calling `getCause()` and throws
it if initial exception (the one at the bottom of the stack) is an
instance of `declaredType`. Example usage:

       try {
         future.get()
       } catch (ExecutionException) {
         MoreThrowables.throwIfInitialCauseInstanceOf(t, BarException.class);
       }

    Throws:
    X extends Throwable


















    Skip navigation links




    Overview
    Package
    Class
    Tree
    Deprecated
    Index
    Help




    All Classes


    <!--
      allClassesLink = document.getElementById("allclasses_navbar_bottom");
      if(window==top) {
        allClassesLink.style.display = "block";
      }
      else {
        allClassesLink.style.display = "none";
      }
      //-->


    JavaScript is disabled on your browser.




    Summary: 
    Nested | 
    Field | 
    Constr | 
    Method


    Detail: 
    Field | 
    Constr | 
    Method
:::
:::
:::
:::
:::
:::

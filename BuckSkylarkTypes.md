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
[Package]{.packageLabelInType} [com.facebook.buck.core.starlark.compatible](package-summary.html)
:::

## Class BuckSkylarkTypes {#class-buckskylarktypes .title title="Class BuckSkylarkTypes"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.starlark.compatible.BuckSkylarkTypes

::: description
-   

    ------------------------------------------------------------------------

        public class BuckSkylarkTypes
        extends Object

    ::: block
    Container class for helper methods having to deal with Skylark
    types. e.g. list or map conversion utilities that supplement the
    built in helpers.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static Object`       | `asDeepI              | ::: block             |
        |                       | mmutable​(Object arg)` | Attempt to get a      |
        |                       |                       | deeply immutable      |
        |                       |                       | instance of a value   |
        |                       |                       | passed in from        |
        |                       |                       | Skylark               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `i                    | ::: block             |
        |                       | sImmutable​(Object o)` | Checks if a given     |
        |                       |                       | value is              |
        |                       |                       | \'Immutable\'.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Object`       | `skylarkValueFromNul  |                       |
        |                       | lable​(Object object)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `toJavaList​(com.googl | ::: block             |
        | atic <NonWildcardType | e.devtools.build.lib. | Validate that all     |
        | ,​DestType extends Non | syntax.SkylarkList<?> | objects are of a      |
        | WildcardType>com.goog |  list,           Clas | given type and return |
        | le.common.collect.Imm | s<NonWildcardType> el | an `ImmutableList`    |
        | utableList<DestType>` | ementClass,           | containing those      |
        |                       |  String description)` | objects.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `                     | ::: block             |
        |                       | validateKwargName​(com | Ensure that a name is |
        |                       | .google.devtools.buil | a valid kwarg/field   |
        |                       | d.lib.events.Location | identifier            |
        |                       |  location,            | :::                   |
        |                       |        String kwarg)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Object`       | `validateNoneOrTy     | ::: block             |
        |                       | pe​(com.google.devtool | Check that a value is |
        |                       | s.build.lib.events.Lo | either `Runtime.NONE` |
        |                       | cation location,      | or an instance of     |
        |                       |               Class<? | `clazz`               |
        |                       | > clazz,              | :::                   |
        |                       |       Object object)` |                       |
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
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#toJavaList(com.google.devtools.build.lib.syntax.SkylarkList,java.lang.Class,java.lang.String)}

        -   #### toJavaList

            ``` methodSignature
            public static <NonWildcardType,​DestType extends NonWildcardType> com.google.common.collect.ImmutableList<DestType> toJavaList​(com.google.devtools.build.lib.syntax.SkylarkList<?> list,
                                                                                                                                                Class<NonWildcardType> elementClass,
                                                                                                                                                @Nullable
                                                                                                                                                String description)
                                                                                                                                         throws com.google.devtools.build.lib.syntax.EvalException
            ```

            ::: block
            Validate that all objects are of a given type and return an
            `ImmutableList` containing those objects.
            This is a workaround for
            `SkylarkList.getContents(Class, String)` being unable to
            handle generic types correctly. e.g. it is currently
            impossible to do:

                 SkylarkList<?> skyList = // Provided by user
                 // Works, but compiler complains because Provider is not specialized
                 ImmutableList<Provider> providers = skyList.getContents(Provider.class, null));
                 // Does not work because Provider.class != the class of Provider<?>
                 ImmutableList<Provider<?>> providers = skyList.getContents(Provider.class, null));
                 

            This function makes the following usage possible
                 SkylarkList<?> skyList = // Provided by user
                 ImmutableList<Provider<?>> providers = BuckSkylarkTypes.toJavaList(skyList, Provider.class, null));
                 

            This function wraps a dirty type cast up and tries to apply
            some basic type boundaries to reduce the likelihood of
            creating a foot gun.
            :::

            [Type Parameters:]{.paramLabel}
            :   `NonWildcardType` - The non-wildcard type. e.g.
                `Provider.class`
            :   `DestType` - The type of the elements in the resulting
                container. This can be either the same as
                `NonWildcardType`, or a generic type like `Provider<?>`

            [Parameters:]{.paramLabel}
            :   `list` - The list of objects to validate
            :   `elementClass` - The non-wildcard version of the desired
                final class
            :   `description` - a description of the argument being
                converted, or null, for debugging

            [Returns:]{.returnLabel}
            :   A list of `DestType`. This is immutable because we do
                some type casting under the hood, and do not want any
                assumptions to be made about the backing store of the
                container, nor do we want users to assume they can
                safely insert into that list.

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException` -
                If one of the elements was not of the type specified in
                `      elementClass`

        []{#asDeepImmutable(java.lang.Object)}

        -   #### asDeepImmutable

            ``` methodSignature
            public static Object asDeepImmutable​(Object arg)
                                          throws MutableObjectException
            ```

            ::: block
            Attempt to get a deeply immutable instance of a value passed
            in from Skylark
            Note that if mutable objects are passed in (namely
            `SkylarkList` or `SkylarkDict`, a copy may be made to get an
            immutable instance. This may happen in very deeply nested
            structures, so the runtime is variable based on how mutable
            the objects are. For the best performance, only immutable
            structures should be passed in, as that turns into a simple
            identity function.
            :::

            [Parameters:]{.paramLabel}
            :   `arg` - A value from the skylark interpreter. This
                should only be primitive objects, or `SkylarkValue`
                instances

            [Returns:]{.returnLabel}
            :   The original object if it was already an immutable
                `SkylarkValue` or a primitive value
                an immutable `SkylarkList` if the original object is a
                `SkylarkList` and all values were immutable or could be
                made immutable. As above, this may be a copy, or inner
                elements may have had to be copied if they were mutable
                An immutable `SkylarkDict` if the original object is a
                `SkylarkDict` and all keys and values were immutable, or
                could be made so. Again, note that copies may be made in
                order to make mutable objects immutable

            [Throws:]{.throwsLabel}
            :   `MutableObjectException` - If a nested or top level
                object was mutable, and could not be made immutable.
                This generally only applies to incorrectly implemented
                native data types that are exported to Skylark.

        []{#validateKwargName(com.google.devtools.build.lib.events.Location,java.lang.String)}

        -   #### validateKwargName

            ``` methodSignature
            public static void validateKwargName​(com.google.devtools.build.lib.events.Location location,
                                                 String kwarg)
                                          throws com.google.devtools.build.lib.syntax.EvalException
            ```

            ::: block
            Ensure that a name is a valid kwarg/field identifier
            This is useful as Skylark does not validate these by default
            when creating a signature
            :::

            [Parameters:]{.paramLabel}
            :   `location` - location of the kwarg currently being
                evaluated
            :   `kwarg` - the name of a kwarg / field

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`

        []{#skylarkValueFromNullable(java.lang.Object)}

        -   #### skylarkValueFromNullable

            ``` methodSignature
            public static Object skylarkValueFromNullable​(@Nullable
                                                          Object object)
            ```

            [Returns:]{.returnLabel}
            :   `None` if `object` is `null`, else return `object`. This
                is just a central place ot make sure things we return
                from internal implementations into Skylark are properly
                turned into None

        []{#validateNoneOrType(com.google.devtools.build.lib.events.Location,java.lang.Class,java.lang.Object)}

        -   #### validateNoneOrType

            ``` methodSignature
            public static Object validateNoneOrType​(com.google.devtools.build.lib.events.Location location,
                                                    Class<?> clazz,
                                                    Object object)
                                             throws com.google.devtools.build.lib.syntax.EvalException
            ```

            ::: block
            Check that a value is either `Runtime.NONE` or an instance
            of `clazz`
            :::

            [Parameters:]{.paramLabel}
            :   `location` - location of evaluation
            :   `clazz` - the class that the object should be an
                instance of if not `Runtime.NONE`
            :   `object` - the object to check

            [Returns:]{.returnLabel}
            :   the original value if it is of a correct type

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException` -
                if the object is not of the correct type

        []{#isImmutable(java.lang.Object)}

        -   #### isImmutable

            ``` methodSignature
            public static boolean isImmutable​(Object o)
            ```

            ::: block
            Checks if a given value is \'Immutable\'. This mostly works
            like `EvalUtils.isImmutable(java.lang.Object)`, but it can
            also handle `ImmutableCollection` and `ImmutableMap`
            :::
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

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
-   Package
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

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
# Package com.facebook.buck.core.exceptions {#package-com.facebook.buck.core.exceptions .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [Depe                             | ::: block                         |
    | ndencyStack.Element](DependencySt | Marker interface for stack trace  |
    | ack.Element.html "interface in co | elements.                         |
    | m.facebook.buck.core.exceptions") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [DependencyStack.Prov             | ::: block                         |
    | idesElement](DependencyStack.Prov | Types which have something to be  |
    | idesElement.html "interface in co | stored in stack trace             |
    | m.facebook.buck.core.exceptions") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ExceptionWithContext](Exception  |                                   |
    | WithContext.html "interface in co |                                   |
    | m.facebook.buck.core.exceptions") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ExceptionWithHumanReadab         |                                   |
    | leMessage](ExceptionWithHumanRead |                                   |
    | ableMessage.html "interface in co |                                   |
    | m.facebook.buck.core.exceptions") |                                   |
    +-----------------------------------+-----------------------------------+
    | [WrapsException](Wra              | ::: block                         |
    | psException.html "interface in co | This interface indicates that an  |
    | m.facebook.buck.core.exceptions") | exception is just used to wrap    |
    |                                   | another and isn\'t the true root  |
    |                                   | cause of the problem.             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [DependencyStack](                | ::: block                         |
    | DependencyStack.html "class in co | Stack-trace for providing better  |
    | m.facebook.buck.core.exceptions") | diagnostics when working with     |
    |                                   | dependency graph.                 |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [HumanReadableExc                 | ::: block                         |
    | eptionAugmentor](HumanReadableExc | A class that can append           |
    | eptionAugmentor.html "class in co | additional information to a       |
    | m.facebook.buck.core.exceptions") | HumanReadableException based on   |
    |                                   | configuration settings.           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [                                 | ::: block                         |
    | HumanReadableExceptions](HumanRea | Utilities to work with            |
    | dableExceptions.html "class in co | [                                 |
    | m.facebook.buck.core.exceptions") | `HumanReadableException`](HumanRe |
    |                                   | adableException.html "class in co |
    |                                   | m.facebook.buck.core.exceptions") |
    |                                   | and                               |
    |                                   | [`ExceptionWithHumanReadable      |
    |                                   | Message`](ExceptionWithHumanReada |
    |                                   | bleMessage.html "interface in com |
    |                                   | .facebook.buck.core.exceptions"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ThrowableCauseIterable](Throwab  | ::: block                         |
    | leCauseIterable.html "class in co | An iterable that uses an iterator |
    | m.facebook.buck.core.exceptions") | to traverse through all causes of |
    |                                   | given `throwable` by recursively  |
    |                                   | calling getCause() function.      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [UserVer                          | ::: block                         |
    | ify](UserVerify.html "class in co | Provides methods similar to       |
    | m.facebook.buck.core.exceptions") | `Verify` but throws               |
    |                                   | [                                 |
    |                                   | `HumanReadableException`](HumanRe |
    |                                   | adableException.html "class in co |
    |                                   | m.facebook.buck.core.exceptions") |
    |                                   | instead.                          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Exception                         | Description                       |
    +===================================+===================================+
    | [BuckUncheckedExe                 | ::: block                         |
    | cutionException](BuckUncheckedExe | Allows wrapping a checked         |
    | cutionException.html "class in co | exception into an unchecked       |
    | m.facebook.buck.core.exceptions") | exception in a way that Buck      |
    |                                   | understands.                      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Buil                             |                                   |
    | dTargetParseException](BuildTarge |                                   |
    | tParseException.html "class in co |                                   |
    | m.facebook.buck.core.exceptions") |                                   |
    +-----------------------------------+-----------------------------------+
    | [HumanReadableException](HumanRe  | ::: block                         |
    | adableException.html "class in co | Exception with an error message   |
    | m.facebook.buck.core.exceptions") | that can sensibly be displayed to |
    |                                   | the user without a stacktrace.    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RetryingException](Re            |                                   |
    | tryingException.html "class in co |                                   |
    | m.facebook.buck.core.exceptions") |                                   |
    +-----------------------------------+-----------------------------------+

    : Exception Summary[ ]{.tabEnd}
:::
:::

::: bottomNav
[]{#navbar.bottom}

::: skipNav
[Skip navigation links](#skip.navbar.bottom "Skip navigation links")
:::

[]{#navbar.bottom.firstrow}

-   [Overview](../../../../../index.html)
-   Package
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

[]{#skip.navbar.bottom}
:::

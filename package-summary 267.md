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
# Package com.facebook.buck.io.watchman {#package-com.facebook.buck.io.watchman .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [ProjectWatc                      |                                   |
    | h](ProjectWatch.html "interface i |                                   |
    | n com.facebook.buck.io.watchman") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Trans                            | ::: block                         |
    | port](Transport.html "interface i | An abstraction for IPC via        |
    | n com.facebook.buck.io.watchman") | messages.                         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [WatchmanClient]                  | ::: block                         |
    | (WatchmanClient.html "interface i | Testable interface for a Watchman |
    | n com.facebook.buck.io.watchman") | client.                           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [WatchmanDiagnostic](Wat          |                                   |
    | chmanDiagnostic.html "interface i |                                   |
    | n com.facebook.buck.io.watchman") |                                   |
    +-----------------------------------+-----------------------------------+
    | [WatchmanEvent                    | ::: block                         |
    | ](WatchmanEvent.html "interface i | Interface for all Watchman        |
    | n com.facebook.buck.io.watchman") | events, requires them to have a   |
    |                                   | base path                         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [Watchman](Watchman.html "class i | ::: block                         |
    | n com.facebook.buck.io.watchman") | Contains the configuration for a  |
    |                                   | Watchman client as well as the    |
    |                                   | ability to create a client.       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [WatchmanCur                      |                                   |
    | sor](WatchmanCursor.html "class i |                                   |
    | n com.facebook.buck.io.watchman") |                                   |
    +-----------------------------------+-----------------------------------+
    | [WatchmanDiagnosticEvent](Watc    |                                   |
    | hmanDiagnosticEvent.html "class i |                                   |
    | n com.facebook.buck.io.watchman") |                                   |
    +-----------------------------------+-----------------------------------+
    | [WatchmanDiag                     | ::: block                         |
    | nosticEventListener](WatchmanDiag | Deduplicating event bus listener  |
    | nosticEventListener.html "class i | that outputs deduplicated         |
    | n com.facebook.buck.io.watchman") | messages over the given event     |
    |                                   | bus.                              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [WatchmanFacto                    | ::: block                         |
    | ry](WatchmanFactory.html "class i | Factory that is responsible for   |
    | n com.facebook.buck.io.watchman") | creating instances of             |
    |                                   | [`W                               |
    |                                   | atchman`](Watchman.html "class in |
    |                                   |  com.facebook.buck.io.watchman"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [                                 | ::: block                         |
    | WatchmanMultiplePathEvent](Watchm | Buck sends this event for all     |
    | anMultiplePathEvent.html "class i | files, directories and symlinks   |
    | n com.facebook.buck.io.watchman") | that were changed since last      |
    |                                   | invalidation                      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [WatchmanMultip                   | ::: block                         |
    | lePathEvent.Change](WatchmanMulti | Contains path and type of file    |
    | plePathEvent.Change.html "class i | system change                     |
    | n com.facebook.buck.io.watchman") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [WatchmanOverflowEvent](Wa        | ::: block                         |
    | tchmanOverflowEvent.html "class i | Buck sends this event when        |
    | n com.facebook.buck.io.watchman") | Watchman is unable to correctly   |
    |                                   | determine the whole set of        |
    |                                   | changes in the filesystem, or if  |
    |                                   | too many files have changed       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [WatchmanPathEvent                | ::: block                         |
    | ](WatchmanPathEvent.html "class i | Buck sends this event for every   |
    | n com.facebook.buck.io.watchman") | file that was added, modified or  |
    |                                   | deleted                           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [WatchmanWatch                    | ::: block                         |
    | er](WatchmanWatcher.html "class i | Queries Watchman for changes to a |
    | n com.facebook.buck.io.watchman") | path.                             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Enum                              | Description                       |
    +===================================+===================================+
    | [Ca                               | ::: block                         |
    | pability](Capability.html "enum i | Various                           |
    | n com.facebook.buck.io.watchman") | [capabil                          |
    |                                   | ities](https://facebook.github.io |
    |                                   | /watchman/docs/capabilities.html) |
    |                                   | supported by different versions   |
    |                                   | of Watchman.                      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [WatchmanDiagnostic.Level](Watc   |                                   |
    | hmanDiagnostic.Level.html "enum i |                                   |
    | n com.facebook.buck.io.watchman") |                                   |
    +-----------------------------------+-----------------------------------+
    | [WatchmanEvent.Kind               | ::: block                         |
    | ](WatchmanEvent.Kind.html "enum i | The kind of event that occurred   |
    | n com.facebook.buck.io.watchman") | in watched file system, like      |
    |                                   | creation of a new file            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [WatchmanEvent.Type               | ::: block                         |
    | ](WatchmanEvent.Type.html "enum i | Type of the file that was         |
    | n com.facebook.buck.io.watchman") | changed, like a regular file or a |
    |                                   | directory                         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [W                                |                                   |
    | atchmanWatcher.CursorType](Watchm |                                   |
    | anWatcher.CursorType.html "enum i |                                   |
    | n com.facebook.buck.io.watchman") |                                   |
    +-----------------------------------+-----------------------------------+
    | [WatchmanWatcher.Fre              |                                   |
    | shInstanceAction](WatchmanWatcher |                                   |
    | .FreshInstanceAction.html "enum i |                                   |
    | n com.facebook.buck.io.watchman") |                                   |
    +-----------------------------------+-----------------------------------+

    : Enum Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Exception                         | Description                       |
    +===================================+===================================+
    | [FileSyst                         | ::: block                         |
    | emNotWatchedException](FileSystem | A                                 |
    | NotWatchedException.html "class i | [`                                |
    | n com.facebook.buck.io.watchman") | Watchman`](Watchman.html "class i |
    |                                   | n com.facebook.buck.io.watchman") |
    |                                   | object does not have a necessary  |
    |                                   | [`ProjectWatch`                   |
    |                                   | ](ProjectWatch.html "interface in |
    |                                   |  com.facebook.buck.io.watchman"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Watchm                           | ::: block                         |
    | anQueryFailedException](WatchmanQ | Watchman returned an error        |
    | ueryFailedException.html "class i | response.                         |
    | n com.facebook.buck.io.watchman") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [WatchmanQu                       | ::: block                         |
    | eryTimedOutException](WatchmanQue | Watchman took too long to respond |
    | ryTimedOutException.html "class i | to a query.                       |
    | n com.facebook.buck.io.watchman") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [WatchmanWatcherException](Watch  |                                   |
    | manWatcherException.html "class i |                                   |
    | n com.facebook.buck.io.watchman") |                                   |
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

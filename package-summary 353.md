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
-   Package
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

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
# Package com.facebook.buck.util {#package-com.facebook.buck.util .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [Direc                            |                                   |
    | toryCleaner.PathSelector](Directo |                                   |
    | ryCleaner.PathSelector.html "inte |                                   |
    | rface in com.facebook.buck.util") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ErrorLogger.LogImp               |                                   |
    | l](ErrorLogger.LogImpl.html "inte |                                   |
    | rface in com.facebook.buck.util") |                                   |
    +-----------------------------------+-----------------------------------+
    | [FilteredDirectoryCopier](F       |                                   |
    | ilteredDirectoryCopier.html "inte |                                   |
    | rface in com.facebook.buck.util") |                                   |
    +-----------------------------------+-----------------------------------+
    | [I                                | ::: block                         |
    | nputStreamConsumer.Handler](Input | Interface to handle a line of     |
    | StreamConsumer.Handler.html "inte | input from the stream.            |
    | rface in com.facebook.buck.util") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Libc](Libc.html "inte            |                                   |
    | rface in com.facebook.buck.util") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Libc.OpenPtyLibrar               |                                   |
    | y](Libc.OpenPtyLibrary.html "inte |                                   |
    | rface in com.facebook.buck.util") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ListeningCharsetDecoder.D        |                                   |
    | ecoderListener](ListeningCharsetD |                                   |
    | ecoder.DecoderListener.html "inte |                                   |
    | rface in com.facebook.buck.util") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ListeningCharsetEncoder.E        |                                   |
    | ncoderListener](ListeningCharsetE |                                   |
    | ncoder.EncoderListener.html "inte |                                   |
    | rface in com.facebook.buck.util") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ListeningProcessExecutor.La      | ::: block                         |
    | unchedProcess](ListeningProcessEx | Represents a process which was    |
    | ecutor.LaunchedProcess.html "inte | launched by a                     |
    | rface in com.facebook.buck.util") | [`ListeningProcessExecutor`]      |
    |                                   | (ListeningProcessExecutor.html "c |
    |                                   | lass in com.facebook.buck.util"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ListeningProcessExecutor.Pr      | ::: block                         |
    | ocessListener](ListeningProcessEx | Callback API to notify the caller |
    | ecutor.ProcessListener.html "inte | on a background thread when a     |
    | rface in com.facebook.buck.util") | process starts, exits, has stdout |
    |                                   | or stderr bytes to read, or is    |
    |                                   | ready to receive bytes on stdin.  |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ProcessExe                       |                                   |
    | cutor](ProcessExecutor.html "inte |                                   |
    | rface in com.facebook.buck.util") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ProcessEx                        | ::: block                         |
    | ecutor.LaunchedProcess](ProcessEx | Represents a running process      |
    | ecutor.LaunchedProcess.html "inte | returned by                       |
    | rface in com.facebook.buck.util") | [`Proce                           |
    |                                   | ssExecutor.launchProcess(ProcessE |
    |                                   | xecutorParams)`](ProcessExecutor. |
    |                                   | html#launchProcess(com.facebook.b |
    |                                   | uck.util.ProcessExecutorParams)). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ProcessExecutorFactory](         |                                   |
    | ProcessExecutorFactory.html "inte |                                   |
    | rface in com.facebook.buck.util") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ProcessM                         | ::: block                         |
    | anager](ProcessManager.html "inte | Checks for and kills processes.   |
    | rface in com.facebook.buck.util") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ProcessRegistry.ProcessRe        | ::: block                         |
    | gisterCallback](ProcessRegistry.P | A callback to be called upon      |
    | rocessRegisterCallback.html "inte | registering a process.            |
    | rface in com.facebook.buck.util") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Scope](Scope.html "inte          | ::: block                         |
    | rface in com.facebook.buck.util") | A more specific interface that    |
    |                                   | doesn\'t throw rather than using  |
    |                                   | [`AutoCloseable`](http            |
    |                                   | ://docs.oracle.com/javase/7/docs/ |
    |                                   | api/java/lang/AutoCloseable.html? |
    |                                   | is-external=true "class or interf |
    |                                   | ace in java.lang"){.externalLink} |
    |                                   | directly.                         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [UserId                           | ::: block                         |
    | Fetcher](UserIdFetcher.html "inte | Fetches the user ID of the        |
    | rface in com.facebook.buck.util") | running process.                  |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [AbstractClosea                   | ::: block                         |
    | bleMemoizedSupplier](AbstractClos | Base class for                    |
    | eableMemoizedSupplier.html "class | [`CloseableMemoizedSupplier`]     |
    |  in com.facebook.buck.util")\<T,​E | (CloseableMemoizedSupplier.html " |
    | extends                           | class in com.facebook.buck.util") |
    | [Exception](ht                    | and                               |
    | tp://docs.oracle.com/javase/7/doc | [`ThrowingCl                      |
    | s/api/java/lang/Exception.html?is | oseableMemoizedSupplier`](Throwin |
    | -external=true "class or interfac | gCloseableMemoizedSupplier.html " |
    | e in java.lang"){.externalLink}\> | class in com.facebook.buck.util") |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AbstractCloseableWrapper](Abs    | ::: block                         |
    | tractCloseableWrapper.html "class | Base class for                    |
    |  in com.facebook.buck.util")\<T,​E | `ThrowingCloseableWrapper` and    |
    | extends                           | `CloseableWrapper`                |
    | [Exception](ht                    | :::                               |
    | tp://docs.oracle.com/javase/7/doc |                                   |
    | s/api/java/lang/Exception.html?is |                                   |
    | -external=true "class or interfac |                                   |
    | e in java.lang"){.externalLink}\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [Ansi](Ansi.html "                | ::: block                         |
    | class in com.facebook.buck.util") | Encapsulates the specifics of     |
    |                                   | writing to a particular kind of   |
    |                                   | terminal.                         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [AnsiEnvironmentCheckin           | ::: block                         |
    | g](AnsiEnvironmentChecking.html " | Utility class to check if the     |
    | class in com.facebook.buck.util") | environment supports ANSI escape  |
    |                                   | sequences.                        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BgProc                           | ::: block                         |
    | essKiller](BgProcessKiller.html " | Safely kill background processes  |
    | class in com.facebook.buck.util") | on nailgun client exit.           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [                                 |                                   |
    | BuckConstant](BuckConstant.html " |                                   |
    | class in com.facebook.buck.util") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ByteBufferRe                     | ::: block                         |
    | placer](ByteBufferReplacer.html " | Performs an in-place              |
    | class in com.facebook.buck.util") | find-and-replace on               |
    |                                   | [`ByteBuffer`]                    |
    |                                   | (http://docs.oracle.com/javase/7/ |
    |                                   | docs/api/java/nio/ByteBuffer.html |
    |                                   | ?is-external=true "class or inter |
    |                                   | face in java.nio"){.externalLink} |
    |                                   | objects, where the replacements   |
    |                                   | are of equal length to what       |
    |                                   | they\'re replacing.               |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CapturingPrintSt                 |                                   |
    | ream](CapturingPrintStream.html " |                                   |
    | class in com.facebook.buck.util") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ChunkAcc                         | ::: block                         |
    | umulator](ChunkAccumulator.html " | Accumulates                       |
    | class in com.facebook.buck.util") | [`String                          |
    |                                   | `](http://docs.oracle.com/javase/ |
    |                                   | 7/docs/api/java/lang/String.html? |
    |                                   | is-external=true "class or interf |
    |                                   | ace in java.lang"){.externalLink} |
    |                                   | chunks, keeping only the most     |
    |                                   | recent to stay under a given      |
    |                                   | maximum size.                     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ClassLoa                         | ::: block                         |
    | derCache](ClassLoaderCache.html " | Maintain a cache mapping class    |
    | class in com.facebook.buck.util") | paths to class loaders that load  |
    |                                   | from these class paths.           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Closeable                        | ::: block                         |
    | Holder](CloseableHolder.html "cla | CloseableHolder is used to pass   |
    | ss in com.facebook.buck.util")\<T | ownership of a Closeable.         |
    | extends                           | :::                               |
    | [Closeable                        |                                   |
    | ](http://docs.oracle.com/javase/7 |                                   |
    | /docs/api/java/io/Closeable.html? |                                   |
    | is-external=true "class or interf |                                   |
    | ace in java.io"){.externalLink}\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [CloseableMemoizedSupplier](Clos  | ::: block                         |
    | eableMemoizedSupplier.html "class | Convenience wrapper class to      |
    |  in com.facebook.buck.util")\<T\> | attach closeable functionality to |
    |                                   | suppliers of resources to be      |
    |                                   | closed.                           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CloseableWrap                    | ::: block                         |
    | per](CloseableWrapper.html "class | Convenience wrapper class to      |
    |  in com.facebook.buck.util")\<T\> | attach closeable functionality to |
    |                                   | non-closeable class so it can be  |
    |                                   | used with try-with-resources to   |
    |                                   | make sure resources are always    |
    |                                   | released and proper exception     |
    |                                   | suppression is used.              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Comman                           | ::: block                         |
    | dSplitter](CommandSplitter.html " | Splits an argument list into a    |
    | class in com.facebook.buck.util") | list of command invocations whose |
    |                                   | total length will not exceed the  |
    |                                   | specified limit if possible.      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Console](Console.html "          |                                   |
    | class in com.facebook.buck.util") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ContextualProcessExecutor]       |                                   |
    | (ContextualProcessExecutor.html " |                                   |
    | class in com.facebook.buck.util") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Def                              | ::: block                         |
    | aultFilteredDirectoryCopier](Defa | This class allows the creation of |
    | ultFilteredDirectoryCopier.html " | copies of multiple directories,   |
    | class in com.facebook.buck.util") | while filtering out files which   |
    |                                   | do not match a specified          |
    |                                   | predicate.                        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [DefaultProcessExecut             | ::: block                         |
    | or](DefaultProcessExecutor.html " | Executes a                        |
    | class in com.facebook.buck.util") | [`Process`                        |
    |                                   | ](http://docs.oracle.com/javase/7 |
    |                                   | /docs/api/java/lang/Process.html? |
    |                                   | is-external=true "class or interf |
    |                                   | ace in java.lang"){.externalLink} |
    |                                   | and blocks until it is finished.  |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Director                         |                                   |
    | yCleaner](DirectoryCleaner.html " |                                   |
    | class in com.facebook.buck.util") |                                   |
    +-----------------------------------+-----------------------------------+
    | [DirectoryCleaner.PathStats](     |                                   |
    | DirectoryCleaner.PathStats.html " |                                   |
    | class in com.facebook.buck.util") |                                   |
    +-----------------------------------+-----------------------------------+
    | [DirectoryCleaner                 |                                   |
    | Args](DirectoryCleanerArgs.html " |                                   |
    | class in com.facebook.buck.util") |                                   |
    +-----------------------------------+-----------------------------------+
    | [DirectoryCleanerArgs.Builder](Di |                                   |
    | rectoryCleanerArgs.Builder.html " |                                   |
    | class in com.facebook.buck.util") |                                   |
    +-----------------------------------+-----------------------------------+
    | [DirtyPrintStreamDecorator]       | ::: block                         |
    | (DirtyPrintStreamDecorator.html " | Decorator of PrintStreams that    |
    | class in com.facebook.buck.util") | tracks whether or not that stream |
    |                                   | has been written to.              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Dis                              | ::: block                         |
    | cardable](Discardable.html "class | Discardable is a simple class     |
    |  in com.facebook.buck.util")\<T\> | that just holds some instance of  |
    |                                   | a type and has a discard() that   |
    |                                   | disables access to the instance.  |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [DuplicatingC                     | ::: block                         |
    | onsole](DuplicatingConsole.html " | Manages a Duplicate Console so    |
    | class in com.facebook.buck.util") | that console actions can be       |
    |                                   | replicated across to another      |
    |                                   | console.                          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ErrorLogger](ErrorLogger.html "  |                                   |
    | class in com.facebook.buck.util") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ErrorLogger                      | ::: block                         |
    | .DeconstructedException](ErrorLog | The result of exception           |
    | ger.DeconstructedException.html " | \"deconstruction\".               |
    | class in com.facebook.buck.util") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Escaper](Escaper.html "          |                                   |
    | class in com.facebook.buck.util") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ForwardingProcessListener]       |                                   |
    | (ForwardingProcessListener.html " |                                   |
    | class in com.facebook.buck.util") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Im                               | ::: block                         |
    | mutableMapWithNullValues](Immutab | `ImmutableMap` uses 16 fewer      |
    | leMapWithNullValues.html "class i | bytes per entry than              |
    | n com.facebook.buck.util")\<K,​V\> | [`TreeMap`]                       |
    |                                   | (http://docs.oracle.com/javase/7/ |
    |                                   | docs/api/java/util/TreeMap.html?i |
    |                                   | s-external=true "class or interfa |
    |                                   | ce in java.util"){.externalLink}, |
    |                                   | but does not allow null values.   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ImmutableMapWithNu               |                                   |
    | llValues.Builder](ImmutableMapWit |                                   |
    | hNullValues.Builder.html "class i |                                   |
    | n com.facebook.buck.util")\<K,​V\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [InputStreamCon                   | ::: block                         |
    | sumer](InputStreamConsumer.html " | An utility to process input       |
    | class in com.facebook.buck.util") | stream with a list of             |
    |                                   | line-by-line consumers            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Len                              | ::: block                         |
    | ientBooleanJsonDeserializer](Leni | JSON deserializer which converts  |
    | entBooleanJsonDeserializer.html " | boolean, numeric, and string      |
    | class in com.facebook.buck.util") | values into booleans.             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Libc                             |                                   |
    | .Constants](Libc.Constants.html " |                                   |
    | class in com.facebook.buck.util") |                                   |
    +-----------------------------------+-----------------------------------+
    | [LineFetcher](LineFetcher.html "  |                                   |
    | class in com.facebook.buck.util") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ListeningCharsetDecode           |                                   |
    | r](ListeningCharsetDecoder.html " |                                   |
    | class in com.facebook.buck.util") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ListeningCharsetEncode           |                                   |
    | r](ListeningCharsetEncoder.html " |                                   |
    | class in com.facebook.buck.util") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ListeningProcessExecutor         | ::: block                         |
    | ](ListeningProcessExecutor.html " | Replacement for                   |
    | class in com.facebook.buck.util") | [`ProcessBuilder`](http:          |
    |                                   | //docs.oracle.com/javase/7/docs/a |
    |                                   | pi/java/lang/ProcessBuilder.html? |
    |                                   | is-external=true "class or interf |
    |                                   | ace in java.lang"){.externalLink} |
    |                                   | which provides an asynchronous    |
    |                                   | callback interface to notify the  |
    |                                   | caller on a background thread     |
    |                                   | when a process starts, performs   |
    |                                   | I/O, or exits.                    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Memoizer](Memoizer.html "class   | ::: block                         |
    |  in com.facebook.buck.util")\<T\> | Memoizes a value, supporting      |
    |                                   | passing in a supplier when        |
    |                                   | getting the value, unlike         |
    |                                   | `                                 |
    |                                   | MoreSuppliers.MemoizingSupplier`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [More                             |                                   |
    | Exceptions](MoreExceptions.html " |                                   |
    | class in com.facebook.buck.util") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Mo                               | ::: block                         |
    | reFunctions](MoreFunctions.html " | Utilities to work with            |
    | class in com.facebook.buck.util") | `Function`.                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Mo                               |                                   |
    | reIterables](MoreIterables.html " |                                   |
    | class in com.facebook.buck.util") |                                   |
    +-----------------------------------+-----------------------------------+
    | [MoreMaps](MoreMaps.html "        |                                   |
    | class in com.facebook.buck.util") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Mo                               |                                   |
    | reSuppliers](MoreSuppliers.html " |                                   |
    | class in com.facebook.buck.util") |                                   |
    +-----------------------------------+-----------------------------------+
    | [More                             |                                   |
    | Throwables](MoreThrowables.html " |                                   |
    | class in com.facebook.buck.util") |                                   |
    +-----------------------------------+-----------------------------------+
    | [NamedTemporaryDirector           | ::: block                         |
    | y](NamedTemporaryDirectory.html " | Creates a temporary directory     |
    | class in com.facebook.buck.util") | that is (recursively) deleted     |
    |                                   | when this object is closed.       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [NamedTempora                     | ::: block                         |
    | ryFile](NamedTemporaryFile.html " | Creates a temporary file that is  |
    | class in com.facebook.buck.util") | deleted when this object is       |
    |                                   | closed.                           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ObjectF                          |                                   |
    | ileCommonModificationDate](Object |                                   |
    | FileCommonModificationDate.html " |                                   |
    | class in com.facebook.buck.util") |                                   |
    +-----------------------------------+-----------------------------------+
    | [PatternAnd                       | ::: block                         |
    | Message](PatternAndMessage.html " | A class that holds a pattern and  |
    | class in com.facebook.buck.util") | a message related to this         |
    |                                   | pattern.                          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Patter                           | ::: block                         |
    | nsMatcher](PatternsMatcher.html " | Helper class that keeps a list of |
    | class in com.facebook.buck.util") | compiled patterns and provides a  |
    |                                   | method to check whether a string  |
    |                                   | matches at least one of them.     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PkillProcessMa                   | ::: block                         |
    | nager](PkillProcessManager.html " | Checks for and kills processes by |
    | class in com.facebook.buck.util") | name.                             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PrintStre                        |                                   |
    | amProcessExecutorFactory](PrintSt |                                   |
    | reamProcessExecutorFactory.html " |                                   |
    | class in com.facebook.buck.util") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ProcessExecut                    | ::: block                         |
    | or.LaunchedProcessImpl](ProcessEx | Wraps a                           |
    | ecutor.LaunchedProcessImpl.html " | [`Process`                        |
    | class in com.facebook.buck.util") | ](http://docs.oracle.com/javase/7 |
    |                                   | /docs/api/java/lang/Process.html? |
    |                                   | is-external=true "class or interf |
    |                                   | ace in java.lang"){.externalLink} |
    |                                   | and exposes only its I/O streams, |
    |                                   | so callers have to pass it back   |
    |                                   | to this class.                    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ProcessExecutor.Resu             | ::: block                         |
    | lt](ProcessExecutor.Result.html " | Values from the result of         |
    | class in com.facebook.buck.util") | [`ProcessExecutor.lau             |
    |                                   | nchAndExecute(ProcessExecutorPara |
    |                                   | ms, Set,  Optional, Optional, Opt |
    |                                   | ional)`](ProcessExecutor.html#lau |
    |                                   | nchAndExecute(com.facebook.buck.u |
    |                                   | til.ProcessExecutorParams,java.ut |
    |                                   | il.Set,java.util.Optional,java.ut |
    |                                   | il.Optional,java.util.Optional)). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ProcessExecutorPar               | ::: block                         |
    | ams](ProcessExecutorParams.html " | Value type passed to              |
    | class in com.facebook.buck.util") | [`ProcessExec                     |
    |                                   | utor`](ProcessExecutor.html "inte |
    |                                   | rface in com.facebook.buck.util") |
    |                                   | to launch a process.              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [P                                |                                   |
    | rocessExecutorParams.Builder](Pro |                                   |
    | cessExecutorParams.Builder.html " |                                   |
    | class in com.facebook.buck.util") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Pr                               | ::: block                         |
    | ocessHelper](ProcessHelper.html " | A helper singleton that provides  |
    | class in com.facebook.buck.util") | facilities such as extracting the |
    |                                   | native process id of a            |
    |                                   | [`Process`                        |
    |                                   | ](http://docs.oracle.com/javase/7 |
    |                                   | /docs/api/java/lang/Process.html? |
    |                                   | is-external=true "class or interf |
    |                                   | ace in java.lang"){.externalLink} |
    |                                   | or gathering the process resource |
    |                                   | consumption.                      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Proces                           | ::: block                         |
    | sRegistry](ProcessRegistry.html " | A singleton helper class for      |
    | class in com.facebook.buck.util") | process registration.             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ProcessResourceConsumption](     | ::: block                         |
    | ProcessResourceConsumption.html " | Represents resource consumption   |
    | class in com.facebook.buck.util") | counters of a                     |
    |                                   | [`Process`]                       |
    |                                   | (http://docs.oracle.com/javase/7/ |
    |                                   | docs/api/java/lang/Process.html?i |
    |                                   | s-external=true "class or interfa |
    |                                   | ce in java.lang"){.externalLink}. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Statistics](Statistics.html "    | ::: block                         |
    | class in com.facebook.buck.util") | A crappy version of               |
    |                                   | `org.apache.commons.math3.sta     |
    |                                   | t.descriptive.SummaryStatistics`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [TeeOut                           | ::: block                         |
    | putStream](TeeOutputStream.html " | An OutputStream which forwards to |
    | class in com.facebook.buck.util") | two OutputStreams.                |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Threads](Threads.html "          |                                   |
    | class in com.facebook.buck.util") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ThrowingClosea                   | ::: block                         |
    | bleMemoizedSupplier](ThrowingClos | Convenience wrapper class to      |
    | eableMemoizedSupplier.html "class | attach closeable functionality to |
    |  in com.facebook.buck.util")\<T,​E | suppliers of resources to be      |
    | extends                           | closed.                           |
    | [Exception](ht                    | :::                               |
    | tp://docs.oracle.com/javase/7/doc |                                   |
    | s/api/java/lang/Exception.html?is |                                   |
    | -external=true "class or interfac |                                   |
    | e in java.lang"){.externalLink}\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [ThrowingCloseableWrapper](Thr    | ::: block                         |
    | owingCloseableWrapper.html "class | Convenience wrapper class to      |
    |  in com.facebook.buck.util")\<T,​E | attach closeable functionality to |
    | extends                           | non-closeable class so it can be  |
    | [Exception](ht                    | used with try-with-resources to   |
    | tp://docs.oracle.com/javase/7/doc | make sure resources are always    |
    | s/api/java/lang/Exception.html?is | released and proper exception     |
    | -external=true "class or interfac | suppression is used.              |
    | e in java.lang"){.externalLink}\> | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ThrowingMemoi                    | ::: block                         |
    | zer](ThrowingMemoizer.html "class | Memoizes a value or an exception  |
    |  in com.facebook.buck.util")\<T,​E | when computing it, supporting     |
    | extends                           | passing in a throwing supplier    |
    | [Exception](ht                    | when getting the value, unlike    |
    | tp://docs.oracle.com/javase/7/doc | `                                 |
    | s/api/java/lang/Exception.html?is | MoreSuppliers.MemoizingSupplier`. |
    | -external=true "class or interfac | :::                               |
    | e in java.lang"){.externalLink}\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [ThrowingPrintW                   | ::: block                         |
    | riter](ThrowingPrintWriter.html " | A (partial) replacement for       |
    | class in com.facebook.buck.util") | [`PrintWriter`                    |
    |                                   | ](http://docs.oracle.com/javase/7 |
    |                                   | /docs/api/java/io/PrintWriter.htm |
    |                                   | l?is-external=true "class or inte |
    |                                   | rface in java.io"){.externalLink} |
    |                                   | with methods that throw           |
    |                                   | [`IOException`]                   |
    |                                   | (http://docs.oracle.com/javase/7/ |
    |                                   | docs/api/java/io/IOException.html |
    |                                   | ?is-external=true "class or inter |
    |                                   | face in java.io"){.externalLink}. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [TimeFormat](TimeFormat.html "    |                                   |
    | class in com.facebook.buck.util") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Types](Types.html "              |                                   |
    | class in com.facebook.buck.util") |                                   |
    +-----------------------------------+-----------------------------------+
    | [UnixUserId                       | ::: block                         |
    | Fetcher](UnixUserIdFetcher.html " | Fetches the user ID of the        |
    | class in com.facebook.buck.util") | running process.                  |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [VersionStringComparato           | ::: block                         |
    | r](VersionStringComparator.html " | Compares version strings such as  |
    | class in com.facebook.buck.util") | \"4.2.2\", \"17.0\",              |
    |                                   | \"r10e-rc4\".                     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [WeakM                            | ::: block                         |
    | emoizer](WeakMemoizer.html "class | Memoizes a value with a weak      |
    |  in com.facebook.buck.util")\<T\> | reference, supporting passing in  |
    |                                   | a supplier when getting the       |
    |                                   | value, unlike                     |
    |                                   | `Mor                              |
    |                                   | eSuppliers.WeakMemoizingSupplier` |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ZipFileT                         |                                   |
    | raversal](ZipFileTraversal.html " |                                   |
    | class in com.facebook.buck.util") |                                   |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Enum                              | Description                       |
    +===================================+===================================+
    | [Ansi.Severi                      |                                   |
    | tyLevel](Ansi.SeverityLevel.html  |                                   |
    | "enum in com.facebook.buck.util") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Dep                              |                                   |
    | endencyMode](DependencyMode.html  |                                   |
    | "enum in com.facebook.buck.util") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Esc                              | ::: block                         |
    | aper.Quoter](Escaper.Quoter.html  | The quoting style to use when     |
    | "enum in com.facebook.buck.util") | escaping.                         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ExitCode](ExitCode.html          | ::: block                         |
    | "enum in com.facebook.buck.util") | ExitCode class defines Buck       |
    |                                   | binary protocol, i.e.             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ProcessExecutor.Opt              | ::: block                         |
    | ion](ProcessExecutor.Option.html  | Options for                       |
    | "enum in com.facebook.buck.util") | [`ProcessExecutor.lau             |
    |                                   | nchAndExecute(ProcessExecutorPara |
    |                                   | ms, Set, Optional,  Optional, Opt |
    |                                   | ional)`](ProcessExecutor.html#lau |
    |                                   | nchAndExecute(com.facebook.buck.u |
    |                                   | til.ProcessExecutorParams,java.ut |
    |                                   | il.Set,java.util.Optional,java.ut |
    |                                   | il.Optional,java.util.Optional)). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Verbosity](Verbosity.html        | ::: block                         |
    | "enum in com.facebook.buck.util") | An indication of how verbose Buck |
    |                                   | should be.                        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Enum Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Exception                         | Description                       |
    +===================================+===================================+
    | [BuckIsDyingExcep                 | ::: block                         |
    | tion](BuckIsDyingException.html " | Indicates that something could    |
    | class in com.facebook.buck.util") | not be done because Buck was      |
    |                                   | dying.                            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CleanBuildShutdownException](C   | ::: block                         |
    | leanBuildShutdownException.html " | \* Exception sent to BuildEngine  |
    | class in com.facebook.buck.util") | to shut it down cleanly, i.e.     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CommandLineExcep                 | ::: block                         |
    | tion](CommandLineException.html " | Exception that is raised when     |
    | class in com.facebook.buck.util") | user-supplied command line        |
    |                                   | contains incompatible parameters  |
    |                                   | or in general cannot be executed  |
    |                                   | :::                               |
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

-   [Overview](../../../../index.html)
-   Package
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

[]{#skip.navbar.bottom}
:::

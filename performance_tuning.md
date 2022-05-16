/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.performance} /\*\*\*/ {template .soyweb} {call buck.page} {param
title: \'Performance Tuning\' /} {param navid:
\'about_performance_tuning\' /} {param description} Buck does a lot of
work to make builds as fast as possible, and we also give developers
tools to figure out where the time is being spent inside of their
builds. {/param} {param content}

## Performance Tuning Your Builds

Buck [does a lot of
work](%7BROOT%7Dconcept/what_makes_buck_so_fast.html) {sp} to make
builds as fast as possible, and we also give developers tools to figure
out where the time is being spent inside of their builds.

## Super Console

![Chrome Tracing
Sample](%7BROOT%7Dstatic/buck-build-15fps.gif){#super_console_sample}

When running Buck in an{sp}
[Ansi](http://en.wikipedia.org/wiki/ANSI_escape_code) compliant
terminal, Buck displays the break down of what each thread is doing,
updated every 100ms, in what we affectionately call \"SuperConsole.\"
While a build is running, this gives developers a good idea of what Buck
is spending its time doing, and can often help people spot issues in
their builds. If you want to see what happened after the fact or to have
a trace you can send around your team, use Chrome Tracing.

## Chrome Tracing

![Chrome Tracing
Sample](%7BROOT%7Dstatic/buck_chrome_sample.png){#chrome_sample} The
Chrome team has built an awesome framework for viewing performance
traces right inside of{sp}
[Chrome](http://www.chromium.org/developers/how-tos/trace-event-profiling-tool).
You can access this by going to `chrome://tracing` in your browser.
Consult the trace viewer\'s {sp}[project
page](https://github.com/google/trace-viewer/) for more information on
the trace viewer and the file format.

After Buck is done with each build, it will produce a Chrome Trace file
that can be loaded up in `chrome://tracing` in the directory
{sp}`buck-out/log/traces/`. Buck will save a file in the format
{sp}`build.[timestamp].trace`, and then create a symlink from the most
recent trace to `build.trace`.

To load up this trace, visit `chrome://tracing` inside of Chrome, and
hit \"Load\". Load the trace file of interest, and look around to see
where time was spent. Each row represents a different thread, and all of
the steps taken for a given rule are logged underneath that rule.
Additionally, we log information about how the rule was built and and
the rule key for each artifact fetch. Press *?* to get the help menu for
the Chrome Trace Viewer. {/param} // content {/call} // buck.page
{/template}

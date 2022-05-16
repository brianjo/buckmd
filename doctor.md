/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.command.doctor} /\*\*\*/ {template .soyweb} {call buck.page} {param
title: \'buck doctor\' /} {param navid: \'command_doctor\' /} {param
description} A command to debug other buck invocations. {/param} {param
content} {call buck.command} {param overview}

The purpose of this command is to help the user debug and solve and
issue of another buck command. This command requires implementing custom
server-side support to be fully functional. We do not provide a
functional implementation with buck, however we have documented the
protocol and the `DoctorCommandIntegrationTest` contains very simple
examples of interactions between the doctor command and server.

You can use this command after setting up the environment.

{literal}

    buck doctor

{/literal}

## Command flow

The command supports the debugging of other commands except invocations
of `buck rage` and `buck doctor`. At the start the user has to choose
the buck invocation that they want to debug. In order for a buck
invocation to appear on the list it must have log files in `buck-out`.
After choosing the command a report is generated and either stored
locally or is uploaded to a remote endpoint defined under `[rage]` in
buckconfig. Also, another Json report is generated structured after
class `AbstractDoctorEndpointRequest` and is send to the remote endpoint
defined under `[doctor]` in buckconfig. This report also contains a URL
to the location of the rage report. Then, the doctor remote endpoint
produces a response that contains information about the status of core
components like parsing, environment and remote cache along with
suggestions on how to solve potential problems.

## Setup notes

-   The command requires the creation of at least one remote endpoint
    that handles the Json request and creates the fixing suggestions
    based on the Json format of `AbstractDoctorEndpointResponse`.
-   If you want to also have the data from the creation of the rage
    report you will need to define another remote endpoint that can get
    the information, otherwise the zipped report will be saved on disk
-   All the communication is sent using POST.

## Formats & Structures

-   Request is based on the Json format of class
    `AbstractDoctorEndpointRequest`.
-   Response is based on the Json format of class
    `AbstractDoctorEndpointResponse`.
-   The rage report zip file contains a Json file will metadata and
    useful information along with a list of log files and local
    configuration.

You can pass extra arguments to the doctor request by defining the
`[doctor_extra_request_args]`. This will add them as extra parameters in
the post request. In this case the main information will be under
parameter `data`.

## Buckconfig example

``` {.prettyprint .lang-js}
{literal}
[rage]
    report_upload_url = https://localhost:4546
    report_max_size = 100MB

[doctor]
    endpoint_url = https://localhost:4545
    extra_request_args = ref=>12ab,token=>42
{/literal}
```

## Request example

``` {.prettyprint .lang-js}
{literal}
{
    buildId: "...",
    rageUrl: "...",
    machineReadableLog: "...",
}
{/literal}
```

## Response example

``` {.prettyprint .lang-js}
{literal}
{
    errorMessage: "...",
    suggestions: [
                   "state": "ERROR",
                   "area": "Environment",
                   "suggestion": "Parsing too slow. Check BUCK file.",
                 ]
}
{/literal}
```

{/param} {/call} {/param} // content {/call} // buck.page {/template}

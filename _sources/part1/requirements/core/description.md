## Overview

A server implementing the OGC API — Processes Standard provides access to processes. Each
implementation has a single landing page (path `/`) that provides links to:

- the API definition (no fixed path),
- the conformance declaration (path `/conformance`),
- the process list (path `/processes`).

The process list contains a summary of each process offered, including a link to a more detailed
description. The process description contains information about inputs and outputs and a link to the
execution endpoint for the process.

A HTTP POST request to the execution endpoint creates a new job. The inputs and outputs are passed
in a JSON execute-request document. The URL for accessing status information is delivered in the
HTTP `Location` response header.

After a process completes (status `successful` or `failed`), the results or exception information
can be retrieved from the job results endpoint.

## API Resources

| Resource | Path | HTTP method |
|---|---|---|
| Landing page | `/` | GET |
| Conformance classes | `/conformance` | GET |
| Process list | `/processes` | GET |
| Process description | `/processes/{processID}` | GET |
| Process execution | `/processes/{processID}/execution` | POST |
| Job status info | `/jobs/{jobID}` | GET |
| Job results | `/jobs/{jobID}/results` | GET |
| Single result | `/jobs/{jobID}/results/{outputID}` | GET |

<!-- requirements -->

The following section covers a subset of the core requirements focusing on the process list
operation. See the [full standard](https://docs.ogc.org/is/18-062r2/18-062r2.html) for all
requirements.

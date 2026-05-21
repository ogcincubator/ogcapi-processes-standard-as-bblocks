This requirements class specifies the JSON encoding for OGC API — Processes responses.

The JSON encoding is one of two pre-defined encodings (the other being HTML). It applies to all
standard API responses: the landing page, conformance declaration, process list, process
description, and job status endpoints. The encoding of process output values is independent of this
requirement — output values can be of any type regardless of whether the server supports the JSON
requirements class.

Servers supporting multiple encodings must provide encoding-specific URIs for resources (for
example, via format-specific path suffixes like `.json` or a query parameter such as `f=json`) so
that links to alternate representations can be expressed.

<!-- requirements -->

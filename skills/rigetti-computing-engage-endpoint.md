---
name: Engage a Rigetti endpoint to execute programs
description: Find or create a QCS endpoint for a quantum processor and open an engagement to execute Quil programs.
api: openapi/rigetti-computing-qcs-openapi-original.yml
operations: [ListEndpoints, GetDefaultEndpoint, GetEndpoint, CreateEndpoint, CreateEngagement, RestartEndpoint]
---

# Engage a Rigetti endpoint to execute programs

Open an execution engagement against a QCS endpoint so pyQuil (or the QCS SDK) can submit compiled Quil to a QPU.

## Auth
OAuth2 (Okta) JWT: `Authorization: Bearer <access_token>`. Base URL `https://api.qcs.rigetti.com`.

## Steps
1. **Find the default endpoint** — `GetDefaultEndpoint` (`GET /v1/quantumProcessors/{quantumProcessorId}/endpoints:getDefault`) for the target processor.
2. **Or list/create** — `ListEndpoints` (`GET /v1/endpoints`) or `CreateEndpoint` (`POST /v1/endpoints`) for a dedicated endpoint. Inspect with `GetEndpoint` (`GET /v1/endpoints/{endpointId}`); note the `mock` flag for test runs.
3. **Open an engagement** — `CreateEngagement` (`POST /v1/engagements`) to obtain the connection credentials/address used to submit programs (actual QPU execution runs over ZeroMQ/rpcq, not HTTP).
4. **Recover** — if an endpoint is unhealthy, `RestartEndpoint` (`POST /v1/endpoints/{endpointId}:restart`). A `503` means the endpoint is temporarily unavailable — retry with backoff.

## Conventions
- Custom methods use colon suffixes (`:getDefault`, `:restart`) per Google AIP-136.
- Errors: `{code, message, requestId, validationErrors}`; `422` returns field-level `validationErrors`.

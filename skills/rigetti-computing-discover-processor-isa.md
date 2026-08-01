---
name: Discover a Rigetti processor and its ISA
description: Enumerate Rigetti quantum processors and fetch a processor's instruction set architecture (qubits, native gates, benchmarks) via the QCS API.
api: openapi/rigetti-computing-qcs-openapi-original.yml
operations: [ListQuantumProcessors, GetQuantumProcessor, GetInstructionSetArchitecture, ListInstructionSetArchitectures, GetQuantumProcessorAccessors]
---

# Discover a Rigetti processor and its ISA

Retrieve the topology, native gate set, and calibration/benchmark data an agent needs to compile Quil for a target QPU.

## Auth
OAuth2 (Okta) JWT: `Authorization: Bearer <access_token>`. Base URL `https://api.qcs.rigetti.com`.

## Steps
1. **List processors** — `ListQuantumProcessors` (`GET /v1/quantumProcessors`).
2. **Select one** — `GetQuantumProcessor` (`GET /v1/quantumProcessors/{quantum_processor_id}`).
3. **Fetch the ISA** — `GetInstructionSetArchitecture` (`GET /v1/quantumProcessors/{quantum_processor_id}/instructionSetArchitecture`) for qubit topology, native instructions, and benchmarks. Feed this to quilc when compiling.
4. **(Optional) Browse all ISAs** — `ListInstructionSetArchitectures` (`GET /v1/instructionSetArchitectures`).
5. **(Optional) Accessors** — `GetQuantumProcessorAccessors` (`GET /v1/quantumProcessors/{quantum_processor_id}/accessors`) to see engagement access options.

## Conventions
- Pagination `pageSize`/`pageToken` → `nextPageToken`.
- Errors: `{code, message, requestId, validationErrors}`. A `404` means the processor id is invalid or not visible to your account.

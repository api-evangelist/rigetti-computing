---
name: Reserve Rigetti QPU time
description: Discover available Rigetti quantum processors and book a reservation on one via the QCS API.
api: openapi/rigetti-computing-qcs-openapi-original.yml
operations: [ListQuantumProcessors, GetQuantumProcessor, FindAvailableReservations, CreateReservation, GetReservation, DeleteReservation]
---

# Reserve Rigetti QPU time

Book dedicated time on a Rigetti quantum processing unit (QPU) through Quantum Cloud Services.

## Auth
All calls require an OAuth2 (Okta) JWT. Download a 24h access token from
`https://qcs.rigetti.com/auth/token` and send `Authorization: Bearer <access_token>`.
Base URL: `https://api.qcs.rigetti.com`.

## Steps
1. **List processors** — `ListQuantumProcessors` (`GET /v1/quantumProcessors`) to enumerate available QPUs. Page with `pageSize`/`pageToken`.
2. **Inspect one** — `GetQuantumProcessor` (`GET /v1/quantumProcessors/{quantum_processor_id}`) to confirm the target.
3. **Find slots** — `FindAvailableReservations` (`GET /v1/reservations:findAvailable`) filtered by processor and time window.
4. **Book** — `CreateReservation` (`POST /v1/reservations`) with the chosen start/end time and processor. A `402` means the account balance is insufficient; a `409` means the slot is no longer available — pick another.
5. **Confirm** — `GetReservation` (`GET /v1/reservations/{reservationId}`).
6. **Cancel if needed** — `DeleteReservation` (`DELETE /v1/reservations/{reservationId}`).

## Conventions
- Pagination: `pageSize` + `pageToken`, response `nextPageToken` (Google AIP-158).
- Errors: JSON `{code, message, requestId, validationErrors}`. Include `requestId` when contacting support. No idempotency key — do not blindly retry `CreateReservation`; re-check with `FindAvailableReservations` first.

# Rigetti Computing

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Rigetti Computing is a full-stack quantum computing company that builds superconducting quantum processors and delivers access to them through Quantum Cloud Services (QCS). Developers program Rigetti quantum processing units (QPUs) with the Quil quantum instruction language via the open-source pyQuil SDK, compile with quilc, and simulate locally with the Quantum Virtual Machine (QVM). The QCS HTTP API (api.qcs.rigetti.com) exposes REST-style operations for quantum processors, instruction set architectures, engagements, endpoints, reservations, groups, billing, and account management, secured with OAuth2 (Okta) JWT bearer tokens. This profile was seeded as a VC-portfolio lead and enriched by the API Evangelist pipeline from Rigetti's public QCS OpenAPI, SDKs, and developer documentation.

**Areas:** Company · Quantum Computing · Quantum Cloud · Developer Tools · SDK · Superconducting Qubits · Scientific Computing · Deep Tech

## Rigetti Computing on APIs.io

Everything profiled for Rigetti Computing is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/rigetti-computing/](https://apis.io/providers/rigetti-computing/)** — or go straight to one of the APIs or properties below.

### APIs (9)

- [Rigetti Computing Account API](https://apis.io/apis/rigetti-computing/rigetti-computing-account-api/) — The account API from Rigetti Computing — 22 operation(s) for account.
- [Rigetti Computing Authentication API](https://apis.io/apis/rigetti-computing/rigetti-computing-authentication-api/) — The authentication API from Rigetti Computing — 4 operation(s) for authentication.
- [Rigetti Computing Client Applications API](https://apis.io/apis/rigetti-computing/rigetti-computing-clientapplications-api/) — Check for the latest SDK versions.
- [Rigetti Computing Endpoints API](https://apis.io/apis/rigetti-computing/rigetti-computing-endpoints-api/) — The Endpoint is the means of access to a Quantum Processor.
- [Rigetti Computing Engagements API](https://apis.io/apis/rigetti-computing/rigetti-computing-engagements-api/) — The Engagement is the authorization mechanism for access to the Quantum Processor.
- [Rigetti Computing Quantum Processors API](https://apis.io/apis/rigetti-computing/rigetti-computing-quantumprocessors-api/) — The Quantum Processor is the heart of the Rigetti services.
- [Rigetti Computing Reservations API](https://apis.io/apis/rigetti-computing/rigetti-computing-reservations-api/) — Find existing time on a Rigetti QPU and reserve it.
- [Rigetti Computing Rigetti QCS API](https://apis.io/apis/rigetti-computing/rigetti-computing-rigetti-qcs-api-api/) — The Rigetti QCS API API from Rigetti Computing — 2 operation(s) for rigetti qcs api.
- [Rigetti Computing Health Check API](https://apis.io/apis/rigetti-computing/rigetti-computing-health-check-api/) — The Health Check API from Rigetti Computing — 1 operation(s) for health check.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [rigetti-qcs](https://apis.io/servers/rigetti-computing/rigetti-qcs/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Rigetti Computing Agentic Access](https://apis.io/agentic-access/rigetti-computing/rigetti-computing-agentic-access/)

#### Collections (9)

Postman and Open Collection request collections.

- [Rigetti QCS account API](https://apis.io/collections/rigetti-computing/open-rigetti-computing-account-api/)
- [Rigetti QCS account authentication API](https://apis.io/collections/rigetti-computing/open-rigetti-computing-authentication-api/)
- [Rigetti QCS account clientApplications API](https://apis.io/collections/rigetti-computing/open-rigetti-computing-clientapplications-api/)
- [Rigetti QCS account endpoints API](https://apis.io/collections/rigetti-computing/open-rigetti-computing-endpoints-api/)
- [Rigetti QCS account engagements API](https://apis.io/collections/rigetti-computing/open-rigetti-computing-engagements-api/)
- [Rigetti QCS account Healthcheck API](https://apis.io/collections/rigetti-computing/open-rigetti-computing-healthcheck-api/)
- [Rigetti QCS account quantumProcessors API](https://apis.io/collections/rigetti-computing/open-rigetti-computing-quantumprocessors-api/)
- [Rigetti QCS account reservations API](https://apis.io/collections/rigetti-computing/open-rigetti-computing-reservations-api/)
- [Rigetti QCS account Rigetti QCS API API](https://apis.io/collections/rigetti-computing/open-rigetti-computing-rigetti-qcs-api-api/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Rigetti Computing Qcs Overlay](https://apis.io/overlays/rigetti-computing/rigetti-computing-qcs-overlay/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Rigetti Computing Authentication](https://apis.io/security/rigetti-computing/rigetti-computing-authentication/)
- [Rigetti Computing Domain Security](https://apis.io/security/rigetti-computing/rigetti-computing-domain-security/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.rigetti.com/)
- [Documentation](https://docs.rigetti.com/)
- [Getting started](https://pyquil-docs.rigetti.com/)
- [API reference](https://docs.rigetti.com/qcs)
- [Sign up](https://www.rigetti.com/get-quantum)
- [Support](https://rigetti.zendesk.com)
- [Blog](https://www.rigetti.com/rigetti-computing-news)
- [Terms of service](https://www.rigetti.com/uploads/Global/Rigetti-Terms-of-Service-2022.pdf)
- [Privacy policy](https://www.rigetti.com/privacy-policy)
- [GitHub](https://github.com/rigetti)

## API Evangelist rating

**Kin Score 39.6** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 73.2 |
| Contract quality | 50.3 |
| Contract governance | 4.5 |
| Operational transparency | 2.6 |
| Developer ergonomics | 56.5 |
| Access clarity | 34.2 |

**Agent readiness 30.5** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | verified |
| OpenAPI Examples | — |
| Rate Limit Signal | verified |
| Event Surface Described | — |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | distinct |

**Regulatory alignment 24.5** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/rigetti-computing/](https://apis.io/providers/rigetti-computing/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Rigetti Computing: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/rigetti-computing/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).

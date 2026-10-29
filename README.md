# Authlete

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

Authlete is an API-first OAuth 2.0 and OpenID Connect backend service that provides a headless authorization-server engine. It handles the OAuth/OIDC protocol logic and token management so organizations can stand up standards-compliant authorization servers and verifiable-credential issuers without building the protocol layer themselves. Authlete separates the Management APIs (configure services and clients) from the Runtime APIs (power authorization, token, introspection, CIBA, device-flow, federation, and OID4VCI endpoints), and offers managed shared cloud, dedicated cloud, and self-managed deployment across US, Japan, Europe, and Brazil regional clusters. It supports advanced profiles including FAPI / FAPI 2.0, CIBA, PAR, Grant Management, OpenID Federation, Native SSO, and OpenID for Verifiable Credential Issuance, plus regional open-banking standards (Brazil Open Banking, Australia CDR). Backed by 500 Global.

**Areas:** Company · Authentication · OpenID Connect · Authorization · Identity · API Security · FAPI · Verifiable Credentials · CIBA

## Authlete on APIs.io

Everything profiled for Authlete is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/authlete/](https://apis.io/providers/authlete/)** — or go straight to one of the APIs or properties below.

### APIs (21)

- [Authlete Authorization Endpoint API](https://apis.io/apis/authlete/authlete-authorization-endpoint-api/) — API endpoints for implementing OAuth 2.0 Authorization Endpoint.
- [Authlete CIBA API](https://apis.io/apis/authlete/authlete-ciba-api/) — API endpoints for implementing Client-Initiated Backchannel Authentication (CIBA).
- [Authlete Client Management API](https://apis.io/apis/authlete/authlete-client-management-api/) — API endpoints for managing OAuth clients, including creation, update, and deletion of clients.
- [Authlete Device Flow API](https://apis.io/apis/authlete/authlete-device-flow-api/) — API endpoints for implementing OAuth 2.0 Device Flow
- [Authlete Dynamic Client Registration API](https://apis.io/apis/authlete/authlete-dynamic-client-registration-api/) — API endpoints for implementing OAuth 2.0 Dynamic Client Registration.
- [Authlete Federation Endpoint API](https://apis.io/apis/authlete/authlete-federation-endpoint-api/) — API endpoints for implementing OpenID Federation using Authlete.
- [Authlete Grant Management Endpoint API](https://apis.io/apis/authlete/authlete-grant-management-endpoint-api/) — API endpoint for implementing OAuth 2.0 grants, including grant management actions like updating and revoking grants.
- [Authlete Hardware Security Key API](https://apis.io/apis/authlete/authlete-hardware-security-key-api/) — API endpoints for managing hardware security keys (HSK).
- [Authlete Introspection Endpoint API](https://apis.io/apis/authlete/authlete-introspection-endpoint-api/) — API endpoints for implementing OAuth 2.0 Introspection Endpoint.
- [Authlete Jose Object API](https://apis.io/apis/authlete/authlete-jose-object-api/) — API endpoints for JOSE objects.
- [Authlete JWK Set Endpoint API](https://apis.io/apis/authlete/authlete-jwk-set-endpoint-api/) — API endpoints for to generate JSON Web Key Set (JWKS) for a service.
- [Authlete Lifecycle API](https://apis.io/apis/authlete/authlete-lifecycle-api/) — The Lifecycle API from Authlete — 1 operation(s) for lifecycle.
- [Authlete Native SSO API](https://apis.io/apis/authlete/authlete-native-sso-api/) — API endpoints for Native SSO
- [Authlete Pushed Authorization Endpoint API](https://apis.io/apis/authlete/authlete-pushed-authorization-endpoint-api/) — API endpoints for implementing OAuth 2.0 Pushed Authorization Requests (PAR).
- [Authlete Revocation Endpoint API](https://apis.io/apis/authlete/authlete-revocation-endpoint-api/) — API endpoint for implementing OAuth 2.0 Revocation Endpoint.
- [Authlete Service Management API](https://apis.io/apis/authlete/authlete-service-management-api/) — API endpoints for managing services, including creation, update, and deletion of services.
- [Authlete Token Endpoint API](https://apis.io/apis/authlete/authlete-token-endpoint-api/) — API endpoints for implementing OAuth 2.0 Token Endpoint.
- [Authlete Token Operations API](https://apis.io/apis/authlete/authlete-token-operations-api/) — API endpoints for various token related operations, including creating, revoking and deleting access_tokens with specified scopes.
- [Authlete UserInfo Endpoint API](https://apis.io/apis/authlete/authlete-userinfo-endpoint-api/) — API endpoints for implementing OpenID Connect UserInfo Endpoint.
- [Authlete Utility Endpoints API](https://apis.io/apis/authlete/authlete-utility-endpoints-api/) — API endpoints for various utility operations.
- [Authlete Verifiable Credential Issuer API](https://apis.io/apis/authlete/authlete-verifiable-credential-issuer-api/) — API endpoints for implementing and running a Verifiable Credential Issuer (VCI).

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [authlete](https://apis.io/servers/authlete/authlete/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Authlete Agentic Access](https://apis.io/agentic-access/authlete/authlete-agentic-access/)

#### Collections (21)

Postman and Open Collection request collections.

- [Authlete Authorization Endpoint API](https://apis.io/collections/authlete/open-authlete-authorization-endpoint-api/)
- [Authlete Authorization Endpoint CIBA API](https://apis.io/collections/authlete/open-authlete-ciba-api/)
- [Authlete Authorization Endpoint Client Management API](https://apis.io/collections/authlete/open-authlete-client-management-api/)
- [Authlete Authorization Endpoint Device Flow API](https://apis.io/collections/authlete/open-authlete-device-flow-api/)
- [Authlete Authorization Endpoint Dynamic Client Registration API](https://apis.io/collections/authlete/open-authlete-dynamic-client-registration-api/)
- [Authlete Authorization Endpoint Federation Endpoint API](https://apis.io/collections/authlete/open-authlete-federation-endpoint-api/)
- [Authlete Authorization Endpoint Grant Management Endpoint API](https://apis.io/collections/authlete/open-authlete-grant-management-endpoint-api/)
- [Authlete Authorization Endpoint Hardware Security Key API](https://apis.io/collections/authlete/open-authlete-hardware-security-key-api/)
- [Authlete Authorization Endpoint Introspection Endpoint API](https://apis.io/collections/authlete/open-authlete-introspection-endpoint-api/)
- [Authlete Authorization Endpoint Jose Object API](https://apis.io/collections/authlete/open-authlete-jose-object-api/)
- [Authlete Authorization Endpoint JWK Set Endpoint API](https://apis.io/collections/authlete/open-authlete-jwk-set-endpoint-api/)
- [Authlete Authorization Endpoint Lifecycle API](https://apis.io/collections/authlete/open-authlete-lifecycle-api/)
- [Authlete Authorization Endpoint Native SSO API](https://apis.io/collections/authlete/open-authlete-native-sso-api/)
- [Authlete Authorization Endpoint Pushed Authorization Endpoint API](https://apis.io/collections/authlete/open-authlete-pushed-authorization-endpoint-api/)
- [Authlete Authorization Endpoint Revocation Endpoint API](https://apis.io/collections/authlete/open-authlete-revocation-endpoint-api/)
- [Authlete Authorization Endpoint Service Management API](https://apis.io/collections/authlete/open-authlete-service-management-api/)
- [Authlete Authorization Endpoint Token Endpoint API](https://apis.io/collections/authlete/open-authlete-token-endpoint-api/)
- [Authlete Authorization Endpoint Token Operations API](https://apis.io/collections/authlete/open-authlete-token-operations-api/)
- [Authlete Authorization Endpoint UserInfo Endpoint API](https://apis.io/collections/authlete/open-authlete-userinfo-endpoint-api/)
- [Authlete Authorization Endpoint Utility Endpoints API](https://apis.io/collections/authlete/open-authlete-utility-endpoints-api/)
- [Authlete Authorization Endpoint Verifiable Credential Issuer API](https://apis.io/collections/authlete/open-authlete-verifiable-credential-issuer-api/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Authlete Openapi Overlay](https://apis.io/overlays/authlete/authlete-openapi-overlay/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Authlete Authentication](https://apis.io/security/authlete/authlete-authentication/)
- [Authlete Domain Security](https://apis.io/security/authlete/authlete-domain-security/)
- [Authlete Vulnerability Disclosure](https://apis.io/security/authlete/authlete-vulnerability-disclosure/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://authlete.com)
- [Documentation](https://docs.authlete.com/)
- [Getting started](https://www.authlete.com/developers/getting_started/)
- [API reference](https://docs.authlete.com/)
- [Pricing](https://www.authlete.com/pricing)
- [Sign up](https://console.authlete.com/)
- [Support](https://www.authlete.com/contact/)
- [Changelog](https://www.authlete.com/developers/relnotes/)
- [Blog](https://www.authlete.com/resources/blog)
- [Security](https://www.authlete.com/.well-known/security.txt)
- [Terms of service](https://www.authlete.com/terms-conditions)
- [Privacy policy](https://www.authlete.com/privacy-policy)
- [GitHub](https://github.com/authlete)
- [Status](https://www.authlete.com/service-status)

## API Evangelist rating

**Kin Score 48.9** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 73.2 |
| Contract quality | 50.4 |
| Contract governance | 4.5 |
| Operational transparency | 52.6 |
| Developer ergonomics | 68.5 |
| Access clarity | 31.6 |

**Agent readiness 30.8** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | verified |
| Error Semantics | derived (partial credit) |
| OpenAPI Examples | verified |
| Rate Limit Signal | — |
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
| Operation Distinctiveness | mostly |

**Regulatory alignment 30.4** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/authlete/](https://apis.io/providers/authlete/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Authlete: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/authlete/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).

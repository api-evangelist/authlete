---
name: Provision a service and register a client
description: Create an Authlete service (authorization-server instance) and register an OAuth/OIDC client under it.
api: openapi/authlete-openapi-original.yml
operations: [service_create_api, service_get_api, client_create_api, client_get_list_api]
---

# Provision a service and register a client

Use this to stand up a new authorization server in Authlete and register a relying-party client.

## Auth
- Send `Authorization: Bearer <token>` on every call. Use an **Organization Token** for service
  creation (service-level automation) — see `authentication/authlete-authentication.yml`.
- Pick a regional cluster base URL: `https://us.authlete.com` (or jp/eu/br).

## Steps
1. **Create the service** — `service_create_api`. Post the service configuration (name, supported
   grant types, response types, scopes, token settings). The response returns the new `serviceId`.
2. **Confirm the service** — `service_get_api` with the `serviceId` to read back the stored config
   and the issued service API credentials.
3. **Register a client** — `client_create_api` under that service. Post the client metadata
   (client name, redirect URIs, grant types, token-auth method, requested scopes). The response
   returns the `clientId` (and secret for confidential clients).
4. **Verify** — `client_get_list_api` (paginated via `start`/`end`) to confirm the client is listed
   under the service.

## Rules
- Pagination is offset-based: pass integer `start`/`end` query params on list calls.
- Errors are signalled by HTTP status (400/401/403/404/500), not problem+json — see
  `errors/authlete-problem-types.yml`. A 401 means a bad/missing token; 403 means the token lacks
  the required permission (e.g. `service.write`, `client.write`).
- No idempotency key is supported; do not blind-retry `create` calls — check the list first.

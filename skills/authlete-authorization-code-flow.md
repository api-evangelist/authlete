---
name: Drive an authorization-code flow at the runtime endpoints
description: Use Authlete's Runtime APIs to implement the OAuth 2.0 authorization-code flow inside your own authorization server.
api: openapi/authlete-openapi-original.yml
operations: [auth_authorization_api, auth_authorization_issue_api, auth_token_api, auth_introspection_api]
---

# Drive an authorization-code flow

Authlete is headless: your authorization-server front end receives the browser/API requests, then
delegates each protocol decision to an Authlete Runtime endpoint. Every Runtime call returns a
result object with an `action` telling you how to respond, plus `resultCode`/`resultMessage`.

## Auth
- `Authorization: Bearer <Service Access Token>` for the service whose authorization server you run.
- Base URL: your service's regional cluster (e.g. `https://us.authlete.com`).

## Steps
1. **Authorization request** — when the browser hits your `/authorize`, forward the query to
   `auth_authorization_api`. Inspect `action`: `INTERACTION` means prompt the user for login/consent;
   the response carries a `ticket` to resume with.
2. **Issue the authorization response** — after the user authenticates and consents, call
   `auth_authorization_issue_api` with the `ticket` and the authenticated `subject`. It returns the
   redirect (`Location`) containing the authorization `code` to send back to the client.
3. **Token request** — when the client posts the `code` to your `/token`, forward it to
   `auth_token_api`. `action: OK` returns the access token (and id/refresh tokens) to relay.
4. **Introspection** — resource servers validate tokens via `auth_introspection_api`; the result
   reports whether the token is active plus its scopes, subject, and client.

## Rules
- Never invent an endpoint: your server owns the HTTP endpoints; Authlete owns the protocol logic.
- Treat `action` as the control signal, not the HTTP status (Runtime calls typically return 200).
- See `conventions/authlete-conventions.yml` for the runtime result-object contract.

---
name: Issue a verifiable credential (OID4VCI)
description: Use Authlete's Verifiable Credential Issuer endpoints to offer and issue a credential under the OpenID for Verifiable Credential Issuance profile.
api: openapi/authlete-openapi-original.yml
operations: [vci_metadata_api, vci_offer_create_api, vci_single_parse_api, vci_single_issue_api]
---

# Issue a verifiable credential (OID4VCI)

Authlete implements OpenID for Verifiable Credential Issuance so a service configured as a VC issuer
can offer and mint credentials.

## Auth
- `Authorization: Bearer <Service Access Token>` for the VC-issuer service.
- Base URL: the service's regional cluster (e.g. `https://eu.authlete.com`).

## Steps
1. **Publish issuer metadata** — `vci_metadata_api` returns the credential-issuer metadata (supported
   credential types, formats, endpoints) that wallets read.
2. **Create a credential offer** — `vci_offer_create_api` produces a credential offer (and offer
   info) to hand to the holder's wallet, e.g. as a QR code / deep link.
3. **Parse the credential request** — when the wallet posts to your credential endpoint, forward it
   to `vci_single_parse_api` to validate the request and access token and extract what to issue.
4. **Issue the credential** — call `vci_single_issue_api` with the parsed request to mint the signed
   credential to return to the wallet. (Use the batch/deferred variants for multiple or async issuance.)

## Rules
- The access token presented by the wallet must have been issued for this service; validate it via
  the parse step rather than trusting the wallet.
- Errors surface as HTTP status codes; runtime outcomes surface in the result object's `action` /
  `resultCode` — see `errors/authlete-problem-types.yml`.

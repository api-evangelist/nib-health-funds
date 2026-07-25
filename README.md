# nib (nib-health-funds)

nib holdings limited (ASX:NHF), trading as nib, is an Australian private health insurer headquartered in Newcastle, New South Wales, and one of the country's largest health funds alongside Medibank, Bupa and HCF. Its lines of business span Australian residents health insurance, New Zealand health insurance through nib nz insurance limited, international workers and overseas student health cover (OSHC), travel insurance, and nib Thrive, its National Disability Insurance Scheme plan-management arm.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/nib-health-funds/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/nib-health-funds/refs/heads/main/apis.yml)

## API Posture

nib publishes **no public, self-serve developer portal and no downloadable OpenAPI definitions**. This profile records that absence honestly rather than inventing a surface.

- `developer.nib.com.au`, `developers.nib.com.au`, `docs.nib.com.au` and `api.nib.com.au` do not resolve.
- `/developers`, `/api`, `/developer`, `/partners` and `/integrations` on `nib.com.au` all return **404**.
- The published sitemap index expands to 1,445 URLs and contains no developer or API documentation page.
- A real first-party gateway exists at `api-gateway.nib.com.au` — named in nib's own Content-Security-Policy — and answers anonymously with **403** `{"message":"Forbidden"}`. Real internal APIs, no public surface.
- Healthcare provider integration is a **login wall** (the [nib HCP portal](https://www.nib.com.au/providers/hcp-portal/user/login)) plus third-party **HICAPS** and **HealthPoint** claiming terminals, with Honeysuckle Health handling medical network and MediGap registration.
- Member identity is an Auth0-backed OpenID Connect tenant at `id.nib.com.au` whose [discovery document](https://id.nib.com.au/.well-known/openid-configuration) is anonymously readable. Consumer sign-in only — no product, policy, or claims scopes.
- **ACORD posture: no ACORD reference found.** ACORD, AL3 and NGDS are property-and-casualty and life standards; Australian private health insurance runs on Medicare ECLIPSE plus HICAPS/HealthPoint terminals instead.
- None of quote, bind, issue or FNOL is exposed as a public API.
- No public Postman workspace, no GraphQL endpoint, no webhook or AsyncAPI event catalog.

Australia has the legal machinery for open insurance and no live obligation. The Consumer Data Right opened banking and energy and was designated to extend to general insurance before being deferred and de-prioritised — and it never covered private health insurance at all. nib's posture is exactly what a market with no forcing function produces.

## Tags

- Insurance
- Australia
- Health Insurance
- Carrier
- Claims
- Private Health Insurance
- Travel Insurance
- New Zealand
- NDIS
- Partner Gated

## Timestamps

- **Created:** 2026-07-25
- **Modified:** 2026-07-25

## APIs

None. nib does not publish a public API. See [review.yml](review.yml) for the full probe log, HTTP statuses, ACORD posture, and auth model.

## Links

- [Website](https://www.nib.com.au/)
- [Healthcare providers](https://www.nib.com.au/providers)
- [nib HCP portal (login)](https://www.nib.com.au/providers/hcp-portal/user/login)
- [Member login](https://my.nib.com.au/login)
- [GitHub organisation](https://github.com/nib-health-funds)
- [LinkedIn](https://www.linkedin.com/company/nib-health)
- [The Check Up (blog)](https://www.nib.com.au/the-checkup)
- [Media centre](https://www.nib.com.au/media)

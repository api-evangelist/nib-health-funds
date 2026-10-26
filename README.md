# nib (nib-health-funds)

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

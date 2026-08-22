# Firestorm

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

Firestorm (Firestorm Labs, Inc.) is a San Diego based defense technology company founded in 2022 by Daniel Magy, Chad McCoy, Ian Muceus and Adrien Lepleux. It builds expeditionary manufacturing systems and modular unmanned aerial systems: the **xCELL** containerized production unit uses HP Multi Jet Fusion additive manufacturing to 3D print industrial-grade PA-12 nylon composite airframes and spare parts at the tactical edge, feeding the **Tempest** modular fixed-wing UAS family and the **Squall** FPV drone. Firestorm holds a five-year, $100M U.S. Air Force IDIQ and closed an $82M Series B in April 2026 led by Washington Harbour Partners.

- Website: https://launchfirestorm.com/
- GitHub: https://github.com/launchfirestorm
- Careers: https://jobs.gem.com/firestorm
- Private-market listing: https://forgeglobal.com/firestorm_stock/

## API surface

**None found.** Firestorm ships hardware. As of the 2026-08-01 enrichment pass it publishes no developer portal, API reference, public API, SDK, OpenAPI/AsyncAPI/GraphQL contract, MCP server, or A2A agent card. Contract discovery probed the web host root and the `api.` / `docs.` / `developer.` / `app.` / `status.` / `trust.` subdomains (all NXDOMAIN) for `/openapi.json`, `/swagger.json`, `/.well-known/*`, `/llms.txt`, and both agent-card paths — every one missed. The probe record is in `well-known/firestorm-well-known.yml`.

## Artifacts

| Path | What it is |
|---|---|
| `packages/firestorm-packages.yml` | Registry + GitHub org search. One first-party open-source tool (`bump`, a versioning CLI); no API client SDK. |
| `well-known/firestorm-well-known.yml` | Every discovery path probed, with HTTP status. All 404 (true negatives — the host does not answer 200 for unknown paths). |
| `security/firestorm-domain-security.yml` | Probed TLS 1.3, HSTS (1 year), SPF and DMARC present (`p=none`), no DNSSEC, no CAA. |
| `llms/firestorm-llms.txt` | Generated llms.txt for the company (no provider-published one exists). |

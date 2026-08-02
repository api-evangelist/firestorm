# Firestorm

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

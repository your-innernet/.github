# security policy

innernet holds people's memory. we treat that as the most sensitive class of data there is, and we want to hear about anything that threatens it.

## reporting a vulnerability

email **[yours@innernet.live](mailto:yours@innernet.live)** with `security` in the subject line.

include what you found, where (URL, endpoint, or tool), and how to reproduce it. a proof of concept beats a theory — but we read everything.

- we acknowledge within **72 hours**
- we keep you updated while we triage and fix
- we ask for reasonable time to remediate before public disclosure
- there's no bounty program yet; we credit reporters (with permission) when a fix ships

## scope

- `innernet.live` — web app, dashboard, docs
- `innernet.live/api/mcp` — the hosted MCP server and its OAuth 2.1 flow
- `innernet.live/api/*` — platform APIs
- the `innernet` CLI and local MCP server

out of scope: denial of service and volumetric attacks, social engineering, and findings in third-party services we build on (report Supabase issues to Supabase, Vercel issues to Vercel).

## the posture

the platform runs row-level security as default-deny, hashes every token at rest, keeps an audit log, offers opt-in encryption-at-rest for memory content, and supports GDPR export and deletion. the full threat model lives in the (private) monorepo; the public summary is at [innernet.live/security](https://innernet.live/security).

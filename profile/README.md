<p align="center">
  <a href="https://innernet.live"><img src="https://innernet.live/brand/mark-color.svg" width="76" alt="innernet" /></a>
</p>

<h3 align="center">the internet, but yours.</h3>

<p align="center">
  <a href="https://innernet.live">innernet.live</a> ·
  <a href="https://innernet.live/docs">docs</a> ·
  <a href="https://innernet.live/company">company</a> ·
  <a href="https://x.com/yourInnernet">@yourInnernet</a>
</p>

---

every AI tool you use starts every conversation knowing nothing. you re-explain yourself, your projects, your taste — every session, every tool, forever. the thinking you've already done evaporates the moment a chat ends.

innernet is the memory layer underneath: one living, versioned context for you and each of your projects, maintained by an agent — not by you — and delivered to every AI tool you use over the [Model Context Protocol](https://modelcontextprotocol.io).

- **versioned** — your context has commits, branches, and merges. fork a direction, park it, fold it back. git for thinking.
- **maintained** — you don't write memory files. an agent captures as you work, consolidates on sync, and prunes what decays.
- **everywhere** — Claude, ChatGPT, Cursor, Cline, Zed — any MCP client reads the same map, live. no copy-paste between tools.
- **yours** — private by default, disclosure-gated, exportable. memory is the artifact, and it belongs to you.

### connect

the hosted server is live. add it to any MCP client and sign in once — no API key:

```json
{
  "mcpServers": {
    "innernet": { "type": "http", "url": "https://innernet.live/api/mcp" }
  }
}
```

per-client wiring lives in the [docs](https://innernet.live/docs).

### where the code is

the product is built in a private monorepo while the foundations settle — TypeScript end to end: a Next.js platform on Supabase, a local-first CLI, and MCP servers exposing the full memory surface (33 hosted tools across projects, personal memory, artifacts, and tasks). what ships and why is public on the [company page](https://innernet.live/company).

found something that looks wrong from the outside? security reports go to [SECURITY.md](https://github.com/your-innernet/.github/blob/main/SECURITY.md) — everything else to [yours@innernet.live](mailto:yours@innernet.live).

<p align="center"><sub>© 2026 innernet · <a href="https://innernet.live">innernet.live</a></sub></p>

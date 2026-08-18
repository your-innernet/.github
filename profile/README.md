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

- **one memory** — it lives at innernet.live, not on a machine. every tool you connect reads and writes the same one; there is no local copy to keep in sync.
- **maintained** — you don't write memory files. netti captures as you work and folds it in afterwards. a dimension describes the present; what a change supersedes is replaced and recorded as one dated line under its `## history`.
- **versioned** — commits, branches, merges. fork a direction, park it, fold it back. git for thinking.
- **everywhere** — Claude Code, Cursor, Codex, Windsurf, Gemini CLI, Claude Desktop, VS Code, Cline, Zed, ChatGPT — any MCP client, live. no copy-paste between tools.
- **yours** — private by default, disclosure-gated, exportable. memory is the artifact, and it belongs to you.

### connect

one command wires every AI tool on your machine:

```bash
npx innernet
```

it signs you in once, writes the config for each tool it finds, and — inside a repo — gives that folder a memory of its own. prefer to do it by hand? every MCP client takes the same URL, and signs in in the browser:

```json
{
  "mcpServers": {
    "innernet": { "type": "http", "url": "https://innernet.live/api/mcp" }
  }
}
```

per-client wiring lives in the [docs](https://innernet.live/docs/connect).

### where the code is

the product is built in a private monorepo while the foundations settle — TypeScript end to end: a Next.js platform on Supabase, the `innernet` CLI on npm, and one hosted MCP server exposing the full memory surface (35 tools across projects, personal memory, artifacts, and tasks, each with a REST twin at `/api/v1`). what ships and why is public on the [company page](https://innernet.live/company).

found something that looks wrong from the outside? security reports go to [SECURITY.md](https://github.com/your-innernet/.github/blob/main/SECURITY.md) — everything else to [yours@innernet.live](mailto:yours@innernet.live).

<p align="center"><sub>© 2026 innernet · <a href="https://innernet.live">innernet.live</a></sub></p>

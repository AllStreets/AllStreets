<div align="center">

### Connor Evans

**I build control planes for untrusted autonomous agents.**

<em>capability gating &nbsp;·&nbsp; kill switches &nbsp;·&nbsp; audit ledgers &nbsp;·&nbsp; graduated autonomy</em>

<br/>

<img alt="focus" src="https://img.shields.io/badge/focus-agent_safety_%26_control-b48bff?style=for-the-badge&labelColor=0a0712"/>
<img alt="stack" src="https://img.shields.io/badge/stack-Rust_%C2%B7_Python_%C2%B7_TypeScript-6b7382?style=for-the-badge&labelColor=0a0712"/>
<img alt="bias" src="https://img.shields.io/badge/bias-local--first_%C2%B7_offline-6b7382?style=for-the-badge&labelColor=0a0712"/>

</div>

---

## The through-line

I built four systems over five months without planning them as a set. They converged on the
same architecture anyway, and I only noticed afterwards:

| | LOOM | ONEXUS | WFR | SMADP |
|---|---|---|---|---|
| **declare capability first** | organ manifest | Aegis manifest | tool policy | agent profile |
| **gate before execution** | sandbox validation | `check_capability` | trust gate | tripwire engine |
| **revoke while running** | per-organ, live | `revoke()` | kill switch + halt | stale on drift |
| **bound the spend** | per-organ budget | trust tiers | cost ledger | judge triage |
| **write down what happened** | git timeline | Chronicle | route ledger | chronicle log |
| **earn autonomy, don't grant it** | consent cards | suggest → autonomous | trust sentinel | evidence ladder |

Every one of them is the same bet: an autonomous agent should have to say what it needs before
it runs, be refused when it asks for more, be stoppable mid-flight, and leave a record you can
read afterwards. I find that more interesting than making agents capable, because capability is
the part that's already working.

---

## Selected work

**Scout** &nbsp;·&nbsp; <sub>Flexport · internal · 30+ countries</sub>
<br/>I was hired as an inbound SDR and selected to lead workflow automation and Clay-based data
enrichment for the sales organisation. That mandate became Scout: prospect discovery, account
intelligence and enrichment pipelines consolidated into one internal platform, comparable in scope to
LinkedIn Sales Navigator. It is now used by Flexport sales employees in more than 30 countries, and my
team has held 100% of quota throughout. The only system on this page whose adoption was decided by
other people.


**[ONEXUS](https://github.com/AllStreets/ONEXUS)** &nbsp;·&nbsp; <sub>Python · 1,353 tests</sub>
<br/>A local-first agent runtime built around **Aegis**, a capability arbiter. An agent declares
filesystem reach, outbound domains and tools in a manifest; every call is checked against it,
allowed or denied, and appended to a ledger that is never rewritten. Trust is earned from recorded
outcomes and decides how much rope a module gets — from *suggest only* up to *fully autonomous*.
A static test AST-parses every kernel module and proves none but Aegis can open a socket.

**[LOOM](https://github.com/AllStreets/loom)** &nbsp;·&nbsp; <sub>Rust · Tauri · TypeScript · 1,315 tests</sub>
<br/>An offline computer that builds itself. Describe a capability in one sentence and a local
model plans it, writes the code *and its tests*, proves the whole thing in a sandbox, repairs its
own failures, commits to a git timeline — then asks permission before the new organ may run.
Powers are declared in a manifest, budgeted, and revocable while running. No cloud, no
subscription; the grid goes down and it still evolves.

**[SMADP](https://github.com/AllStreets/SMADP)** &nbsp;·&nbsp; <sub>Python · Docker · 973 tests</sub>
<br/>*Safe Multi-Agent Deployment Platform.* Nobody has systematically studied what happens when
the coding agent, the browser agent and the email agent all share your filesystem and OAuth
scopes. SMADP publishes that matrix — and grades every claim on a four-rung evidence ladder from
*docs-only* to *executed-in-sandbox*. Eleven pairs have actually been run against each other;
2,268 are labelled priors, in the data rather than in a footnote. The ladder is the contribution.

**[AUSPEX](https://github.com/AllStreets/AUSPEX)** &nbsp;·&nbsp; <sub>JavaScript · Three.js · 134 tests · live</sub>
<br/>A living globe of the planet's perils and breakthroughs, free and login-free. Autonomous
pipelines read USGS, GDACS, NASA FIRMS, Launch Library and global RSS, score each event for
severity *and* confidence, and render it honestly — calm where the world is calm, red reserved for
real danger, good news carried beside the bad. Built against the doom-optimised feed.

**[ONEXUS-Agents](https://github.com/AllStreets/ONEXUS-Agents)** &nbsp;·&nbsp; <sub>Python · Astro · live</sub>
<br/>The catalog the runtime reaches for. Nightly GitHub and Hugging Face crawl, with the ranking
weights **published in source** — log-normalised popularity, a 90-day recency half-life, archived
and template penalties — so any score can be recomputed independently rather than trusted.

**[EMBER](https://github.com/AllStreets/ember)** &nbsp;·&nbsp; <sub>vanilla JS · no build step</sub>
<br/>An offline survival console for the day the network isn't there. A local LLM advisor, 38 field
guides, offline navigation, a solar power budget, and a Forge that rewrites the console's own code
from a plain-language prompt. Genuinely zero external requests — the only thing it ever talks to
is `localhost`.

---

<div align="center">
<sub>Numbers here are ones I ran, not ones I estimated. Where a project publishes a large figure,
the README beside it says how much was verified and how much was inferred.</sub>
</div>

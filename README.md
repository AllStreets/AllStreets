<div align="center">

<br/>

# Connor Evans

### I build control planes for untrusted autonomous agents.

<sub><em>capability gating &nbsp;·&nbsp; kill switches &nbsp;·&nbsp; audit ledgers &nbsp;·&nbsp; graduated autonomy</em></sub>

<br/>

<img alt="tests" src="https://img.shields.io/badge/4%2C977-tests_run_not_estimated-4ADE80?style=for-the-badge&labelColor=0a0712"/>
<img alt="scout" src="https://img.shields.io/badge/30%2B-countries_running_Scout-D3A158?style=for-the-badge&labelColor=0a0712"/>
<img alt="lines" src="https://img.shields.io/badge/311k-lines_written-b48bff?style=for-the-badge&labelColor=0a0712"/>

<sub>Chicago, IL &nbsp;·&nbsp; <a href="mailto:connorevans29@gmail.com">connorevans29@gmail.com</a></sub>

<br/>
</div>

---

## The through-line I didn't plan

I built four of these over five months without intending them as a set. They converged on the
same architecture anyway, in three different languages, and I only noticed once I put them
side by side.

```
                          ┌──────────────────────────────────────────┐
   an agent wants to      │  1  declare it first ....... manifest    │
   do something           │  2  gate it ................ arbiter     │
          │               │  3  bound the spend ........ budget      │
          └──────────────▶│  4  stop it mid-flight ..... revoke      │
                          │  5  write down what happened ledger      │
                          │  6  earn the next rung ..... trust       │
                          └──────────────────────────────────────────┘
                                             │
             ┌───────────────┬───────────────┼───────────────┐
             ▼               ▼               ▼               ▼
           LOOM           ONEXUS            WFR            SMADP
        Rust · TS         Python         TypeScript    Python · Docker
```

| | LOOM | ONEXUS | WFR | SMADP |
|---|---|---|---|---|
| **declare first** | organ manifest | Aegis manifest | tool policy | agent profile |
| **gate** | sandbox validation | `check_capability` | trust gate | tripwire engine |
| **revoke live** | per-organ | `revoke()` | kill switch + halt | stale on drift |
| **bound spend** | per-organ budget | trust tiers | cost ledger | judge triage |
| **record it** | git timeline | Chronicle | route ledger | chronicle log |
| **earn autonomy** | consent cards | suggest → autonomous | trust sentinel | evidence ladder |

Every one is the same bet: an agent should have to say what it needs before it runs, be refused
when it asks for more, be stoppable mid-flight, and leave a record you can read afterwards. I
find that more interesting than making agents capable, because capability is the part that
already works.

---

## Selected work

<table>
<tr><td width="150" valign="top">

**[Scout](https://github.com/AllStreets)**
<br/><sub>`Flexport · internal`</sub>
<br/><sub>`30+ countries`</sub>

</td><td valign="top">

Hired as an inbound SDR, then selected to lead workflow automation and Clay-based enrichment for
the sales organization. That mandate became Scout: prospect discovery, account intelligence and
enrichment pipelines in one internal platform, comparable in scope to LinkedIn Sales Navigator.
Now used by Flexport sales employees in **more than 30 countries**; my team has held 100% of quota
throughout.

*The only system here whose adoption was decided by other people.*

</td></tr>
<tr><td width="150" valign="top">

**[ONEXUS](https://github.com/AllStreets/ONEXUS)**
<br/><sub>`Python`</sub>
<br/><sub>`1,366 tests`</sub>

</td><td valign="top">

A local-first agent runtime built on **Aegis**, a 786-line capability arbiter. An agent declares
filesystem reach, outbound domains and tools in a manifest; every call is checked against it,
allowed or denied, and appended to a ledger that is never rewritten. A static test AST-parses
every kernel module and proves none but Aegis can open a socket.

Then I [red-teamed it](https://github.com/AllStreets/ONEXUS/blob/main/docs/REDTEAM-AEGIS.md),
found that `revoke()` did not actually stop an agent holding a grant, fixed it, and published the
six attacks that failed alongside the three that landed.

</td></tr>
<tr><td width="150" valign="top">

**[LOOM](https://github.com/AllStreets/loom)**
<br/><sub>`Rust · Tauri · TS`</sub>
<br/><sub>`1,315 tests`</sub>

</td><td valign="top">

An offline computer that builds itself. Describe a capability in one sentence and a local model
plans it, writes the code *and its tests*, proves it in a sandbox, repairs its own failures over
bounded rounds, and commits to a git timeline. It then asks permission before the new organ may run.
Powers are declared, budgeted and revocable while running. No cloud, no subscription, no telemetry.

</td></tr>
<tr><td width="150" valign="top">

**[SMADP](https://github.com/AllStreets/SMADP)**
<br/><sub>`Python · Docker`</sub>
<br/><sub>`973 tests`</sub>

</td><td valign="top">

*Safe Multi-Agent Deployment Platform.* Nobody has systematically studied what happens when the
coding agent, the browser agent and the email agent all share your filesystem and OAuth scopes.
SMADP publishes that matrix, with a tripwire engine that halts a run mid-flight when a planted
secret leaks or egress steps outside the allowlist.

Every verdict carries its evidence rung as a field on the record. **Eleven** pairs have actually
been executed against each other; 2,268 are labeled priors, in the data rather than a footnote.

</td></tr>
<tr><td width="150" valign="top">

**[AUSPEX](https://github.com/AllStreets/AUSPEX)**
<br/><sub>`JS · Three.js`</sub>
<br/><sub>`134 tests · live`</sub>

</td><td valign="top">

A living globe of the planet's perils **and** its breakthroughs, free and login-free. Autonomous
pipelines read USGS, GDACS, NASA FIRMS, Launch Library and global RSS, score each event for
severity *and* confidence, and render it honestly: calm where the world is calm, red reserved for
genuine danger. The disaster path needs zero API keys, which is what lets it stay free.

</td></tr>
<tr><td width="150" valign="top">

**[HYPERION](https://github.com/AllStreets/GAM3)**
<br/><sub>`Next.js · Three.js`</sub>
<br/><sub>`511 tests`</sub>

</td><td valign="top">

A browser game about running a private orbital agency over a living Earth, with real orbital
mechanics, real world events, and a world that keeps evolving while you are offline. A scheduled server tick
advances every away player's world, so you return to a digest of what changed without you.

</td></tr>
<tr><td width="150" valign="top">

**[Flexport SDR Console](https://github.com/AllStreets/Flexport-sales-dashboard)**
<br/><sub>`React · Express`</sub>
<br/><sub>`19,219 lines`</sub>

</td><td valign="top">

I wanted to work in freight forwarding, so instead of writing a cover letter I built the tool the
job would need: ICP-scored prospects, live AIS vessel positions, live ADS-B aircraft, port-congestion
rings, FRED macro data and tariff tables in one console. The working core came together in a
**30-hour weekend** before my final interviews. I kept building it after, and ran it in production
for my own team.

</td></tr>
<tr><td width="150" valign="top">

**[EMBER](https://github.com/AllStreets/ember)**
<br/><sub>`vanilla JS`</sub>
<br/><sub>`0 external requests`</sub>

</td><td valign="top">

An offline survival console for the day the network isn't there: a local LLM advisor, 38 field
guides, offline navigation, a solar power budget, and a Forge that rewrites the console's own code
from a plain-language prompt. Genuinely zero external requests; the only thing it ever talks to
is `localhost`.

</td></tr>
</table>

---

<div align="center">
<sub>Numbers here are ones I ran, not ones I estimated. Where a project publishes a large figure,<br/>
the README beside it says how much was verified and how much was inferred.</sub>
</div>

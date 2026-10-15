<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/header-dark.svg">
  <img alt="Connor Evans, design engineer in Chicago" src="assets/header-light.svg" width="100%">
</picture>

I design and build interfaces where the detail is the product: real-time 3D, information-dense tools, and software with AI inside it. I work from typography and motion down to shaders and frame budgets, because that is where an interface earns trust.

Two convictions run through the work. An interface should survive close inspection. Software that acts for you should show its work and let you take it back.

At Flexport, alongside my sales role, I was picked to lead workflow automation for the sales team. That became **Scout**, an internal tool now used by Flexport sales teams in more than 30 countries. Before that, I founded two small software companies while studying at UNC.

<br/>

### Selected work

<table>
<tr>
<td width="50%" valign="top">
<a href="https://chicago-open-world.vercel.app"><img src="assets/chicago.webp" width="100%" alt="Chicago Open World: the camera drifts around the skyline at dusk, seen from over Lake Michigan"/></a>
<h3><a href="https://chicago-open-world.vercel.app">Chicago Open World</a></h3>
<em>A city you can fly through.</em>
<p>All of Chicago in 3D, built from City of Chicago and OpenStreetMap data. More than 100,000 buildings stand at their true heights and light up floor by floor as the real sun goes down. On nights a Chicago team wins, the skyline wears its colors.</p>
<sub><a href="https://chicago-open-world.vercel.app">Live&nbsp;↗</a>&emsp;<a href="https://github.com/AllStreets/Chicago-Open-World">Code&nbsp;↗</a>&emsp;<code>React</code> <code>Three.js</code> <code>GLSL</code></sub>
</td>
<td width="50%" valign="top">
<a href="https://f1-pixel-cup.vercel.app"><img src="assets/f1.webp" width="100%" alt="F1 Pixel Cup: the full field fighting through the first corner at Albert Park"/></a>
<h3><a href="https://f1-pixel-cup.vercel.app">F1 Pixel Cup</a></h3>
<em>Arcade racing, played by a real paddock's rules.</em>
<p>The 2025 grid on all 24 circuits of the calendar, traced from their real layouts. Rain, night races, and power-ups that recast Mario Kart items as F1 rules. An unofficial fan project.</p>
<sub><a href="https://f1-pixel-cup.vercel.app">Live&nbsp;↗</a>&emsp;<a href="https://github.com/AllStreets/F1PixelCup">Code&nbsp;↗</a>&emsp;<code>Three.js</code> <code>Canvas</code></sub>
</td>
</tr>
<tr>
<td width="50%" valign="top">
<a href="https://coranto-production.up.railway.app"><img src="assets/coranto.webp" width="100%" alt="CORANTO: the globe turning under live headlines, each pinned to the place it happened"/></a>
<h3><a href="https://coranto-production.up.railway.app">CORANTO</a></h3>
<em>The news, placed on the planet.</em>
<p>Live headlines on a 3D globe, each carrying its publisher, link, time and place. Stories are grouped across outlets, a source that goes down says so instead of going quiet, and anything a model wrote is labeled as such.</p>
<sub><a href="https://coranto-production.up.railway.app">Live&nbsp;↗</a>&emsp;<a href="https://github.com/AllStreets/coranto">Code&nbsp;↗</a>&emsp;<code>CesiumJS</code> <code>Node</code> <code>Supabase</code></sub>
</td>
<td width="50%" valign="top">
<a href="https://crucible-weld.vercel.app"><img src="assets/crucible.webp" width="100%" alt="Crucible: scrolling from the instrument record's front page into its trace of every run"/></a>
<h3><a href="https://crucible-weld.vercel.app">Crucible</a></h3>
<em>A lab notebook for AI agents.</em>
<p>Open-source agents, cloned at pinned commits and set against each other on a shared machine. The results read as an editorial record, and every number on the page is a count of rows you can open.</p>
<sub><a href="https://crucible-weld.vercel.app">Live&nbsp;↗</a>&emsp;<code>Next.js</code> <code>Python</code></sub>
</td>
</tr>
</table>

<br/>

### Also built

<table>
<tr>
<td valign="top" width="22%"><b>CHI ATLAS</b></td>
<td valign="top">A mission-control room for one city: live CTA trains, scores and lake conditions on a 3D map of Chicago.</td>
<td valign="top" width="17%"><sub><a href="https://chi-nine-zeta.vercel.app">Live&nbsp;↗</a>&ensp;<a href="https://github.com/AllStreets/chi">Code&nbsp;↗</a></sub></td>
</tr>
<tr>
<td valign="top"><b>GAM3</b></td>
<td valign="top">Run a private orbital agency in the browser, with real orbital mechanics over a live Earth.</td>
<td valign="top"><sub><a href="https://hyperion-flax.vercel.app">Live&nbsp;↗</a>&ensp;<a href="https://github.com/AllStreets/GAM3">Code&nbsp;↗</a></sub></td>
</tr>
<tr>
<td valign="top"><b>ONEXUS Agents</b></td>
<td valign="top">An evidence-graded catalog of open-source AI agents, ranked by published weights, with every claim labeled by how it was verified.</td>
<td valign="top"><sub><a href="https://onexus-agents.vercel.app">Live&nbsp;↗</a>&ensp;<a href="https://github.com/AllStreets/ONEXUS-Agents">Code&nbsp;↗</a></sub></td>
</tr>
<tr>
<td valign="top"><b>loom</b></td>
<td valign="top">An offline computer that extends itself. Describe a capability in one sentence; a local model plans it, writes and tests the code, and asks before it runs.</td>
<td valign="top"><sub><a href="https://github.com/AllStreets/loom">Code&nbsp;↗</a></sub></td>
</tr>
<tr>
<td valign="top"><b>ember</b></td>
<td valign="top">An offline console for when the grid goes down: a local model, field guides and navigation, and not one external request.</td>
<td valign="top"><sub><a href="https://github.com/AllStreets/ember">Code&nbsp;↗</a></sub></td>
</tr>
</table>

<br/>

### Agent safety

Under the interfaces, most of my work asks one question: how does an AI agent earn permission to act, and how do you stop one that shouldn't? [ONEXUS](https://github.com/AllStreets/ONEXUS) is a local-first runtime that checks every tool call against the manifest the agent declared and writes each decision to an audit ledger. I [red-teamed it myself](https://github.com/AllStreets/ONEXUS/blob/main/docs/REDTEAM-AEGIS.md) and published what broke and how I fixed it. [SMADP](https://github.com/AllStreets/SMADP) analyzes agents that share a filesystem, clipboard and OAuth scopes, and grades every verdict by how it was verified.

<br/>

<sub>CONTACT</sub><br/>
[connorevans29@gmail.com](mailto:connorevans29@gmail.com)

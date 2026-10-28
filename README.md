<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/header-dark.svg">
  <img alt="Connor Evans, design engineer in Chicago" src="assets/header-light.svg" width="100%">
</picture>

I design and build interfaces where the detail is the product: real-time 3D, information-dense tools, and software with AI inside it. I work from typography and motion down to shaders and frame budgets, because that is where an interface earns trust.

Two convictions run through my work. An interface should survive close inspection. Software that acts for you should show its work and let you take it back.

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
<a href="https://coranto-production.up.railway.app"><img src="assets/coranto.webp" width="100%" alt="The whole CORANTO window: the globe turns across the dawn line from city lights into daylight over Asia, a click on the Hong Kong story narrows the newsfeed, and the camera flies down over Victoria Harbour"/></a>
<h3><a href="https://coranto-production.up.railway.app">CORANTO</a></h3>
<em>The news, placed on the planet.</em>
<p>Live headlines on a 3D globe, each carrying its publisher, link, time and place. Stories are grouped across outlets, a source that goes down says so instead of going quiet, and anything a model wrote is labeled as such. Built on Bilawal Sidhu's <a href="https://github.com/bilawalsidhu/gods-eye-view">God's Eye View</a>; I added the news layer and the grounded briefs.</p>
<sub><a href="https://coranto-production.up.railway.app">Live&nbsp;↗</a>&emsp;<a href="https://github.com/AllStreets/coranto">Code&nbsp;↗</a>&emsp;<code>CesiumJS</code> <code>Node</code> <code>Supabase</code></sub>
</td>
<td width="50%" valign="top">
<a href="https://github.com/AllStreets/bombechat"><picture><source srcset="assets/bombechat.avif" type="image/avif"><img src="assets/bombechat.webp" width="100%" alt="Bombechat: the drums turning as a message arrives by sound and settles in type, then the cursor opens Settings, the machine turns round to its back panel, and two patch plugs are pulled to new jacks, Send volume from 3 to 5 and Light switch from Off to Read and flash, while the wiring schedule updates beside them"/></picture></a>
<h3><a href="https://github.com/AllStreets/bombechat">Bombechat</a></h3>
<em>Messages that never touch the internet.</em>
<p>Encrypted messages between laptops in the same room, sent by sound on sixteen tones between 17.6 and 19.8 kHz that most adults barely hear, or by light from one screen to the other laptop's camera. Each message is sealed with X25519 and XChaCha20-Poly1305 and signed with Ed25519, and there is no account, no server and no network code in the build. It looks and sounds like the machine Turing designed at Bletchley Park to break Enigma.</p>
<sub><a href="https://github.com/AllStreets/bombechat">Code&nbsp;↗</a>&emsp;<code>Rust</code> <code>Tauri</code> <code>three.js</code> <code>SQLCipher</code></sub>
</td>
</tr>
<tr>
<td width="50%" valign="top">
<a href="https://github.com/AllStreets/teardown"><img src="assets/teardown.webp" width="100%" alt="Teardown reading the Claude desktop app: the overview of every installed app, then a radial map of Claude's bundle with its largest parts labelled"/></a>
<h3><a href="https://github.com/AllStreets/teardown">Teardown</a></h3>
<em>Every app on your Mac, taken apart.</em>
<p>Reads each installed app the way a reverse engineer would, with Apple's own tools, and explains it in plain English with the evidence beside every claim. Then it lets you act: roll back an update, take back a permission, switch off a background service. On my Mac it found 21 separate copies of Chromium.</p>
<sub><a href="https://github.com/AllStreets/teardown">Code&nbsp;↗</a>&emsp;<code>TypeScript</code> <code>Rust</code> <code>React</code></sub>
</td>
<td width="50%" valign="top">
<a href="https://github.com/AllStreets/ONEXUS"><img src="assets/onexus.webp" width="100%" alt="ONEXUS in one take: a request to refactor the kernel runtime is typed and sent, Cortex routes it to Council and the whole window warms from calm teal to deliberating red, Council asks to write nexus/kernel/cortex.py, Allow once clears the request, and a thumbs-up lifts the trust rail"/></a>
<h3><a href="https://github.com/AllStreets/ONEXUS">ONEXUS</a></h3>
<em>AI agents you can watch think.</em>
<p>A local-first runtime for AI agents. Every tool call is checked against the manifest the agent declared and written to a hash-chained ledger, and I attacked it myself in three published red-team rounds; the last put launched agents in a locked-down container behind an egress proxy. The 53 agents in its store install that way, with none of your files and only the hosts you approve. Its public catalog, <a href="https://onexus-agents.vercel.app">ONEXUS Agents</a>, ranks more than 5,000 open-source agents and says how each one was verified.</p>
<sub><a href="https://github.com/AllStreets/ONEXUS/blob/main/docs/REDTEAM-AEGIS.md">Red-team&nbsp;↗</a>&emsp;<a href="https://github.com/AllStreets/ONEXUS">Code&nbsp;↗</a>&emsp;<a href="https://onexus-agents.vercel.app">Catalog&nbsp;↗</a></sub>
</td>
</tr>
</table>

<br/>

### Also built

<table>
<tr>
<td width="50%" valign="top">
<h4><a href="https://github.com/AllStreets/Assay">Assay</a></h4>
A bill of materials for the whole Mac. It reads every app, AI model, extension and package down to the libraries inside, checks each against published advisories, and catches a model that would run code before anything loads it. Flaws are ranked by what each app can actually reach.
<br/><sub><a href="https://github.com/AllStreets/Assay">Code&nbsp;↗</a></sub>
</td>
<td width="50%" valign="top">
<h4><a href="https://edm-daw.vercel.app">EDM-DAW</a></h4>
A music studio in a browser tab. Describe a song and Claude builds it as sections you can edit, or work in a full DAW with an AI companion whose every change you can accept or undo.
<br/><sub><a href="https://edm-daw.vercel.app">Live&nbsp;↗</a>&emsp;<a href="https://github.com/AllStreets/edm-daw">Code&nbsp;↗</a></sub>
</td>
</tr>
<tr>
<td width="50%" valign="top">
<h4><a href="https://crucible-weld.vercel.app">Crucible</a></h4>
A lab notebook for AI agents. Open-source agents, cloned at pinned commits, are set against each other on a shared machine, and the results read as an editorial record where every number on the page is a count of rows you can open.
<br/><sub><a href="https://crucible-weld.vercel.app">Live&nbsp;↗</a>&emsp;<a href="https://github.com/AllStreets/crucible">Code&nbsp;↗</a></sub>
</td>
<td width="50%" valign="top">
<h4><a href="https://github.com/AllStreets/ember">ember</a></h4>
An offline survival console for when the grid goes down: a local AI advisor, field guides, offline maps and a solar power budget, with no outside requests. Its Forge rewrites the console's own code from a plain request and shows every check and the diff before saving.
<br/><sub><a href="https://github.com/AllStreets/ember">Code&nbsp;↗</a></sub>
</td>
</tr>
</table>

<br/>

See my portfolio, on a 3D globe, at **[connor-evans.vercel.app](https://connor-evans.vercel.app)**.

<br/>

### Agent safety

Under the interfaces, most of my work asks one question: how does an AI agent earn permission to act, and how do you stop one that shouldn't? [ONEXUS](https://github.com/AllStreets/ONEXUS), above, is my answer for a single machine, and its [red-team](https://github.com/AllStreets/ONEXUS/blob/main/docs/REDTEAM-AEGIS.md) says plainly what it still doesn't protect. I started measuring how agents treat each other with [SMADP](https://allstreets.github.io/SMADP/), which estimated the risk of every pair from their documentation. Estimates scale, but nobody can check one, so I built [Crucible](https://crucible-weld.vercel.app) to run real agents against each other and publish what they actually did, down to every run.

<br/>

### Contact:

connorevans29@gmail.com

<a href="mailto:connorevans29@gmail.com"><picture><source media="(prefers-color-scheme: dark)" srcset="assets/email-dark.svg"><img src="assets/email-light.svg" height="44" alt="Send an email to connorevans29@gmail.com"></picture></a>

<!--
  davephoenix360 — GitHub profile README
  Theme: retro arcade / CRT / pixel
  No build step; HTML+CSS in a markdown HTML block.
  Live dynamic widgets: typing SVG, visitor counter, streak, trophies, stats.
-->

<!-- Load a pixel font for any inline text + a mono for stats -->
<link rel="preconnect" href="https://fonts.googleapis.com" />
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
<link href="https://fonts.googleapis.com/css2?family=Press+Start+2P&family=VT323&family=JetBrains+Mono:wght@400;700&display=swap" rel="stylesheet" />

<style>
  /* === CRT scanline overlay across the whole README === */
  /* The host page is a <div> GitHub renders. We paint a subtle scanline
     pattern into the README container. Low opacity, fixed position. */
  .markdown-body,
  article {
    position: relative;
  }
  .markdown-body::after,
  article::after {
    content: "";
    position: fixed;
    inset: 0;
    pointer-events: none;
    background: repeating-linear-gradient(
      to bottom,
      rgba(0, 0, 0, 0) 0,
      rgba(0, 0, 0, 0) 2px,
      rgba(0, 0, 0, 0.08) 3px,
      rgba(0, 0, 0, 0) 4px
    );
    z-index: 9999;
    mix-blend-mode: multiply;
  }
  /* Tiny CRT vignette */
  .markdown-body::before,
  article::before {
    content: "";
    position: fixed;
    inset: 0;
    pointer-events: none;
    background: radial-gradient(ellipse at center, rgba(0,0,0,0) 55%, rgba(0,0,0,0.35) 100%);
    z-index: 9998;
  }
  /* Pixel-rendering of the few headings we write in raw text */
  .pixel {
    font-family: "Press Start 2P", "VT323", monospace;
    letter-spacing: 0.05em;
  }
  .crt-text {
    font-family: "VT323", "JetBrains Mono", monospace;
    color: #39ff14;
    text-shadow: 0 0 1px #39ff14, 0 0 6px rgba(57, 255, 20, 0.35);
  }
  /* "INSERT COIN" pill */
  .coin {
    display: inline-block;
    padding: 6px 14px;
    margin: 2px 4px;
    border: 2px solid #ffcc00;
    color: #ffcc00;
    font-family: "Press Start 2P", monospace;
    font-size: 10px;
    text-decoration: none;
    background: rgba(255, 204, 0, 0.06);
    box-shadow: 0 0 0 2px #000, 0 0 12px rgba(255, 204, 0, 0.4);
    transition: transform 0.15s ease;
  }
  .coin:hover { transform: translateY(-1px) scale(1.04); color: #fff; }
  .coin.ghost { border-color: #00ffff; color: #00ffff; background: rgba(0,255,255,0.06); box-shadow: 0 0 0 2px #000, 0 0 12px rgba(0,255,255,0.35); }
  .coin.heart { border-color: #ff3131; color: #ff3131; background: rgba(255,49,49,0.06); box-shadow: 0 0 0 2px #000, 0 0 12px rgba(255,49,49,0.35); }
  /* "ACHIEVEMENT UNLOCKED" badge */
  .achievement {
    display: inline-block;
    padding: 2px 8px;
    margin-right: 6px;
    background: #39ff14;
    color: #000;
    font-family: "Press Start 2P", monospace;
    font-size: 9px;
    border: 2px solid #000;
    box-shadow: 3px 3px 0 #000;
  }
  /* Pixel block divider */
  .block-divider { color: #39ff14; opacity: 0.7; }
  /* Tables = leaderboard look */
  .markdown-body table {
    border-collapse: collapse;
  }
  .markdown-body table th,
  .markdown-body table td {
    border: 1px solid #39ff14 !important;
    padding: 8px 12px !important;
  }
  .markdown-body table th {
    background: #0d0d0d;
    color: #ffcc00;
    font-family: "Press Start 2P", monospace;
    font-size: 10px;
  }
</style>

<div align="center">

```
██╗  ██╗██╗███████╗██████╗ ██████╗ ███████╗██╗   ██╗███████╗
██║  ██║██║██╔════╝██╔══██╗██╔══██╗██╔════╝╚██╗ ██╔╝██╔════╝
███████║██║█████╗  ██████╔╝██████╔╝█████╗    ╚████╔╝ █████╗  
██╔══██║██║██╔══╝  ██╔═══╝ ██╔══██╗██╔══╝      ╚██╔╝  ██╔══╝  
██║  ██║██║███████╗██║     ██║  ██║███████╗     ██║   ███████╗
╚═╝  ╚═╝╚═╝╚══════╝╚═╝     ╚═╝  ╚═╝╚══════╝     ╚═╝   ╚══════╝
```

> <sub><b>↑ yes, I drew that in ASCII. yes, by hand. yes, I'm procrastinating.</b></sub>

</div>

<br />

<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Press+Start+2P&size=18&duration=3000&pause=1200&color=39FF14&center=true&vCenter=true&width=600&height=80&lines=PLAYER+1+:+DIEPREYE;SOFTWARE+ENGINEER+%40+UALBERTA;BACKEND+%2F+DEVOPS+%2F+SYSTEMS;I+BUILD+STUFF+THAT+DOES+THINGS" alt="Typing SVG" />

</div>

<br />

<div align="center">

<!-- INSERT COIN: visitor counter styled as an arcade status bar -->
<a href="https://diepreyecd.dev">
  <img src="https://komarev.com/ghpvc/?username=davephoenix360&label=PLAYERS+WHO+ENTERED&color=39ff14&style=flat-square" alt="profile views" />
</a>
<a href="https://github.com/davephoenix360?tab=followers">
  <img src="https://img.shields.io/github/followers/davephoenix360?style=flat-square&label=FOLLOWERS&color=ffcc00" alt="followers" />
</a>
<a href="https://github.com/davephoenix360">
  <img src="https://img.shields.io/github/stars/davephoenix360?style=flat-square&label=STARS&color=00ffff" alt="stars" />
</a>

</div>

<br />

<div align="center">

### <span class="pixel">▼ ACHIEVEMENTS UNLOCKED ▼</span>

| 🏆 Trophy | Status |
|:--|:--|
| 🪪 SWE @ UAlberta | `IN PROGRESS · 90/120 credits` |
| 🛠️ Shipped Nextep, DragonShell, MapReduce, Streamer U. | `+1,247,398 XP` |
| ☕ Coffee dependency | `STACK OVERFLOW RISK` |
| 🌙 Sleep schedule | `NOT IN TOP 3` |
| 📫 Replied to recruiter within 24h | `RARE DROP` |

</div>

<br />

---

### <span class="pixel">▶ INSERT COIN TO CONTINUE</span>

<a class="coin" href="https://diepreyecd.dev">▶ PORTFOLIO</a>
<a class="coin ghost" href="https://www.linkedin.com/in/diepreyecd/">▶ LINKEDIN</a>
<a class="coin heart" href="mailto:davediepreye05@gmail.com">▶ SEND EMAIL</a>
<a class="coin" href="https://github.com/davephoenix360/Portfolio-Website">▶ SOURCE OF THIS PAGE</a>

<br />

---

### <span class="pixel">▶ HIGH SCORES</span>

<div align="center">

<!-- Profile stats card (big + bold) -->
<img src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=davephoenix360&theme=radical&hide_border=true" alt="Profile Details" />

<br />

<!-- Most-used language, productive hours, repos-per-language (the "trophies" replacement) -->
<img height="180" src="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=davephoenix360&theme=radical&hide_border=true" alt="Top Language" />
<img height="180" src="https://github-profile-summary-cards.vercel.app/api/cards/stats?username=davephoenix360&theme=radical&hide_border=true" alt="Stats" />
<img height="180" src="https://github-profile-summary-cards.vercel.app/api/cards/productive-time?username=davephoenix360&theme=radical&hide_border=true&utcOffset=-7" alt="Productive Time" />

<br />

<!-- Year-of-commits activity graph (the new "streak" — shows the whole year in one go) -->
<img src="https://github-readme-activity-graph.vercel.app/graph?username=davephoenix360&theme=radical&hide_border=true&area=true" alt="Activity Graph" />

<br />

<!-- Compact stats: total commits, PRs, issues, etc. (the retro-classic) -->
<img height="155" src="https://github-readme-stats.vercel.app/api?username=davephoenix360&show_icons=true&theme=radical&hide_border=true&bg_color=0d0d0d&title_color=ffcc00&icon_color=39ff14&text_color=ffffff" alt="GitHub Stats" />
<img height="155" src="https://github-readme-stats.vercel.app/api/top-langs/?username=davephoenix360&layout=compact&theme=radical&hide_border=true&bg_color=0d0d0d&title_color=ffcc00&text_color=ffffff" alt="Top Langs" />

</div>

<br />

<div align="center">

<sub><i>school run — separate save file</i></sub>

<img height="145" src="https://github-readme-stats.vercel.app/api?username=DIEPREYECD&show_icons=true&theme=tokyonight&hide_border=true&hide_title=true" alt="School Stats" />
<img height="145" src="https://github-readme-stats.vercel.app/api/top-langs/?username=DIEPREYECD&layout=compact&theme=tokyonight&hide_border=true&hide_title=true" alt="School Langs" />

</div>

---

### <span class="pixel">▶ EQUIPMENT LOADOUT</span>

<div align="center">

<a href="https://skillicons.dev">
  <img src="https://skillicons.dev/icons?i=python,ts,js,java,cpp,c,cs,react,nodejs,express,postgres,mysql,aws,gcp,docker,kubernetes,terraform,linux,git,githubactions,threejs,tailwind" />
</a>

</div>

<br />

```
loadout: software engineer | difficulty: senior year
primary:   backend services, APIs, CI/CD
secondary: cloud (aws/gcp), databases, linux
loot:      PHP/WordPress (legacy), Unity (side-quest), three.js (new hobby)
```

---

### <span class="pixel">▶ BOSS RUNS (selected)</span>

| 🎮 Quest | 🎯 Objective | ⭐ Outcome |
|---|---|---|
| **Nextep** *(private dev)* | Chrome ext. for job-application automation (WXT, TS) | Lvl. up. **Source not public yet — ask me about it.** |
| [**DragonShell**](https://github.com/DIEPREYECD/dragonshell-f25-DIEPREYECD) | Custom Unix shell (jobs, concurrency) | Beat the boss. Lost a few lives to segfaults. |
| [**MapReduce / fs-sim**](https://github.com/DIEPREYECD/assignment2-mapreduce-DIEPREYECD) | Threadpool + filesystem simulation | Speedrun clear. Race conditions were the wall-jump section. |
| [**Streamer University**](https://github.com/DIEPREYECD/CMPUT-250-Project) | Unity event-card system + minigames | Co-op clear. [Play it.](https://diepreyecdd.itch.io/streamer-university) |

---

### <span class="pixel">▶ ACTIVE QUESTS (TODAY)</span>

- 📚 Finishing the SWE degree (graduating May 2027, cross your fingers)
- 💼 Wrangling internship things (will share when it's shareable)
- 🛠️ Building tools I wish someone else had already built
- 🏃 Staying alive (fitness, sleep, the basics)

---

### <span class="pixel">▶ GUILD</span>

- 🏛️ **BESA (Black Engineering Students' Association @ UAlberta)** — VP Academics, run mentorship + pro-dev events, made some marketing pixels move
- 🧭 Care about **clarity + velocity**: docs, defaults, fewer "ask three seniors" bottlenecks

---

<div align="center">

### <span class="pixel">▶ PLAYER 1'S CURRENTLY PLAYING</span>

<a href="https://open.spotify.com/" target="_blank">
  <img src="https://img.shields.io/badge/Spotify-1ED760?style=for-the-badge&logo=spotify&logoColor=black" alt="Spotify" />
</a>

<sub><i>♪ something with a beat, probably. maybe lo-fi. definitely not silence.</i></sub>

<sub><i>(replace the URL above with your Spotify profile link — or remove this whole block if you don't want it)</i></sub>

</div>

<br />

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=39ff14&height=120&section=footer&text=THANKS%20FOR%20PLAYING&fontSize=30&fontColor=ffcc00&fontAlignY=70" alt="Footer" />

<sub><b><span class="crt-text">▶ HIGH SCORE SAVED · 2026</span></b></sub>

<sub><i>built with HTML, a pixel font, and too much coffee ·</i></sub>

</div>

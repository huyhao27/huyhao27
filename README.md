<h1 align="center">
  <a href="https://git.io/typing-svg">
    <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&weight=600&size=30&pause=1000&color=F75C7E&center=true&vCenter=true&width=435&lines=Hi+I'm+Nguyen+Huy+Hao;Unity+Developer;Software+Engineering+Student;Game+Enthusiast" alt="Typing SVG" />
  </a>
</h1>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=huyhao27&label=Profile%20Views&color=0e75b6&style=flat" alt="huyhao27" />
</p>

<p align="center">
  <em>"NHH"</em>
</p>

---

# Nguyen Huy Hao

**Unity Developer @ Sonat Game Studio** · Hanoi, Vietnam

I build casual and puzzle mobile games in Unity / C#, and the level tooling behind them —
editors, validators and difficulty simulation that let designers ship content without opening Unity.

[LinkedIn](https://www.linkedin.com/in/hao-nguyen-huy-aaa746437/) · [Email](mailto:hao.k19.fpthola@gmail.com)

---

## Shipped Games

| Game | Links | My work |
|---|---|---|
| **Bubble Fish: Sort Puzzle**<br/>Triple-match sort puzzle | [Google Play](https://play.google.com/store/apps/details?id=com.bubble.fish.sort.puzzle) · [App Store](https://apps.apple.com/app/id6813802366) | Gameplay, level pipeline, level validation, DDA |
| **Cozy Life: Decor Room**<br/>Unpacking & room-decoration puzzle · 100K+ downloads | [Google Play](https://play.google.com/store/apps/details?id=com.unpacking.cozy.home.dream) · [App Store](https://apps.apple.com/app/id6744342887) | Gameplay, playtest & level tooling |

## Level Design Tooling — Bubble Fish

A browser-based **Level Studio** (Python + vanilla JS) used by game designers and marketing
to build, check and tune 1,300+ levels without Unity.

**Level editor**
- Edit bubbles, fish, capacities and 15 level mechanics (frozen, locked/key, hidden fish, …) with undo, hotkeys and multi-select
- In-browser playtest that mirrors the in-game board, trays and waiting queue
- Batch export straight into the Unity project's Addressables folder, with deterministic `.meta` GUIDs so re-exports never break references

**Validation**
- Validator ported 1:1 from the game's C# `LevelDataValidator` — one rule set shared by the CLI, the web editor and the runtime
- Audited the rules against real gameplay code: removed three rules inherited from ball-sort that falsely failed valid levels, and promoted fish overflow to an error after finding it silently made levels unbeatable
- Greedy solver checks every level is clearable before it ships

**Dynamic difficulty (DDA)**
- Tray-order model that picks the next fish species from live board, queue and pending-bubble pools
- Feasibility filter so a tray is only ever ordered when enough fish remain to fill it
- Five-tier priority by fish availability, with deterministic tie-breaks and no duplicate species across trays
- DDA certification panel that simulates levels under the game's rules to check difficulty before release

## Other Tools

- **Playtest & level tool (Cozy Life)** — imports artist PSB/PSD files and rebuilds levels, sprites and boards automatically; in-tool editor; exports sync straight into Unity
- **Haptics module** — cross-platform haptics bridge with an on-device companion app for tuning feedback on real hardware

## Non-Unity Project

**Dream Coffee** — PC game (`.exe`) built with [engine/framework]
- [One line: genre / what the game is]
- Storefront: Astro + Hono + React on Cloudflare Workers (D1, R2), with license-key signing and Playwright E2E tests

## Game Jams

- **[SeeeJam](https://github.com/huyhao27/SeeeJam)** — BKU Game Jam
- **[Gametopia]([link])** — [one line]
- **[Game Jam 2026]([link])** — [one line]

## Tech

**Game:** C# · Unity · Addressables · DOTween · Feel
**Tooling:** Python · JavaScript · PyInstaller
**Web:** TypeScript · Astro · Hono · Cloudflare Workers

---

<sub>Software Engineering student at FPT University (K19).</sub>

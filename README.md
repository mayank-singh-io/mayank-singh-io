<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=24&duration=3200&pause=900&color=00E5A0&center=true&vCenter=true&width=640&lines=CS+undergrad+building+privacy+tooling;agent-first%3A+BMAD+Method+%2B+Claude+Code;offline-first+%E2%80%A2+zero+network+egress" alt="intro" />

<a href="mailto:kunwarmayanksingh78@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="email" /></a>
<a href="https://linkedin.com/in/YOUR_LINKEDIN"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="linkedin" /></a>
<img src="https://komarev.com/ghpvc/?username=mayank-singh-io&style=for-the-badge&color=00E5A0&label=VISITORS" alt="views" />

</div>

---

```console
mayank@github:~$ whoami

  name      →  Kunwar Mayank Singh
  role      →  CS undergrad · security & privacy tooling
  based     →  Lucknow, India
  school    →  B.Tech CSE, Chandigarh University (1st year)
  method    →  BMAD (spec → architecture → impl) + Claude Code
  building  →  Cypher — on-device redaction for cloud LLM prompts
  learning  →  DevOps: CI/CD, containers, Linux server admin
  status    →  open to internships & collaborations

mayank@github:~$ _
```

I build things end to end — research and threat modelling through implementation, tests and deployment. Most of it runs **locally**: if a feature can work without touching a network, it does.

I also work **agent-first on every project**. Specs and architecture go through the BMAD Method — including Party Mode sessions that pressure-test designs across specialist agent personas before any code exists — with Claude Code as the implementation and pairing tool, backed by tests and CI gates.

---

### Stack

<div align="center">

<img src="https://skillicons.dev/icons?i=python,ts,js,react,nextjs,nodejs,fastapi,tailwind&theme=dark" alt="stack row 1" />
<br/>
<img src="https://skillicons.dev/icons?i=postgres,supabase,sqlite,docker,git,vercel,cloudflare,linux&theme=dark" alt="stack row 2" />

</div>

<div align="center">
<sub>
<b>also:</b> PyQt5/6 · asyncio · Vitest · WebSocket/REST · Chrome MV3 &amp; Firefox extensions · Ollama &amp; local LLMs · Ed25519 · SQLite WAL/FTS5
</sub>
</div>

---

### Selected work

Several repos below are private while in development — happy to walk through the code or give access on request.

<table>
<tr>
<td width="50%" valign="top">

#### 🔒 Cypher
**Local redaction layer for cloud AI prompts** · `private`

Chrome MV3 extension that tokenises confidential values *before* a prompt leaves the machine and restores them in the streamed reply — so ChatGPT and Claude never receive the identifiers. Patches `window.fetch` in the page world to rewrite both the outgoing body and the incoming SSE stream.

Detection is entirely on-device with **zero network egress, CI-enforced**. A 40 KB two-layer engine runs at **0.031 ms median** per document; **431 tests**, with false positives on clean documents cut from 13 → 1 across a 46-document labelled corpus.

`TypeScript` `Chrome MV3` `SSE` `Vitest`

</td>
<td width="50%" valign="top">

#### 🎙️ Nexus
**Offline personal voice assistant** · `private` · Mar–Jul 2026

Fully offline, **CPU-only** Windows assistant built for constrained hardware (i5-8365U, 16 GB, no GPU): wake word → VAD-gated STT → local LLM routing → streaming TTS, on an async service architecture.

Shipped **12 additive, config-gated phases without a rewrite** — long-term memory (SQLite WAL + FTS5 + vector search), OCR-first screen perception, crash recovery and safe mode, a Fernet secrets vault with key rotation, and sentence-level streaming so speech starts before generation finishes.

`faster-whisper` `OpenWakeWord` `Kokoro TTS` `Ollama` `PyQt5`

</td>
</tr>
<tr>
<td width="50%" valign="top">

#### 🛡️ The Witness
**Verifiable data sanitization & forensic recovery** · `spec + PRD complete`

An erasure platform where **the signed record, not the wipe, is the product**. The tool runs its own forensic carver across the sanitised device and signs whatever it recovers into an Ed25519-signed, hash-chained, offline-verifiable certificate.

Led a **six-person Smart India Hackathon 2026 team** new to development — taught the toolchain from scratch, scoped the PRD into ownable work, reviewed what came back. Specified against NIST SP 800-88r2, IEEE 2883-2022 and the DPDP Rules 2025.

Honest degradation is a hard constraint: a non-conformant certificate is never signed, and a run that reached Clear where Purge was targeted reports that failure at the same visual weight as a success.

`Python 3.12` `FastAPI` `React` `Ed25519`

</td>
<td width="50%" valign="top">

#### 🏗️ Architecture & Engineering Firm Site
**Live production client site** · `confidential`

Built, deployed and maintain the production site for a Lucknow-based architecture and structural engineering practice — 10+ pages with Supabase-backed forms, audience-split conversion paths, SEO/Open Graph metadata and a consent-gated cookie banner.

Responsive component-based pages, optimised image delivery, and ongoing maintenance and content updates.

`Next.js` `React` `Vercel` `Supabase`

</td>
</tr>
</table>

<details>
<summary><b>More things I've built</b></summary>

<br/>

| Project | What it does | Stack |
|---|---|---|
| **PrintGuard** | Windows print monitoring enforcing per-user page limits, with a real-time admin dashboard, CSV usage logging and remote access via Cloudflare Tunnel | `Windows` `System Tray` |
| **Smart Scheduler** | Desktop scheduler with natural-language event input powered by a local LLM; Google Calendar/Gmail integration, companion Discord bot, tray notifications | `Python` `PyQt6` `Ollama` |
| **SyncMesh** | Self-hosted LAN file sync with a browser dashboard and SHA-256 content diffing to minimise transfer overhead | `Node.js` `WebSocket` |
| **Video DownloadHelper — Firefox port** | Ported a Chrome MV3 extension to Firefox across several iterations, resolving cross-browser and CORS issues; added ETA display and duplicate-download detection | `MV3 → Firefox` |
| **WhatsApp Web file-send logger** | Userscript plus backend logger tracking file sends on WhatsApp Web, with real-time push notifications | `Node.js` `Tampermonkey` `ntfy` |

</details>

---

### Focus areas

`offline-first & privacy-preserving design` · `threat modelling` · `applied cryptography — Ed25519, hash chains, checksum validation` · `standards-led specification — NIST SP 800-88r2, IEEE 2883` · `prompt & context engineering`

---

### Activity

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=mayank-singh-io&show_icons=true&theme=dark&bg_color=0D1117&border_color=30363D&icon_color=00E5A0&title_color=00E5A0&text_color=C9D1D9&include_all_commits=true&count_private=true" alt="stats" />
<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=mayank-singh-io&layout=compact&theme=dark&bg_color=0D1117&border_color=30363D&title_color=00E5A0&text_color=C9D1D9&langs_count=8" alt="languages" />

<br/><br/>

<img src="https://streak-stats.demolab.com?user=mayank-singh-io&theme=dark&background=0D1117&border=30363D&ring=00E5A0&fire=00E5A0&currStreakLabel=00E5A0" alt="streak" />

<br/><br/>

<img src="https://raw.githubusercontent.com/mayank-singh-io/mayank-singh-io/output/snake.svg" alt="contribution snake" />

</div>

---

<div align="center">

**Currently open to internships and collaborations** — especially anything touching privacy, local-first systems or security tooling.

<a href="mailto:kunwarmayanksingh78@gmail.com">kunwarmayanksingh78@gmail.com</a>

</div>

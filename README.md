## Hi, I'm Tyler 👋

**Han Tang Lin** · backend engineer in Taipei · former astronomer

- 🧑‍💻 Backend Supervisor at **Pacston**: technical lead on a FastAPI + PostgreSQL platform I architected end to end, leading a backend team of five
- 🔭 Previously an observational astronomer with two first-author papers, on M-dwarf stellar flares (*AJ*) and Type Ia supernova hosts (*MNRAS*)
- 🐛 Most useful where a live system is *quietly wrong under concurrency*: jobs that run three times, locks that aren't there, retries that multiply traffic, tokens nobody verifies
- 🎨 Off-hours: GLSL shaders, React Three Fiber and Blender models, all on [my site](https://tylerastro.dev/en/gallery)
- 🌏 中文 · English · Français · 日本語

### ⚡ Production, by the numbers

- 📈 **1M+ requests / month across 195 REST endpoints** over 44 tables; I wrote ~90% of its 44K production lines
- 🚀 **p99 39.2 s → 1.0 s**: moved a 37-second reconciliation off the request path behind a Postgres advisory lock; slow requests 880 → 19 per day
- 🔁 **3× → exactly once**: traced a triple-firing scheduled job to a trigger timeout colliding with AWS async retries
- 🌊 **418× retry amplification shut down**: 43K requests were fanning out into 18M Lambda invocations
- 🔍 **N+1 hunting**: 1,108 → 6 queries per request (12.3 s → 775 ms) and 244 → 3 (2.6 s → 210 ms) on core endpoints; primary API mean duration −48%, cold-start init −23%

<details>
<summary>More from production</summary>

- 🧯 **Runaway job contained**: production API p99 28.2 s → 9.4 s; 5xx on the affected endpoint 87% → 0%
- 🔐 **JWT verification hardened**: every token now checked for signature and expiry
- 🤝 **100 PRs merged** integrating 2,392 commits from 8 engineers; introduced the team's first CI quality gate and its uv + ruff toolchain

</details>

### 🛠️ Things I've built

- 🔭 **[NCU TOM](https://tom.astro.ncu.edu.tw)**: target & observation manager in production at Lulin Observatory, built solo (FastAPI, PostgreSQL, Next.js). Rebuilt its light-curve plotting on canvas after benchmarking 15 charting libraries: DOM nodes 60,082 → 104 at 20k points · [issue tracker](https://github.com/Tylerastro/NCU_TOM-tracker)
- ⚖️ **[sync-async-k8s-path](https://github.com/Tylerastro/sync-async-k8s-path)**: FastAPI sync vs async measured under Locust load, from CPU-pinned Docker Compose to Kubernetes. Async 512 vs sync 335 RPS, a connection-pool sweep from 167 to 642 RPS, and the single-pod breaking point at 5,000 users · [interactive walkthrough](https://tylerastro.github.io/sync-async-k8s-path/)
- 🤖 **[tylerastro.dev](https://tylerastro.dev)**: my trilingual notebook for code, life and 推し活, with *Tyler-bot*, a streaming chat assistant on the Vercel AI SDK checked by an 80+ case pytest eval suite
- 🎤 **[Utano Track](https://utanotrack.fans)**: 15,000+ fan timestamps from VTuber streams, turned into a clickable song index
- 🎶 **[Let's Sing Together](https://www.lets-sing-together.com/en-US)**: YouTube playback synced line by line to lyrics, for learning Japanese by singing along
- 🗺️ **[Folium Institute Map](https://tylerastro.github.io/Folium_Astronomy_Institutes/)**: the QS top-100 physics & astronomy institutes on one interactive world map
- 🛰️ **[Astronomy-FITS-examples](https://github.com/Tylerastro/Astronomy-FITS-examples)**: tools and demos for downloading science images from observatories

### 📄 Papers

- ✨ [Simultaneous Detection of Optical Flares of the Magnetically Active M-dwarf Wolf359](https://doi.org/10.3847/1538-3881/ac4e92), *AJ* 163, 164 (2022), my M.Sc. thesis
- 💥 [A closer look at the host-galaxy environment of high-velocity Type Ia supernovae](https://doi.org/10.1093/mnras/stae1268), *MNRAS* 531, 1988 (2024)

### 🧰 Stack

**Backend** · Python · FastAPI · Django · SQLAlchemy · Pydantic · AWS Chalice  
**Data** · PostgreSQL · MySQL · DynamoDB · Elasticsearch  
**AWS** · Lambda · API Gateway (REST & WebSockets) · Cognito · EventBridge · App Runner · Aurora · CloudWatch  
**Frontend** · TypeScript · Next.js · React · React Three Fiber · Three.js  
**Tooling** · Docker · GitHub Actions · uv · ruff · pytest · OpenAI & Anthropic APIs

### 🎧 Off the clock

- ⚾ Catcher in baseball, outfielder in softball
- 🎤 推し: 白玖ウタノ. Utano Track and her [3rd-anniversary site](https://www.utanoko.fans) are my fan projects
- 🎮 Little Busters! and 📺 Angel Beats!, so Key soundtracks on repeat. "My Soul, Your Beats!" forever

### 📫 Elsewhere

🌐 [tylerastro.dev](https://tylerastro.dev) · 💼 [LinkedIn](https://www.linkedin.com/in/tylerastro) · ✍️ [Medium](https://medium.com/@tylerastro) · ✉️ [tyler@tylerastro.dev](mailto:tyler@tylerastro.dev) · 📄 [CV](https://tylerastro.dev/cv.pdf)

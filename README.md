## Hi, I'm Tyler — Han Tang Lin

Backend engineer in Taipei. I'm the technical lead on a FastAPI + PostgreSQL document-automation platform that I architected end to end; before that I built serverless systems on AWS. Before software, I was an astrophysicist studying Type Ia supernova host environments.

I'm most useful where a live system is *quietly wrong under concurrency* — jobs that run three times, locks that aren't there, retries that multiply traffic, tokens nobody verifies.

### Production, by the numbers

- **1M+ requests / month across 195 REST endpoints** over 44 tables — architected end to end; I wrote ~90% of its 44K production lines
- **p99 39.2 s → 1.0 s** — moved a 37-second reconciliation off the request path behind a Postgres advisory lock; slow requests 880 → 19 per day
- **3× → exactly once** — traced a triple-firing scheduled job to a trigger timeout colliding with AWS async retries
- **418× retry amplification shut down** — 43K requests were fanning out into 18M Lambda invocations, half of all Lambda spend
- **Runaway job contained** — production API p99 28.2 s → 9.4 s; 5xx on the affected endpoint 87% → 0%
- **N+1 hunting** — 1,108 → 6 queries per request (12.3 s → 775 ms) and 244 → 3 (2.6 s → 210 ms) on core endpoints; primary API mean duration −48%, cold-start init −23%
- **Auth bypass closed** — replaced unverified JWT claim reads with full signature and expiry verification
- **100 PRs merged** integrating 2,392 commits from 8 engineers; introduced the team's first CI quality gate and its uv + ruff toolchain

### Stack

**Python** · FastAPI · Django · SQLAlchemy · Pydantic · AWS Chalice  
**Data** · PostgreSQL · MySQL · DynamoDB · Elasticsearch  
**AWS** · Lambda · API Gateway (REST & WebSockets) · Cognito · EventBridge · App Runner · Aurora · CloudWatch  
**Tooling** · Docker · GitHub Actions · uv · ruff · pytest · OpenAI & Anthropic APIs

### From astronomy

- **[NCU TOM](https://tom.astro.ncu.edu.tw)** — Target & Observation Management platform, still in use at Lulin Observatory ([issue tracker](https://github.com/Tylerastro/NCU_TOM-tracker)). Rebuilt its light-curve plotting on canvas after benchmarking 15 charting libraries: DOM nodes 60,082 → 104 at 20k points
- **[Astronomy-FITS-examples](https://github.com/Tylerastro/Astronomy-FITS-examples)** — tools and demos for downloading science images from observatories
- M.Sc. Astronomy (NCU) · B.Sc. Physics (NSYSU) · two first-author papers, incl. *MNRAS*

### Elsewhere

[tylerastro.dev](https://tylerastro.dev) · [LinkedIn](https://www.linkedin.com/in/tylerastro) · [Medium](https://medium.com/@tylerastro) · [tyler@tylerastro.dev](mailto:tyler@tylerastro.dev)

<sub>中文 · English · Français · 日本語</sub>

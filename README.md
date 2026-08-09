```console
$ whoami
neekunj-chaturvedi

$ cat /etc/motd
Distributed Systems Engineer. I build systems that don't fail.
I don't write code — I engineer software.

$ uptime
up 4 years, shipping since 2022 · load avg: 0.09, 0.44, 1.91
```

```
┌─ SYSTEM STATUS ─────────────────────────────────────────────┐
│                                                             │
│   BUILD      between projects — on a break   ◐ paused       │
│   FOCUS      distributed systems · scale     ● operational  │
│   CAPACITY   open to collaboration           ● accepting    │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

## `~/manifest.yaml`

```yaml
apiVersion: engineer/v1
kind: DistributedSystemsEngineer
metadata:
  name: neekunj-chaturvedi
  since: 2022
spec:
  building: null # on a break — planned maintenance window
  learning: [expo, cloud-native, design-systems, web3]
  askMeAbout: [system-design, modern-ui, blockchain, cloud, startups]
  openTo: [ambitious-products, open-source]
  replicas: 1 # not horizontally scalable, sorry
```

## `GET /metrics`

```prom
# HELP track_record Numbers that actually happened.
# TYPE track_record gauge

product_mrr_usd{state="scaled"}            1000     # $1K MRR, product I built
users_served{env="production"}            50000     # 50K on a live service
github_rank_percentile{year="2025"}          98     # top 2% on GitHub
incidents_caused_by_scale{}                   0     # the whole point
```

## Services I run

| Service         | Description                                              | SLO                       |
| :-------------- | :------------------------------------------------------- | :------------------------ |
| `build/`        | Shipping products 0 → 1, and then some                   | ships or it didn't happen |
| `distributed/`  | Services that stay correct when the network doesn't      | no split brains           |
| `architecture/` | System design that survives contact with users           | 99.9%                     |
| `infra/`        | DevOps, pipelines, containers, the boring critical stuff | 99.95%                    |
| `scale/`        | Making the graph go up without the pager going off       | p99 < 200ms               |
| `ui/`           | Pixel-perfect, accessible, actually usable interfaces    | 0 a11y regressions        |
| `automation/`   | Killing toil, raising team velocity                      | −1 manual step / week     |

## Runbook

```bash
1. read the problem twice        # most "bugs" are misread requirements
2. design for the failure case   # happy paths write themselves
3. ship small, ship often        # big bang deploys are a smell
4. measure, then optimize        # never the other way round
5. leave it simpler than found   # complexity is the real outage
```

## `tail -f /var/log/favourites`

```log
[VITE  ] local dev server running at http://localhost:5173
[SERVER] node api listening on :8000
[DOCKER] building image app-service:latest ... done
[HTTP  ] 200 OK  /api/login  124ms
[DEPLOY] rollout complete — 0 errors
```

## Telemetry

<img src="https://github-readme-streak-stats.herokuapp.com?user=neekunjchaturvedi&theme=dark&hide_border=true&background=00000000&ring=58a6ff&fire=58a6ff&currStreakLabel=8b949e" height="160" />

## Endpoints

```http
GET  /email      → neekunjchaturvedi3@gmail.com
GET  /linkedin   → /in/neekunj-chaturvedi
GET  /github     → /neekunjchaturvedi
GET  /twitter    → @neekunj_ch
```

[`mail`](mailto:neekunjchaturvedi3@gmail.com) · [`linkedin`](https://linkedin.com/in/neekunj-chaturvedi/) · [`github`](https://github.com/neekunjchaturvedi) · [`twitter`](https://x.com/neekunj_ch)

<sub><code>EOF</code> · thanks for reading the logs</sub>

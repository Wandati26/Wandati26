<div align="center">

<img src="assets/banner.svg" alt="Marvin Wandati — DevSecOps Engineer. AWS, Kubernetes, Terraform, software supply-chain security, observability." width="100%" />

<br/>

<a href="https://www.linkedin.com/in/marvin-wandati/"><img src="https://img.shields.io/badge/LinkedIn-connect-5ef2a0?style=for-the-badge&logo=linkedin&logoColor=5ef2a0&labelColor=0b131c&color=141f2b" alt="LinkedIn" /></a>
<a href="mailto:wandatimarvin23@gmail.com"><img src="https://img.shields.io/badge/Email-reach%20out-5ef2a0?style=for-the-badge&logo=gmail&logoColor=5ef2a0&labelColor=0b131c&color=141f2b" alt="Email" /></a>
<img src="https://komarev.com/ghpvc/?username=Wandati26&style=for-the-badge&label=VISITORS&color=141f2b&labelColor=0b131c" alt="Profile views" />

</div>

---

## `$ whoami`

```console
wandati@secops:~$ cat /etc/profile.d/identity.sh

  ROLE      DevSecOps Engineer — secure, observable, production-ready cloud platforms
  BASED     Milan, Italy
  EXP       2+ years across cloud platform engineering and production operations
  CONTEXT   B2B SaaS · sole DevSecOps engineer · AWS-native platform
  REGION    eu-west-1 · 3 isolated environments · fully Terraform-managed
  THESIS    Practical security — controls that reduce risk, survive audits,
            and keep delivery moving.

wandati@secops:~$ _
```

I work across **AWS**, **Kubernetes**, **Terraform**, **CI/CD**, **container hardening**, **software supply-chain security**, **observability**, and **production operations** — and I act as first responder when production pages.

---

## `$ ./report --impact --verified`

> Every number below is from work I shipped and can walk you through.

| | Before | After | What it took |
|---|---:|---:|---|
| **Container image findings** | `1,014` | **`9`** | base image rebuild, layer surgery, dependency pruning |
| **Critical CVEs** | `25` | **`0`** | continuous scanning wired into the merge gate |
| **High CVEs** | `284` | **`7`** | same pipeline, enforced on every build |
| **Production image size** | `2.5 GB+` | **`< 200 MB`** | multi-stage builds, ruthless layer elimination |
| **Long-lived AWS keys in CI** | `100%` | **`0`** | full GitHub Actions → OIDC migration |
| **Avoidable RDS storage cost** | `$1,300+/mo` | **`reclaimed`** | 13.2 TB rebuilt on gp3 under Terraform ownership |

<div align="center">

<img src="https://img.shields.io/badge/CRITICAL_CVEs-0-5ef2a0?style=for-the-badge&labelColor=0b131c&color=14301f" alt="Critical CVEs: 0" />
<img src="https://img.shields.io/badge/STATIC_CI_KEYS-0-5ef2a0?style=for-the-badge&labelColor=0b131c&color=14301f" alt="Static CI keys: 0" />
<img src="https://img.shields.io/badge/UNSIGNED_IMAGES_IN_PROD-0-5ef2a0?style=for-the-badge&labelColor=0b131c&color=14301f" alt="Unsigned images in prod: 0" />
<img src="https://img.shields.io/badge/ANNUAL_COST_RECLAIMED-%2415.6K%2B-f5b942?style=for-the-badge&labelColor=0b131c&color=2b2312" alt="Annual cost reclaimed: $15.6K+" />

</div>

---

## `$ systemctl status secure-delivery`

I built the DevSecOps foundation from zero: a **six-gate GitHub Actions pipeline** that caught **4 HIGH-severity CVEs before the first production deployment**. Unsigned images cannot reach production — Cosign verification is mandatory, not advisory.

<div align="center">
<img src="assets/pipeline.svg" alt="Secure delivery pipeline: commit flows through SAST, secret scanning, dependency review, image scanning, SBOM generation and Cosign signing before deploy. Unsigned images are blocked at admission." width="100%" />
</div>

Promotion through **dev → staging → prod** runs on tag-based gates with required approvals, so every production release is **reviewed, signed, and traceable**.

---

## `$ radar --scan --year 2026`

<table>
<tr>
<td width="48%" valign="top">
<img src="assets/threat-radar.svg" alt="Focus radar showing four tracked domains: AI and agentic security, software supply chain, policy-as-code, and platform engineering with FinOps." width="100%" />
</td>
<td width="52%" valign="top">

### `[01]` AI & Agentic Security
The attack surface moved. Agents that hold credentials, call tools, and act autonomously need the same rigour we spent a decade building for CI/CD — **identity, least privilege, audit trail, and a kill switch**. OWASP LLM Top 10 as a baseline, MCP server hardening, prompt-injection boundaries, and AI-BOM alongside SBOM.

### `[02]` Software Supply Chain
**Provenance beats trust.** SBOM on every build, Cosign signatures enforced at admission, and dependency review that blocks rather than warns. If you can't prove where an artifact came from, it doesn't ship.

### `[03]` Policy-as-Code & Shift-Left
Security that lives in a PDF is decoration. Controls belong **in the pipeline as code** — scanning gates, admission control, and CIS benchmark checks that fail the build instead of filing a ticket.

### `[04]` Platform Engineering + FinOps
Golden paths so the secure route is the *easy* route. And **cost as a guardrail**, not a quarterly surprise — the same instinct that found $15.6K/year sitting in over-provisioned storage.

</td>
</tr>
</table>

---

## `$ ls -la ~/toolchain`

<table>
<tr>
<td width="52%" valign="top">

**Cloud & Infrastructure**

![AWS](https://img.shields.io/badge/AWS-5ef2a0?style=for-the-badge&logo=amazonwebservices&logoColor=5ef2a0&labelColor=0b131c&color=141f2b)
![Terraform](https://img.shields.io/badge/Terraform-5ef2a0?style=for-the-badge&logo=terraform&logoColor=5ef2a0&labelColor=0b131c&color=141f2b)
![Kubernetes](https://img.shields.io/badge/Kubernetes-5ef2a0?style=for-the-badge&logo=kubernetes&logoColor=5ef2a0&labelColor=0b131c&color=141f2b)
![Docker](https://img.shields.io/badge/Docker-5ef2a0?style=for-the-badge&logo=docker&logoColor=5ef2a0&labelColor=0b131c&color=141f2b)
![Ansible](https://img.shields.io/badge/Ansible-5ef2a0?style=for-the-badge&logo=ansible&logoColor=5ef2a0&labelColor=0b131c&color=141f2b)
![Helm](https://img.shields.io/badge/Longhorn-5ef2a0?style=for-the-badge&logo=rancher&logoColor=5ef2a0&labelColor=0b131c&color=141f2b)

**Security & Supply Chain**

![Cosign](https://img.shields.io/badge/Cosign-5ef2a0?style=for-the-badge&logo=sigstore&logoColor=5ef2a0&labelColor=0b131c&color=141f2b)
![SBOM](https://img.shields.io/badge/SBOM-5ef2a0?style=for-the-badge&logo=linuxfoundation&logoColor=5ef2a0&labelColor=0b131c&color=141f2b)
![OIDC](https://img.shields.io/badge/OIDC-5ef2a0?style=for-the-badge&logo=openid&logoColor=5ef2a0&labelColor=0b131c&color=141f2b)
![SAST](https://img.shields.io/badge/SAST%20%2F%20SCA-5ef2a0?style=for-the-badge&logo=snyk&logoColor=5ef2a0&labelColor=0b131c&color=141f2b)
![KMS](https://img.shields.io/badge/AWS%20KMS-5ef2a0?style=for-the-badge&logo=amazonaws&logoColor=5ef2a0&labelColor=0b131c&color=141f2b)
![WAF](https://img.shields.io/badge/AWS%20WAF-5ef2a0?style=for-the-badge&logo=amazonaws&logoColor=5ef2a0&labelColor=0b131c&color=141f2b)

</td>
<td width="48%" valign="top">
<img src="assets/stack-orbit.svg" alt="Toolchain orbiting a hardened, signed core." width="100%" />
</td>
</tr>
</table>

**CI/CD & Automation**

![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-5ef2a0?style=for-the-badge&logo=githubactions&logoColor=5ef2a0&labelColor=0b131c&color=141f2b)
![Python](https://img.shields.io/badge/Python-5ef2a0?style=for-the-badge&logo=python&logoColor=5ef2a0&labelColor=0b131c&color=141f2b)
![Bash](https://img.shields.io/badge/Bash-5ef2a0?style=for-the-badge&logo=gnubash&logoColor=5ef2a0&labelColor=0b131c&color=141f2b)
![Playwright](https://img.shields.io/badge/Playwright-5ef2a0?style=for-the-badge&logo=playwright&logoColor=5ef2a0&labelColor=0b131c&color=141f2b)

**Observability & Data**

![Grafana](https://img.shields.io/badge/Grafana%20Cloud-5ef2a0?style=for-the-badge&logo=grafana&logoColor=5ef2a0&labelColor=0b131c&color=141f2b)
![OpenSearch](https://img.shields.io/badge/OpenSearch-5ef2a0?style=for-the-badge&logo=opensearch&logoColor=5ef2a0&labelColor=0b131c&color=141f2b)
![CloudWatch](https://img.shields.io/badge/CloudWatch%20%2B%20X--Ray-5ef2a0?style=for-the-badge&logo=amazoncloudwatch&logoColor=5ef2a0&labelColor=0b131c&color=141f2b)
![Elastic](https://img.shields.io/badge/ELK%20Stack-5ef2a0?style=for-the-badge&logo=elasticstack&logoColor=5ef2a0&labelColor=0b131c&color=141f2b)
![Athena](https://img.shields.io/badge/Athena-5ef2a0?style=for-the-badge&logo=amazonaws&logoColor=5ef2a0&labelColor=0b131c&color=141f2b)
![PostgreSQL](https://img.shields.io/badge/RDS%20PostgreSQL-5ef2a0?style=for-the-badge&logo=postgresql&logoColor=5ef2a0&labelColor=0b131c&color=141f2b)

---

## `$ ls ~/.credentials`

<div align="center">

<img src="https://img.shields.io/badge/Docker%20%2B%20Kubernetes-Udemy-5ef2a0?style=for-the-badge&logo=docker&logoColor=5ef2a0&labelColor=0b131c&color=141f2b" alt="Docker and Kubernetes — Udemy" />
<img src="https://img.shields.io/badge/Certified%20DevOps%20Practitioner-TechWorld%20with%20Nana-5ef2a0?style=for-the-badge&logo=kubernetes&logoColor=5ef2a0&labelColor=0b131c&color=141f2b" alt="Certified DevOps Practitioner — TechWorld with Nana" />
<img src="https://img.shields.io/badge/Postman%20API%20Fundamentals%20Expert-Canvas-5ef2a0?style=for-the-badge&logo=postman&logoColor=5ef2a0&labelColor=0b131c&color=141f2b" alt="Postman API Fundamentals Expert — Canvas" />

<br/>

<img src="https://img.shields.io/badge/AWS%20Educate-8%20completed-38d9e0?style=for-the-badge&logo=amazonwebservices&logoColor=38d9e0&labelColor=0b131c&color=12212b" alt="AWS Educate — 8 completed" />
<img src="https://img.shields.io/badge/KodeKloud-6%20completed-38d9e0?style=for-the-badge&logo=kubernetes&logoColor=38d9e0&labelColor=0b131c&color=12212b" alt="KodeKloud — 6 completed" />

</div>

---

## `$ journalctl --unit platform --since "2025-02"`

<details open>
<summary><b>◢ DevSecOps Engineer · Expandi Group</b> · <code>Feb 2026 — Present</code> — <i>B2B SaaS · sole DevSecOps engineer · AWS-native</i></summary>

<br/>

- **Built the DevSecOps foundation from zero** — a 6-gate GitHub Actions pipeline (SAST, secret scanning, dependency review, image scanning, SBOM, artifact signing) that caught **4 HIGH-severity CVEs before the first production deployment**.
- **Eliminated 100% of long-lived AWS keys from CI/CD** by migrating GitHub Actions to OIDC, and enforced Cosign verification so unsigned images cannot reach production.
- **Led container hardening for a core service** — findings `1,014 → 9`, Critical `25 → 0`, High `284 → 7`, image size `2.5 GB+ → < 200 MB`.
- **Deployed and operate 3 isolated AWS environments** in `eu-west-1` with modular Terraform (App Runner, API Gateway, S3, CloudFront, ECR, RDS, Route 53) — including a **zero-downtime DNS migration** from GoDaddy to Route 53.
- **Own the dev → staging → prod release lifecycle** — promotion through GitHub Actions with tag-based gates and required approvals; every production release is reviewed, signed, and traceable.
- **Established the first production observability baseline** (OpenObserve, Grafana Cloud, CloudWatch, X-Ray, Micrometer, structured JSON logs, WAF telemetry) with alarms on p95/p99 latency, JVM, database and queue health — and act as **first responder for production incidents**.
- **Provisioned a private Terraform-managed OpenSearch platform** for **3.22M company documents (78.3M Lucene docs)** with KMS encryption, VPC-only access, and least-privilege IAM separation.
- **Reclaimed $1,300+/month ($15.6K+/year)** in avoidable RDS storage cost by recreating a 13.2 TB database on gp3 under Terraform ownership, restoring auditable IaC control.
- **Made a previously unqueryable S3 document archive product-ready** — validated and curated **40 GB+** with Athena, then migrated it into RDS.

</details>

<details>
<summary><b>◢ DevOps Engineer · Ryanada Limited</b> · <code>Feb 2025 — Aug 2025</code> — <i>Cloud hosting platform · domains & VPS · Kubernetes operations</i></summary>

<br/>

- **Standardized configuration across 100+ hosting servers** with reusable Ansible playbooks, replacing hours-long manual setup with repeatable provisioning and cutting configuration drift.
- **Replaced customer-reported failures with synthetic detection** — Playwright monitors for customer-facing services, routed through Elasticsearch and ElastAlert to Slack, so operations could intervene *before* incidents became support calls.
- **Operated containerized services across two Kubernetes clusters**, improving stateful workload resilience with Longhorn persistent storage, automated snapshots, and node-failure recovery workflows.
- **Strengthened recovery across both clusters** with Kasten K10 backups to MinIO S3, with schedules and retention aligned to workload criticality.
- **Centralized high-volume platform logs** in the ELK stack, automating alerts for CPU saturation and application latency to accelerate investigation.

</details>

---

## `$ git log --graph --author=Wandati26`

> Most of what I build lives in private company repositories, so this graph
> undercounts by a wide margin. The numbers worth judging me on are in the
> impact table above — and I'm happy to walk through any of them.

<div align="center">
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Wandati26/Wandati26/output/github-snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Wandati26/Wandati26/output/github-snake.svg" />
  <img src="https://raw.githubusercontent.com/Wandati26/Wandati26/output/github-snake-dark.svg" alt="Snake eating my contribution graph" />
</picture>
</div>

---

## `$ cat ~/.philosophy`

```console
wandati@secops:~$ cat ~/.philosophy

  01  Security that blocks the build beats security that files a ticket.
  02  If you can't prove where an artifact came from, it doesn't ship.
  03  Observability is not dashboards. It's knowing before the customer does.
  04  Cost is a guardrail, not a quarterly surprise.
  05  The secure path has to be the easy path, or nobody takes it.

wandati@secops:~$ _
```

---

<div align="center">

### `$ ./connect`

<a href="https://www.linkedin.com/in/marvin-wandati/"><img src="https://img.shields.io/badge/LinkedIn-5ef2a0?style=for-the-badge&logo=linkedin&logoColor=5ef2a0&labelColor=0b131c&color=141f2b" alt="LinkedIn" /></a>
<a href="mailto:wandatimarvin23@gmail.com"><img src="https://img.shields.io/badge/Gmail-5ef2a0?style=for-the-badge&logo=gmail&logoColor=5ef2a0&labelColor=0b131c&color=141f2b" alt="Email" /></a>
<a href="https://github.com/Wandati26"><img src="https://img.shields.io/badge/GitHub-5ef2a0?style=for-the-badge&logo=github&logoColor=5ef2a0&labelColor=0b131c&color=141f2b" alt="GitHub" /></a>

<br/><br/>

<sub><code>signed · scanned · attested — every artifact, every release</code></sub>

</div>

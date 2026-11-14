# Awesome-QA-Testing-Test-Case-Management

# Awesome QA Testing & Test Case Management

> A curated list of top QA Testing and Test Case Management platforms — both SaaS/Hosted commercial solutions and open-source alternatives for organizing test cases, planning runs, and tracking execution results.
> 🌟 Star this repo if you find it useful! 🌟

---

## 📋 Table of Contents

- [SaaS / Hosted Platforms](#-saas--hosted-platforms)
  - [TestRail](#testrail)
  - [Zephyr Enterprise](#zephyr-enterprise)
  - [Xray](#xray)
  - [Qase](#qase)
  - [BrowserStack Test Management](#browserstack-test-management)
- [Open-Source Software](#-open-source-software)
  - [Kiwi TCMS](#kiwi-tcms)
  - [TestLink](#testlink)
  - [TestPlanIt](#testplanit)
  - [QA Studio](#qa-studio)
  - [Squash TM](#squash-tm)
  - [Suitest](#suitest)
  - [FitNesse](#fitnesse)
  - [Tuleap](#tuleap)
- [Comparison at a Glance](#-comparison-at-a-glance)
- [Contributing](#-contributing)

---

## 🟦 SaaS / Hosted Platforms

Commercial, cloud-hosted QA Testing and Test Case Management platforms. These are not open-source but are included as reference points for feature comparison.

| Platform | Company & Scale (Valuation / Revenue) | Deployment / Integration | Starting Price | Free Tier / Trial Limits | Key Features |
|---|---|---|---|---|---|
| **BrowserStack Test Management** | **BrowserStack** (~$4.0B valuation, ~$250M+ ARR) | Cloud (BrowserStack Ecosystem) | $29.80 / user / month ($149 / month for 5-user team pack) | Permanent Free tier: Up to 5 users, unlimited test cases, unlimited test runs, 10GB storage, 30-day run history | AI-assisted test authoring, rich media attachments, device cloud execution integration |
| **TestRail** | **Idera, Inc.** (~$3.0B valuation, ~$300M+ revenue) | Cloud / Server (Standalone) | $38 / user / month (Professional) or $25 / user / month (Essentials, up to 5 users) | 30-day free trial (Full features, no credit card required; no permanent free plan) | Structured test case repository, milestone runs, custom fields, audit logs, REST API |
| **Xray** | **Idera, Inc. / Xblend** (~$3.0B parent valuation, ~$300M+ corporate revenue) | Jira-native (Cloud / Data Center) | $10 / month flat base (Standard edition for 1–10 Jira users) | 30-day free trial on Atlassian Marketplace (All Jira users licensed; no permanent free plan) | Requirement-to-defect traceability, BDD/Gherkin support, CI/CD REST API, coverage reports |
| **Zephyr (Enterprise & Scale)** | **SmartBear Software** (~$1.8B–$2.0B valuation, ~$150M+ ARR) | Jira-native (Scale/Squad) & Standalone Cloud (Enterprise) | $10 / month flat base (Zephyr Scale for 1–10 Jira users) | 30-day free trial on Atlassian Marketplace (Matches host Jira user count; no permanent free plan) | Deep Jira ecosystem integration, traceability matrix, automated test execution results |
| **Qase** | **Qase Inc.** (~$42M valuation, ~$4.7M ARR) | Cloud (Standalone & Integrations) | $35 / user / month (Teams plan, min 5 seats; billed annually) | Permanent Free tier: Up to 4 users, 2 projects, 2 concurrent runs, 500MB storage, 30-day run history (also 14-day Teams trial) | Modern developer-first UI, automated test result ingestion, defect tracking, Jira/GitLab integration |

---

## 🟩 Open-Source Software

Self-hosted, community-driven QA Testing and Test Case Management tools. The open-source ecosystem spans **mature standards-compliant platforms**, **modern self-hostable alternatives**, and **specialized frameworks**.

### Kiwi TCMS
**Stack:** Python / Django / PostgreSQL | **License:** GPL-2.0+  
Kiwi TCMS is the most widely recognized open-source test management system, described as IEEE 829 compatible, free, and open source with a strong community behind the project [citation:3]. It provides test plan and test case creation, progress tracking across multiple teams, and instant insight into testing status for release planning. Plugins for popular testing frameworks collect automation results, and 1-click bug reporting integrates with third-party bug trackers. **Best for:** Teams wanting a proven, actively maintained open-source TCMS with a clean interface and no unnecessary complexity.

### TestLink
**Stack:** PHP / MySQL | **License:** GPL-2.0  
TestLink is a long-standing web-based test management system with requirements tracking and integration with bug trackers including Bugzilla, Jira, and Mantis [citation:4]. Features include hierarchical test case organization with traceable history, keyword support, test prioritization, milestone definitions, reporting and metrics, and export to HTML/Word/Excel. **Trade-off:** Interface and workflow feel dated, and automation integration is DIY [citation:7]. It is widely used in projects with 20+ engineers and 1,000+ test cases. **Best for:** Budget-constrained teams with internal maintenance capability and relatively basic requirements for test case and execution tracking.

### TestPlanIt
**Stack:** TypeScript / PostgreSQL / Docker | **License:** Open Source  
TestPlanIt was released as open source after two years of development, positioned as a modern alternative to expensive proprietary test management tools [citation:1]. It supports self-hosting with full data control, customization for team-specific workflows, and code auditing for security and compliance. Deployment involves cloning the repository and running `pnpm install`, with Docker deployment options available. **Best for:** Teams wanting a modern open-source option with active development and self-hosted deployment, accepting a younger ecosystem than Kiwi TCMS or TestLink.

### QA Studio
**Stack:** SvelteKit / PostgreSQL / Prisma | **License:** AGPL-3.0  
QA Studio is a modern, open-source test management platform built by QA engineers, for QA engineers, with a focus on speed and no bloat [citation:6]. Key features include hierarchical test suites and cases with full traceability, test execution across multiple environments, rich media attachments (screenshots, videos, logs, stack traces), an API-first design, and self-hosted authentication. It supports deployment on Vercel, Docker, or any Node.js host. **Important:** It requires a Vercel Blob storage token for attachments even in development. **Best for:** Teams wanting a modern, fast self-hosted test management platform with API-first design and rich media support.

### Squash TM
**Stack:** Java / PostgreSQL/MySQL | **License:** LGPL-3.0 (open core)  
Squash TM is an open-core test management platform with a strong requirements-to-test model and Jira synchronization options [citation:7]. The core is LGPL-3.0, with Premium and Ultimate licenses adding functionality. It is best suited for teams that manage requirements and tests together and use Jira, with plugins for reporting, automation (Squash AUTOM), and a REST API. **Trade-off:** Some Jira and requirements plugins sit behind Premium or Ultimate licenses, and the platform has more concepts and configuration than simpler tools [citation:7]. **Best for:** Agile teams using Jira that must demonstrate requirement coverage and are prepared to buy a license if the free tier proves limiting.

### Suitest
**Stack:** Vite / React 19 / MCP-native | **License:** Apache-2.0  
Suitest is a self-hostable, MCP-native testing platform with manual test management, deterministic runs, and optional AI [citation:15]. It is explicitly positioned as free and open-source with no subscription fees, supporting self-hosting without limits. Key features include manual test case management via a web dashboard, execution across browsers (Playwright), APIs, databases, mobile (Appium), desktop, and Kubernetes. **Important:** While manual TCM does not require AI, MCP execution and AI features require a validated workspace LLM. **Best for:** Teams wanting a modern, MCP-native test platform with optional AI assistance and broad execution target support, accepting the LLM dependency for advanced features.

### FitNesse
**Stack:** Java | **License:** Open Source  
FitNesse is a fully integrated standalone wiki and acceptance testing framework [citation:5][citation:9]. It functions as a collaboration tool (wiki web server with low entry and learning curve), a test tool (wiki pages run as tests against the application), and an open-source project not owned by any company [citation:14]. It enables customers, testers, and programmers to collaboratively define acceptance tests and compare expectations to actual results. **Trade-off:** It is a wiki-based acceptance testing framework rather than a traditional test case management platform with test plans, runs, and reporting. **Best for:** Teams wanting collaborative acceptance testing with business stakeholders in a wiki format, rather than structured test case repository management.

### Tuleap
**Stack:** PHP / MySQL | **License:** GPL (Community) / Commercial (Enterprise)  
Tuleap is an open-source application lifecycle management (ALM) platform that includes test management, requirements, agile planning, and trackers [citation:7]. It suits regulated or large organizations wanting traceability in one self-hosted system. **Important caveat:** Tuleap's documentation lists "Test Management: test campaigns and traceability" among plugins distributed only to Tuleap Enterprise subscribers—confirm that you can obtain the test-management module under your intended edition before committing [citation:7]. **Best for:** Compliance-focused organizations needing requirements, tests, and defects traced in one platform, accepting the Enterprise dependency for the test management module.

---

## 📊 Comparison at a Glance

| Software | License | Stack | Requirements Traceability | Automation Integration | Self-Hosted | Best For |
|----------|---------|-------|---------------------------|------------------------|-------------|----------|
| **TestRail** | Proprietary | Cloud | (Plugin) | CLI/API | ❌ | Dedicated standalone test management |
| **Zephyr** | Proprietary | Jira plugin | ✅ | ✅ | ❌ | Jira-centric large-scale libraries |
| **Xray** | Proprietary | Jira plugin | ✅ Strong | ✅ | ❌ | Requirements traceability in Jira |
| **Qase** | Proprietary | Cloud | ✅ | ✅ API | ❌ | Modern automation-first test management |
| **BrowserStack** | Proprietary | Cloud | (2-way binding) | ✅ | ❌ | BrowserStack device cloud users |
| **Kiwi TCMS** | GPL-2.0+ | Python/Django | (IEEE 829) | ✅ Plugins | ✅ | Proven OSS test management |
| **TestLink** | GPL-2.0 | PHP/MySQL | ✅ Strong | DIY | ✅ | Budget OSS with basic needs |
| **TestPlanIt** | Open Source | TypeScript/Docker | (Check) | (Check) | ✅ | Modern OSS alternative |
| **QA Studio** | AGPL-3.0 | SvelteKit/Postgres | ✅ Hierarchical | (API-first) | ✅ | Fast modern self-hosted TCMS |
| **Squash TM** | LGPL (core) | Java | ✅ Strong | ✅ (Squash AUTOM) | ✅ | Requirements + Jira coverage |
| **Suitest** | Apache-2.0 | Vite/React | (MCP-native) | ✅ Multi-target | ✅ | MCP-native + optional AI |
| **FitNesse** | Open Source | Java | (Wiki-based) | ✅ Acceptance | ✅ | Collaborative acceptance testing |
| **Tuleap** | GPL/Commercial | PHP/MySQL | ✅ Strong | (Check) | ✅ | ALM + traceability (Enterprise test module) |

---

## 🤝 Contributing

Contributions are welcome! If you know of an open-source QA Testing or Test Case Management tool that should be listed here, please open a pull request with:

- Project name and URL
- Brief description (1–2 sentences)
- Stack and license
- Why it stands out

Please ensure the project is actively maintained (releases within the last 12 months) and genuinely open-source. Note that the open-source ecosystem offers strong options: **Kiwi TCMS** is the most mature and widely adopted open-source TCMS with IEEE 829 compatibility [citation:3], **TestLink** remains viable for budget-constrained teams with internal maintenance capability [citation:4][citation:11], **TestPlanIt** and **QA Studio** represent newer modern alternatives with active development [citation:1][citation:6], and **Squash TM** provides the strongest requirements-to-test traceability with Jira integration in its open-core edition [citation:7]. **Suitest** is notable for its MCP-native architecture with optional AI and broad execution target support [citation:15].

---

## 📄 License

This list is released under CC0 1.0 Universal (Public Domain). The software projects listed retain their respective licenses.

---

⭐ **If this list helped you discover a useful tool, please star the repo!** ⭐

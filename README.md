<h1 align="center">Caleb Love</h1>

<p align="center">
  <strong>Building infrastructure for autonomous AI agents</strong><br>
  Solutions Engineer · Sydney, Australia
</p>

<p align="center">
  <a href="https://caleb-love.com">caleb-love.com</a> ·
  <a href="https://linkedin.com/in/caleb-love">LinkedIn</a> ·
  <a href="mailto:hello@caleb-love.com">hello@caleb-love.com</a>
</p>

---

I work on the systems that make AI agents reliable in production — tracing, evaluation, cost controls, regression detection. Not the demo, the infrastructure underneath it.

By day I'm a Solutions Engineer at [Pendo](https://pendo.io), running technical evaluations and building proof-of-concepts for enterprise teams. By night I'm deep in agentic AI, building the tooling that turns autonomous agents from impressive demos into things you can actually trust.

<br>

## Foxhound

> **Compliance-grade observability for AI agent fleets.**
>
> Trace every decision. Evaluate every response. Budget every dollar.

<p>
  <a href="https://github.com/caleb-love/foxhound"><img src="https://img.shields.io/badge/GitHub-foxhound-181717?style=flat&logo=github" alt="GitHub"></a>
  <a href="https://github.com/caleb-love/foxhound/blob/main/LICENSE"><img src="https://img.shields.io/github/license/caleb-love/foxhound?style=flat" alt="MIT License"></a>
  <a href="https://foxhound.caleb-love.com"><img src="https://img.shields.io/badge/docs-foxhound.caleb--love.com-blue?style=flat" alt="Docs"></a>
</p>

[Foxhound](https://github.com/caleb-love/foxhound) is an open-source observability platform I built for teams running AI agents in production. Generic APM tools treat agent workflows as black boxes — Foxhound traces the full decision tree so you can see exactly what happened, why, and where it broke.

**What it does:**

- **Tracing** — Structured span trees for every agent run, session replay to reconstruct state at any point, run diffs to compare executions side-by-side
- **Evaluation** — LLM-as-judge evaluators, dataset curation from production traces, experiment runner with A/B comparison
- **Cost & SLA** — Per-agent budgets with SDK callbacks, SLA monitoring, automated alerting across Slack, PagerDuty, Linear, and webhooks
- **Regression Detection** — Behavioral baselines per agent version, automated drift detection across deployments
- **Prompt Management** — Versioned templates with label-based promotion from staging to production
- **Quality Gate** — GitHub Actions integration that blocks PRs failing eval thresholds

**Architecture:**

```
11-package TypeScript monorepo · Fastify API (~80 endpoints) · PostgreSQL + Redis
7 background job queues · Python & TypeScript SDKs · 37 MCP debugging tools
```

**Auto-instrumentation for:** LangGraph · CrewAI · Pydantic AI · OpenAI Agents · Claude Agent SDK · Google ADK · AWS Bedrock AgentCore · Mastra · OpenTelemetry

<br>

## Other work

- **[Dex](https://github.com/davekilleen/dex)** — Open-source personal knowledge system built on Claude. Active contributor, daily user, testbed for agentic patterns.
- **[OpenClaw](https://github.com/OpenClaw)** — Exploring how different agent frameworks handle orchestration, tool use, and long-running autonomous tasks.
- **MCP servers & integrations** — Connecting AI agents to the tools people actually use: Slack, calendars, CRMs, project management. Making agents do more than generate text.

<br>

## Lessons from the field

| | |
|:--|:--|
| **Clarity > cleverness** | Agents don't read between the lines. Vague specs produce vague output. |
| **Fluent ≠ correct** | AI fails confidently. The skill is catching what looks right but isn't. |
| **Orchestration is design** | Multi-agent systems only work with right-sized tasks and clean handoffs. |
| **Know the failure modes** | Context degradation, spec drift, silent failures. You learn fast once burned. |
| **Context is the unlock** | Right information, right agent, right time. That's what separates demos from systems. |
| **Not everything needs an agent** | Sometimes a script is the right call. Half the job is knowing the economics. |

<br>

## Stack

<table>
  <tr>
    <td><strong>Languages</strong></td>
    <td>
      <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white" alt="TypeScript">
      <img src="https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white" alt="Python">
      <img src="https://img.shields.io/badge/SQL-4479A1?style=flat&logo=postgresql&logoColor=white" alt="SQL">
    </td>
  </tr>
  <tr>
    <td><strong>Backend</strong></td>
    <td>
      <img src="https://img.shields.io/badge/Node.js-339933?style=flat&logo=nodedotjs&logoColor=white" alt="Node.js">
      <img src="https://img.shields.io/badge/Fastify-000000?style=flat&logo=fastify&logoColor=white" alt="Fastify">
      <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white" alt="PostgreSQL">
      <img src="https://img.shields.io/badge/Redis-DC382D?style=flat&logo=redis&logoColor=white" alt="Redis">
      <img src="https://img.shields.io/badge/Drizzle-C5F74F?style=flat&logo=drizzle&logoColor=black" alt="Drizzle">
    </td>
  </tr>
  <tr>
    <td><strong>Frontend</strong></td>
    <td>
      <img src="https://img.shields.io/badge/Next.js-000000?style=flat&logo=nextdotjs&logoColor=white" alt="Next.js">
      <img src="https://img.shields.io/badge/React-61DAFB?style=flat&logo=react&logoColor=black" alt="React">
      <img src="https://img.shields.io/badge/Tailwind-06B6D4?style=flat&logo=tailwindcss&logoColor=white" alt="Tailwind">
    </td>
  </tr>
  <tr>
    <td><strong>Infra</strong></td>
    <td>
      <img src="https://img.shields.io/badge/Fly.io-7B36ED?style=flat&logo=flydotio&logoColor=white" alt="Fly.io">
      <img src="https://img.shields.io/badge/Cloudflare-F38020?style=flat&logo=cloudflare&logoColor=white" alt="Cloudflare">
      <img src="https://img.shields.io/badge/Turborepo-EF4444?style=flat&logo=turborepo&logoColor=white" alt="Turborepo">
      <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat&logo=githubactions&logoColor=white" alt="GitHub Actions">
    </td>
  </tr>
  <tr>
    <td><strong>AI</strong></td>
    <td>
      <img src="https://img.shields.io/badge/Claude-D97706?style=flat&logo=anthropic&logoColor=white" alt="Claude">
      <img src="https://img.shields.io/badge/OpenAI-412991?style=flat&logo=openai&logoColor=white" alt="OpenAI">
      <img src="https://img.shields.io/badge/LangGraph-1C3C3C?style=flat&logo=langchain&logoColor=white" alt="LangGraph">
      <img src="https://img.shields.io/badge/MCP-000000?style=flat" alt="MCP">
    </td>
  </tr>
</table>

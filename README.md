# Hi, I'm Shay

📍 **Seattle** | Backend engineer at AWS. Building agent systems that can be measured, not just demoed.

![Java](https://img.shields.io/badge/-Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/-Spring%20Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white)
![AWS](https://img.shields.io/badge/-AWS-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white)
![Kafka](https://img.shields.io/badge/-Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white)
![Redis](https://img.shields.io/badge/-Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/-PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/-Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Linux](https://img.shields.io/badge/-Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![MCP](https://img.shields.io/badge/-MCP-000000?style=flat-square&logo=anthropic&logoColor=white)
![Claude](https://img.shields.io/badge/-Claude-000000?style=flat-square&logo=anthropic&logoColor=white)
![Astro](https://img.shields.io/badge/-Astro-BC52EE?style=flat-square&logo=astro&logoColor=white)

## What I'm working on

The interesting part of an agent is rarely the prompt. It's everything around it:
which tool to call and in what order, what to do when two sources disagree, and
how you would know if the answer were wrong. Most of what I build starts from
the eval and works backwards.

- **Cost-ordered tool chains** — cheap checks first, expensive ones only when they could still change the answer
- **Constraint extraction** from natural language, separating the hard requirements from the soft preferences, because only one of those is allowed to be violated
- **Evals with deterministic ground truth**, so correctness is measured rather than eyeballed. A demo that looks right and a system that is right are different artifacts
- **MCP servers on the JVM**, which barely exist yet — most of the agent ecosystem quietly assumes Python
- **Distributed systems at AWS**, on EC2 Outposts: APIs and services running at the edge, where the network back to the region is not a given

## Projects

- 🥾 **[pnw-trail-finder](https://github.com/shayesta19/pnw-trail-finder)** — Ask a language model whether a trail is melted out this weekend and it answers from the season rather than the year. This one checks. It pulls the hard and soft constraints out of the query, runs a cost-ordered tool chain over SNOTEL snow depth, NWS forecasts, USFS road status and NPS closures, and returns ranked trails together with the values it actually looked at. Spring Boot, JDK 21.

- 🗺️ **[seattlerec](https://github.com/shayesta19/seattlerec)** — A local's guide to Seattle, built on top of my own Google Maps history. Google publishes no API for saved lists, so an importer reads a Takeout export, lifts coordinates straight out of the saved-place URLs, geocodes the stragglers, and filters out everything personal before any of it ships. Every list opens onto a map, with search across all of them at once. Live at **[seattlerec.com](https://seattlerec.com)**.

- 🚗 **[AVSimulation--OOD](https://github.com/shayesta19/AVSimulation--OOD)** — An autonomous-vehicle simulator built around pluggable driving rules: one rule interface over a shared road, lane and vehicle model, with concrete strategies for holding a lane and for passing on the left or on either side. A Swing front end runs the scenarios live, so a rule is something you watch play out rather than read the output of.

- 🧬 **[PSAproject](https://github.com/shayesta19/PSAproject)** — Recovers a decryption key by evolving toward it instead of searching for it. Chromosomes encode candidate keys, fitness scores each on how much like real language the output reads, and successive generations converge on plaintext.

## Currently building

- **trails-mcp** — the snow, weather, road and closure tools from `pnw-trail-finder`, split out as a standalone Java MCP server
- A set of agent projects that each ship with the eval that proves them: deadline and jurisdiction routing, salary benchmarking against LCA and BLS filings, itinerary feasibility checking

## Contribution snake

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/shayesta19/shayesta19/output/github-snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/shayesta19/shayesta19/output/github-snake.svg" />
  <img alt="github-snake" src="https://raw.githubusercontent.com/shayesta19/shayesta19/output/github-snake-dark.svg" />
</picture>

## Connect

[![GitHub](https://img.shields.io/badge/-Follow-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/shayesta19)
[![LinkedIn](https://img.shields.io/badge/-shayestaparveenr-0077B5?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/shayestaparveenr/)

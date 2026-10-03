<h1 align="center">sera0x</h1>

```ini
# ~/.config/sera0x/profile.conf
# last modified: 2026-10-03

[identity]
handle  = sera0x
focus   = tools for the boring parts of running side projects
started = 2026, still here

[now]
building  = dkit
            # self-hosted secrets, cron, monitors, log drain
url       = https://dkit.name.ng
stack     = node, postgres, redis, react
infra     = one VPS, pm2, cloudflare tunnel
sidequest = whatsapp bot that runs my own automations
```

<p align="center">
  <img alt="Node" src="https://img.shields.io/badge/node-18%2B-339933?logo=node.js&logoColor=white">
  <img alt="Express" src="https://img.shields.io/badge/express-4-000000?logo=express&logoColor=white">
  <img alt="React" src="https://img.shields.io/badge/react-18-149ECA?logo=react&logoColor=white">
  <img alt="Postgres" src="https://img.shields.io/badge/postgres-14%2B-4169E1?logo=postgresql&logoColor=white">
  <img alt="Redis" src="https://img.shields.io/badge/redis-6%2B-DC382D?logo=redis&logoColor=white">
</p>

## Building

[D-Kit](https://github.com/sera0x/D-Kit) is a self-hosted secrets manager with scheduled jobs, uptime monitors and a log drain. One CLI, one dashboard, one API, all talking to the same backend. You can run it on your own VPS with a start script and three env vars, or use the hosted instance at [dkit.name.ng](https://dkit.name.ng), free while it's in beta.

The parts I care most about are the unglamorous ones: keys hashed at rest and shown exactly once, cron written as `daily 09:30` instead of `30 9 * * *`, and deletes that make you type the project name first.

## Why not Go or Rust

The obvious question about a secrets manager in Node. Answer: D-Kit is one language top to bottom. The CLI ships through npm, the API is Express, the dashboard is React, and one toolchain covers all three. Go would buy a smaller memory footprint on a VPS that idles most of the day anyway. If a piece ever outgrows Node, I'll rewrite that piece, not the product.

## Stats

<table>
  <tr>
    <td>
      <img alt="sera0x's GitHub stats" src="https://github-readme-stats.vercel.app/api?username=sera0x&show_icons=true&hide_border=true&theme=github_dark" />
    </td>
    <td>
      <img alt="Top languages" src="https://github-readme-stats.vercel.app/api/top-langs/?username=sera0x&layout=compact&hide_border=true&theme=github_dark&langs_count=6" />
    </td>
  </tr>
</table>

## The graph

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/sera0x/sera0x/snake/github-contribution-grid-snake-dark.svg" />
  <img alt="contribution snake" src="https://raw.githubusercontent.com/sera0x/sera0x/snake/github-contribution-grid-snake.svg" />
</picture>

## Elsewhere

- [dkit.name.ng](https://dkit.name.ng) — the hosted instance
- [dkit.name.ng/docs](https://dkit.name.ng/docs) — full CLI and API reference
- [dkit.name.ng/tools](https://dkit.name.ng/tools) — browser dev tools, nothing leaves the page

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&height=190&section=header&color=0:0C1210,50:1A2A24,100:0C1210&text=Diego%20Bravo%20Opazo&fontSize=42&fontColor=E7E2D4&fontAlignY=38&desc=Full-Stack%20Engineer%20%C2%B7%20Chile&descSize=15&descAlignY=60&animation=twinkling" width="100%" alt="Diego Bravo Opazo" />

[![Typing SVG](https://readme-typing-svg.demolab.com?font=IBM+Plex+Mono&weight=500&size=17&duration=2800&pause=900&color=C9A36A&center=true&vCenter=true&width=760&height=34&lines=Codex+Orchestra+%C2%B7+local+control+plane+for+Codex;CalculaChile+%C2%B7+%2B2%2C000+organic+visits+%2F+month;Sitiazo+%C2%B7+production+websites+for+Chilean+SMBs)](https://github.com/falopass/Codex-Orchestra)

</div>

Full-stack engineer based in Chile. I design, build, deploy and operate what I ship: developer tooling, YMYL consumer products and client websites.

Python since 2020 · Spanish (native) · English (C1–C2) · Ingeniería Civil en Computación, Universidad de Talca.

---

## Flagship

<table>
<tr>
<td>

### [Codex Orchestra](https://github.com/falopass/Codex-Orchestra)

**Windows-first local control plane for [Codex](https://github.com/openai/codex) and an external Codex Router.** It keeps Router health, logical team roles, managed project files and diagnostics coherent without becoming a second chat UI. Public surface is plugin-first: skills plus a local stdio MCP; the Tauri desktop app is the advanced UI.

- Redacted health for Codex, Router, providers and thread control; secrets never leave local stores
- Router lifecycle (detect / doctor / start / restart / logs / update / rollback) behind `confirm=true`
- Managed `AGENTS.md` writes with preview, backup, atomic rename and rollback
- 13 MCP tools · MIT · CI on every push

[![CI](https://github.com/falopass/Codex-Orchestra/actions/workflows/ci.yml/badge.svg)](https://github.com/falopass/Codex-Orchestra/actions/workflows/ci.yml)
[![License: MIT](https://img.shields.io/badge/License-MIT-1F4B3A.svg)](https://github.com/falopass/Codex-Orchestra/blob/main/LICENSE)
![Status](https://img.shields.io/badge/status-v0.1.0_alpha-C9A36A)
![Rust](https://img.shields.io/badge/Rust-Tauri_2-DEA584?logo=rust&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-contracts-3178C6?logo=typescript&logoColor=white)
![Python](https://img.shields.io/badge/Python-plugin_%2B_MCP-3776AB?logo=python&logoColor=white)

```powershell
codex plugin marketplace add falopass/Codex-Orchestra
codex plugin add codex-orchestra@codex-orchestra
```

`orchestra_status` · `orchestra_doctor` · `orchestra_models` · `orchestra_team` · `orchestra_router` · `orchestra_worktrees` · +7 more

</td>
</tr>
</table>

---

## In production

<table>
<tr>
<td width="50%" valign="top">

### [CalculaChile](https://calculadorachile.cl)

Labor, tax and finance calculators for Chile. **YMYL vertical**: every formula maps to a verified official source and a test. Live UF / UTM / USD / EUR from the Central Bank with snapshot fallback. SEO-first, AdSense-monetized.

**+2,000 organic visits per month.**

39 active calculators · 12 pillar guides · blog

[Repo](https://github.com/falopass/calculadorachile) · [Sueldo líquido](https://calculadorachile.cl/calculadoras/calculadora-sueldo-liquido) · [IVA](https://calculadorachile.cl/calculadoras/calculadora-iva) · [Finiquito](https://calculadorachile.cl/calculadoras/calculadora-finiquito)

`Next.js 15` · `React 19` · `TypeScript` · `Tailwind 3` · `Vitest` · `Vercel`

</td>
<td width="50%" valign="top">

### [Sitiazo](https://sitiazo.cl)

Boutique web studio for Chilean SMBs. Conversion-oriented sites, static export, delivered in 7 days, from **$79,990 CLP**. Published case study: Roma Crochet.

[Repo](https://github.com/falopass/s-tialo) · [sitiazo.cl](https://sitiazo.cl)

`Next.js 16` · `TypeScript` · `Tailwind v4` · `Framer Motion 11` · static export

</td>
</tr>
</table>

---

## Stack across these projects

| Layer | Choices |
|-------|---------|
| Tooling | Rust / Tauri 2 · TypeScript contracts · Python plugin + MCP |
| Web | Next.js 15–16 · React 19 · TypeScript · Tailwind · Framer Motion |
| Quality | Vitest · typecheck · CI · YMYL audit scripts |
| Shipping | Vercel · Windows-first local tooling |

---

## Now

- Hardening Orchestra `v0.1.0` alpha: plugin, doctor, team roles, Router lifecycle
- Keeping CalculaChile sources verified and public URLs stable
- Growing Sitiazo as the client-facing channel

---

## Contact

[ddiegosebastianbb@gmail.com](mailto:ddiegosebastianbb@gmail.com)

Open to full-time roles with visa sponsorship (Netherlands, Ireland, Germany, Australia, New Zealand).

<details>
<summary>Español</summary>

Ingeniero full-stack en Chile. Diseño, construyo, despliego y opero lo que publico.

- **[Codex Orchestra](https://github.com/falopass/Codex-Orchestra)** (principal): control plane local para Codex y Router externo. Plugin + MCP stdio, desktop Tauri como UI avanzada. Alpha `v0.1.0`, MIT.
- **[CalculaChile](https://calculadorachile.cl)**: 39 calculadoras laborales, tributarias y financieras con fuentes oficiales verificadas y tests. +2.000 visitas orgánicas/mes.
- **[Sitiazo](https://sitiazo.cl)**: estudio web para pymes chilenas, static export, entrega en 7 días, desde $79.990.

Contacto: [ddiegosebastianbb@gmail.com](mailto:ddiegosebastianbb@gmail.com)

</details>

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&height=90&section=footer&color=0:0C1210,50:1A2A24,100:0C1210&animation=twinkling" width="100%" alt="" />

</div>

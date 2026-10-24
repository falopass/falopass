<p align="center">
  <img src="https://raw.githubusercontent.com/falopass/falopass/main/assets/banner.svg" width="100%" alt="Diego Bravo Opazo, full-stack engineer from the Maule, Chile" />
</p>

<p align="center">
  <a href="mailto:ddiegosebastianbb@gmail.com"><img src="https://img.shields.io/badge/email-ddiegosebastianbb%40gmail.com-C9A36A?style=flat-square&labelColor=0C1210" alt="Email" /></a>
  <img src="https://img.shields.io/badge/based_in-Regi%C3%B3n_del_Maule%2C_Chile-5EE4A3?style=flat-square&labelColor=0C1210" alt="Based in Región del Maule, Chile" />
  <img src="https://img.shields.io/badge/aka-Sovran-E8743B?style=flat-square&labelColor=0C1210" alt="aka Sovran" />
</p>

```text
diego@maule:~$ whoami

   ▗▖   arica          name       Diego Bravo Opazo
   ▐▌                  aka        Sovran
   ▐▌                  role       full-stack engineer, solo builder
   ▐▌   atacama        does       design · build · deploy · operate
   ▐▌                  school     Ing. Civil en Computación · Universidad de Talca
   ▐▙   santiago       python     since 2020
   ▐█ ◄── maule        home       Región del Maule, Chile
   ▐▌                  speaks     Spanish (native) · English (C1–C2)
   ▝▙   biobío
    ▐▌
    ▝▚▖ chiloé
     ▝▚▖
       ▝▀▚▄  magallanes
```

```text
diego@maule:~$ ls -l ~/ship

drwxr-xr-x  calculachile/   46 calculators · sourced formulas · +2,000 visits/mo
drwxr-xr-x  brasa/          wildfire alerts by place · satellites every 10 min
drwxr-xr-x  sitiazo/        websites for SMBs · demo in 48 h · live in 7 days
```

<br />

<a href="https://calculadorachile.cl"><img src="https://raw.githubusercontent.com/falopass/falopass/main/assets/calculachile.svg" width="100%" alt="CalculaChile: 46 labor, tax and finance calculators for Chile" /></a>

**Labor, tax and finance calculators for Chile.** Sueldo líquido, finiquito, IVA and dozens more: the numbers people use to sign a contract, quit a job or file taxes. That is a YMYL vertical, so the rule is simple: **no formula ships without an official source and a test.**

```text
  official source ──► formula ──► test (vitest) ──► calculator ──► indexed page
                         ▲
                         │   UF · UTM · USD · EUR
  Banco Central ─────────┘   live, with snapshot fallback when the API is down
```

- **46 calculators** live, plus guides and a blog
- **+2,000 organic visits per month**, SEO-first, AdSense-monetized
- Stable public URLs: a calculator, once indexed, keeps its address

[calculadorachile.cl](https://calculadorachile.cl) · [Sueldo líquido](https://calculadorachile.cl/calculadoras/calculadora-sueldo-liquido) · [Finiquito](https://calculadorachile.cl/calculadoras/calculadora-finiquito) · [IVA](https://calculadorachile.cl/calculadoras/calculadora-iva) · [repo](https://github.com/falopass/calculadorachile)

![Next.js](https://img.shields.io/badge/Next.js_15-0C1210?style=flat-square&logo=nextdotjs&logoColor=white)
![React](https://img.shields.io/badge/React_19-0C1210?style=flat-square&logo=react&logoColor=61DAFB)
![TypeScript](https://img.shields.io/badge/TypeScript-0C1210?style=flat-square&logo=typescript&logoColor=3178C6)
![Tailwind](https://img.shields.io/badge/Tailwind_3-0C1210?style=flat-square&logo=tailwindcss&logoColor=06B6D4)
![Vitest](https://img.shields.io/badge/Vitest-0C1210?style=flat-square&logo=vitest&logoColor=6E9F18)
![Vercel](https://img.shields.io/badge/Vercel-0C1210?style=flat-square&logo=vercel&logoColor=white)

<br />

<a href="https://github.com/falopass/brasas"><img src="https://raw.githubusercontent.com/falopass/falopass/main/assets/brasa.svg" width="100%" alt="BRASA Chile: wildfire alerts by place, from satellite detections every 10 minutes" /></a>

> *«¿Mi casa, mi parcela o mi familia están en riesgo hoy, y qué debo hacer?»*

**BRASA answers one question.** Save the places you care about; it watches the satellites, groups detections into incidents and tells you when a reliable hotspot appears inside your radius. It complements SENAPRED and CONAF and never competes with them.

```text
  NOAA GOES-East ─┐ every 10 min
  NASA VIIRS ─────┤
  NASA FIRMS ─────┼─► ingest ─► cluster ─► incident ─► alert by place ─► Web Push
  CONAF ──────────┘                │           │                          Telegram
                            volcanoes and   only CONAF can
                            industry are    mark it "confirmed"
                            filtered out

  Open-Meteo ────────► 30-30-30 risk per comuna, 7 days, hour by hour
                       temp > 30 °C  ·  humidity < 30 %  ·  wind > 30 km/h
```

```text
  incident lifecycle

  señal de calor ─► posible incendio ─► visto por vecinos
                 ─► confirmado por CONAF ─► controlado ─► sin calor nuevo

  an alert turns URGENT when
    ├─ the wind blows from the hotspot toward your place
    ├─ the hotspot is ≤ 2 km away
    └─ or ≤ 5 km away on a high-risk day
```

- **Historical replays**, hour by hour, every figure with its source and date:

  ```text
  2011-12 ─────── 2014 ─────── 2017 ─────────── 2023 ─────────── 2024 ─────── 2026
  Torres del     Valparaíso   Las Máquinas    Ñuble · Biobío   Viña del     Penco ·
  Paine                                       · Araucanía      Mar          Lirquén
  ```

- **No simulated data.** Everything on screen shows source, time and confidence; if a source fails, the UI says so
- **Privacy by default.** Citizen photo reports are re-encoded without EXIF/GPS and nothing is published without human review
- **Emergency mode**: one screen with distance, what the authority said, calls to 132 and 130, and four steps

> [!WARNING]
> Independent prototype, not affiliated with CONAF, SENAPRED or NASA/NOAA. **Never use it to decide an evacuation**: official alerts (SAE on your phone) remain the authority.

[repo](https://github.com/falopass/brasas) · AGPL-3.0

![Python](https://img.shields.io/badge/Python_3.12-0C1210?style=flat-square&logo=python&logoColor=FFD43B)
![FastAPI](https://img.shields.io/badge/FastAPI-0C1210?style=flat-square&logo=fastapi&logoColor=009688)
![Shapely](https://img.shields.io/badge/Shapely_%C2%B7_NumPy_%C2%B7_h5py-0C1210?style=flat-square&logo=numpy&logoColor=4DABCF)
![PWA](https://img.shields.io/badge/PWA_%C2%B7_Web_Push-0C1210?style=flat-square&logo=pwa&logoColor=5A0FC8)
![Telegram](https://img.shields.io/badge/Telegram-0C1210?style=flat-square&logo=telegram&logoColor=26A5E4)
![Docker](https://img.shields.io/badge/Docker-0C1210?style=flat-square&logo=docker&logoColor=2496ED)

<br />

<a href="https://sitiazo.cl"><img src="https://raw.githubusercontent.com/falopass/falopass/main/assets/sitiazo.svg" width="100%" alt="Sitiazo: websites for Chilean SMBs, free demo in 48 hours, live in 7 business days" /></a>

**A web studio for Chilean SMBs, run from Curicó.** The pitch is the process: you see your website before paying a peso.

```text
  day 0                        48 h                          7 business days
  ──●────────────────────────────●──────────────────────────────●──────►
    send your Instagram          free demo on WhatsApp,          published,
    or Google Business profile   built with your real photos     if you like it
```

| Plan | Price (CLP) | Pages | Ready in |
|---|---:|---:|---:|
| Básico | $79.990 · or $12.990 / mo with hosting and domain | 1 | 7 business days |
| Recomendado | $129.990 | up to 5 | 10 business days |
| Catálogo | $199.990 | up to 10 | 14 business days |

Every plan splits into 3 interest-free installments. **624 demos** across industries, and a published case study: Rancho Itahue.

[sitiazo.cl](https://sitiazo.cl) · [repo](https://github.com/falopass/s-tialo)

![Next.js](https://img.shields.io/badge/Next.js_16-0C1210?style=flat-square&logo=nextdotjs&logoColor=white)
![React](https://img.shields.io/badge/React_19-0C1210?style=flat-square&logo=react&logoColor=61DAFB)
![TypeScript](https://img.shields.io/badge/TypeScript-0C1210?style=flat-square&logo=typescript&logoColor=3178C6)
![Tailwind](https://img.shields.io/badge/Tailwind_v4-0C1210?style=flat-square&logo=tailwindcss&logoColor=06B6D4)
![Framer Motion](https://img.shields.io/badge/Framer_Motion_11-0C1210?style=flat-square&logo=framer&logoColor=white)
![Static export](https://img.shields.io/badge/static_export-0C1210?style=flat-square)

<br />

## How I build

```text
  01  every number has a source   official formulas · Banco Central · CONAF · NOAA
  02  if a source fails, say it   snapshot fallbacks, visible status, no fake data
  03  privacy is a default        photos stripped of EXIF, nothing unreviewed goes live
  04  static when it can be       less to run, less to break, faster for the user
  05  one person can maintain it  boring stack, tests wherever money is at stake
  06  ship, then operate          a deploy is not done until it is verified live
```

<p align="center">
  <img src="https://skillicons.dev/icons?i=python,fastapi,ts,react,nextjs,tailwind,docker,linux,vercel,git" alt="Python, FastAPI, TypeScript, React, Next.js, Tailwind, Docker, Linux, Vercel, Git" />
</p>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/falopass/falopass/output/github-contribution-grid-snake-dark.svg" />
    <img src="https://raw.githubusercontent.com/falopass/falopass/output/github-contribution-grid-snake.svg" width="100%" alt="Contribution graph eaten by a snake" />
  </picture>
</p>

<details>
<summary><b>En español</b></summary>

<br />

Ingeniero full-stack de la Región del Maule. Diseño, construyo, despliego y opero lo que publico. Ingeniería Civil en Computación, Universidad de Talca. Python desde 2020.

- **[CalculaChile](https://calculadorachile.cl)**: 46 calculadoras laborales, tributarias y financieras. Cada fórmula tiene fuente oficial y test; UF, UTM, USD y EUR en vivo desde el Banco Central. Más de 2.000 visitas orgánicas al mes.
- **[BRASA Chile](https://github.com/falopass/brasas)**: alertas ciudadanas de incendios forestales por lugar, riesgo 30-30-30 por comuna y reconstrucción de incendios históricos. Prototipo independiente, no afiliado a CONAF ni SENAPRED; no sirve para decidir una evacuación.
- **[Sitiazo](https://sitiazo.cl)**: páginas web para pymes chilenas desde Curicó. Demo gratis en 48 horas por WhatsApp y publicada en 7 días hábiles, desde $79.990.

Contacto: [ddiegosebastianbb@gmail.com](mailto:ddiegosebastianbb@gmail.com)

</details>

```text
───────────────────────────────────────────────────────────────────────────
   hecho en el Maule, Chile  ·  calculadorachile.cl  ·  sitiazo.cl  ·  brasa
───────────────────────────────────────────────────────────────────────────
```

<div align="center">

# Hey, I'm Suhas 👋

**I build things end-to-end, then break them on purpose to see if they hold.**

`Python` · `JavaScript` · `TypeScript` · `C` · `Java` · `SQL` · `HTML/CSS`

[![SourceShelf](https://img.shields.io/badge/🔎_SourceShelf-1%2C619_apps_indexed-2ea44f?style=flat-square)](https://github.com/storm201/sourceshelf)
[![GeoFUSE](https://img.shields.io/badge/🛰️_GeoFUSE-SIH_2026-1f6feb?style=flat-square)](https://github.com/storm201/GEOFUSE)
[![ATLA](https://img.shields.io/badge/🌍_ATLA-React_+_Flask-8957e5?style=flat-square)](https://github.com/storm201/ATLA)
[![Email](https://img.shields.io/badge/✉️_suhasbannikal@gmail.com-EA4335?style=flat-square)](mailto:suhasbannikal@gmail.com)

</div>

---

I learn by shipping. An idea turns into a repo, the repo turns into a crawler, a
database, a test suite, and eventually something that runs every night without me
checking on it like a nervous parent.

Three things I keep coming back to: **data pipelines that survive real APIs**,
**full-stack apps where the caching is actually thought through**, and **stating
honestly what a system can and cannot do**. That last one is rarer than it should
be. Turns out "here are the failure cases" is a feature, not an apology.

---

## 🚀 Flagship Projects

### 🔎 [SourceShelf](https://github.com/storm201/sourceshelf)
*A searchable catalog of **1,619 installable apps** across 23 categories and 10
platforms, re-crawled from the GitHub API every night at 03:17 UTC, with **276
direct download links** resolved from real release assets (`.exe`, `.dmg`,
`.AppImage`, `.apk`).*

- **Zero-server architecture.** GitHub Actions crawls, rebuilds, commits and
  deploys. Supabase free tier plus GitHub Pages. No backend to babysit, no bill to
  explain to anyone.
- **Open submissions, automated approvals.** Anyone can propose an app through a
  GitHub issue template, and an approval workflow validates the repo and commits it
  into the catalog. The project now accepts contributions without me being the
  bottleneck.
- **Honest edge cases.** When the API rate limit hits, the crawler falls back to
  scraping GitHub's release HTML pages instead of quietly giving up. The
  "Download" vs "Get app" button tells you *why* a binary doesn't exist, which is
  more than most app stores manage.
- **History, not guesses.** A `first_seen` column in Supabase is the only
  reliable way to answer "what appeared today." GitHub's search API knows what
  exists now, and nothing about yesterday.
- **Tested offline.** 22 assertions against a mock PostgREST server, so the storage
  layer is verifiable without signing up for anything. It caught bugs before a real
  database ever did.
- **Fast by subtraction.** Vanilla JS, in-memory index, 48-card
  `IntersectionObserver` paging. No framework, no external scripts, no analytics
  quietly reporting home. Oh, and SECURITY.md, Dependabot, and a documented
  hardening pass, because "it's only a static site" is how static sites get owned.

`Python` `Supabase` `GitHub Actions` `Vanilla JS` `RSS` `GitHub API`

### 🛰️ [GeoFUSE SentinelGuard](https://github.com/storm201/GEOFUSE)
*Deep-learning super-resolution for Sentinel-2 satellite imagery, built for
**Smart India Hackathon 2026** around one stubborn rule: sharper pixels must
arrive with evidence attached.*

- **Trust Receipts.** Every reconstructed tile ships a machine-readable JSON of
  uncertainty, stability and spectral-consistency checks. You get the sharper image
  and the reasons to believe it, in one package.
- **Research hygiene over leaderboard scores.** Contiguous geographic hold-out
  split, because random patch splitting leaks spatially correlated tiles and
  inflates your numbers. Flattering metrics from a leaky split are just lies with
  decimal places.
- **Measured, not claimed.** +0.49 dB PSNR and +0.0062 SSIM over the bicubic
  baseline, reported alongside ΔNDVI and edge-F1 instead of buried under them.
- **Full stack.** PyTorch ensemble backend on FastAPI, React inspection UI,
  Streamlit fallback, a 5x5 interactive tile grid, and a split-curtain
  before/after viewer for when a screenshot needs to do the arguing.

`Python` `PyTorch` `FastAPI` `React` `Streamlit` `Remote Sensing`

### 🌍 [ATLA](https://github.com/storm201/ATLA)
*A country intelligence platform that merges the REST Countries and World Bank
APIs into one analytics view: rankings, comparisons, and an interactive 3D globe.*

- **Two-layer caching.** In-memory for speed, SQLite for durability, with datasets
  preloaded on startup so the first ranking request isn't the one that suffers.
- **Real visualizations.** Three.js globe, D3-Geo projections, Recharts radar
  charts for side-by-side country comparison across GDP, population, literacy,
  internet usage and life expectancy.
- **Production habits on a hobby project.** Flask-Limiter rate limiting, CORS,
  security headers, input validation, and Waitress instead of the dev server.
- **The hard part was the data.** Two APIs with different shapes, different
  country name spellings and different update cadences. Normalizing that is 80% of
  the work and none of the screenshot.

`React` `TypeScript` `Vite` `TailwindCSS` `Three.js` `Flask` `SQLite` `Waitress`

---

## 🌱 Also Built

### 🌿 [Growth Garden](https://github.com/storm201/Growth-Garden)
*A visual journaling app where goals, habits and memories become plants in a
digital garden. Progress feels alive instead of measured.*

- Plants grow through stages based on how often you write: Seedling at 0 updates,
  Sprout at 1 to 3, Young Tree at 4 to 7, Mature Tree at 8+.
- Four garden beds (Goals, Projects, Habits, Memories), a per-plant timeline, a
  photo gallery, and a dashboard summarizing total plants, updates and mature trees.
- Safe deletion cascades through related updates, photos and uploaded files, so the
  database doesn't quietly rot.
- Flask, SQLite, SQLAlchemy, and CSS written by hand on purpose. No framework, no
  gradient soup.

`Python` `Flask` `SQLAlchemy` `SQLite` `CSS`

### 📊 [Country-Report](https://github.com/storm201/Country-Report) · [data-analysis](https://github.com/storm201/data-analysis)

Where I learned to stop trusting a dataset on the first read. Country-Report pulls
population, GDP, life expectancy and internet usage through the REST Countries and
World Bank APIs. The data-analysis repos are Pandas and Matplotlib work on real
datasets, including all the boring cleaning that never makes the chart.

ATLA is what Country-Report turned into once I wanted rankings, comparisons and a
frontend. Consider this the origin story with worse CSS.

`Python` `Requests` `Pandas` `Matplotlib` `REST APIs`

---

## 🛠️ Tech I Actually Reach For

| | |
|---|---|
| **Languages** | `Python` `TypeScript` `JavaScript` `SQL` `C` `Java` `HTML` `CSS` |
| **Data & ML** | `Pandas` `Matplotlib` `PyTorch` `NumPy` |
| **Frontend** | `React` `Vite` `TailwindCSS` `Three.js` `D3` `Recharts` |
| **Backend & Infra** | `Flask` `FastAPI` `SQLAlchemy` `SQLite` `Supabase` `GitHub Actions` `Git` |

---

<div align="center">

**Currently:** hardening SourceShelf's nightly pipeline and its issue-driven
submission flow, reading up on how to evaluate ML systems properly<br/>
**Open to:** interesting problems, weird ideas, and code reviews that sting a little

[GitHub](https://github.com/storm201) · [Email](mailto:suhasbannikal@gmail.com)

<i>Still building. Still breaking things. Still fixing them before anyone notices.</i> ✌️

</div>

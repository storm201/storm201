<div align="center">

# Hey, I'm Suhas 👋

**I build things end-to-end, then break them on purpose to see if they hold.**

`Python` · `JavaScript` · `C` · `Java` · `SQL` · `HTML/CSS`

[![SourceShelf](https://img.shields.io/badge/🔎_SourceShelf-1%2C619_apps_live-2ea44f?style=flat-square)](https://github.com/storm201/sourceshelf)
[![GeoFUSE](https://img.shields.io/badge/🛰️_GeoFUSE-SIH_2026-1f6feb?style=flat-square)](https://github.com/storm201/GEOFUSE)
[![Email](https://img.shields.io/badge/✉️_suhasbannikal@gmail.com-EA4335?style=flat-square)](mailto:suhasbannikal@gmail.com)

</div>

---

I learn by shipping. An idea turns into a repo, the repo turns into a crawler, a
database, a test suite, and eventually something that runs every night without me
checking on it like a nervous parent.

Three things I keep coming back to: **data pipelines that survive real APIs**,
**frontends with no build step that still feel fast**, and **stating honestly what
a system can and cannot do**. That last one is rarer than it should be. Turns out
"here are the failure cases" is a feature, not an apology.

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
- **Honest edge cases.** When the API rate limit hits, the crawler falls back to
  scraping GitHub's release HTML pages instead of quietly giving up. The
  "Download" vs "Get app" button tells you *why* a binary doesn't exist, which is
  more than most app stores manage.
- **History, not guesses.** A `first_seen` column in Supabase is the only
  reliable way to answer "what appeared today." GitHub's search API knows what
  exists now, and nothing about yesterday.
- **Tested offline.** 22 assertions against a mock PostgREST server, so the
  storage layer is verifiable without signing up for anything. It caught bugs
  before a real database ever did.
- **Fast by subtraction.** Vanilla JS, in-memory index, 48-card
  `IntersectionObserver` paging. No framework, no external scripts, no analytics
  quietly reporting home.

`Python` `Supabase` `GitHub Actions` `Vanilla JS` `RSS` `GitHub API`

### 🛰️ [GeoFUSE SentinelGuard](https://github.com/storm201/GEOFUSE)
*Deep-learning super-resolution for Sentinel-2 satellite imagery, built for
**Smart India Hackathon 2026** around one stubborn rule: sharper pixels must
arrive with evidence attached.*

- **Trust Receipts.** Every reconstructed tile ships a machine-readable JSON of
  uncertainty, stability and spectral-consistency checks. You get the sharper
  image and the reasons to believe it, in one package.
- **Research hygiene over leaderboard scores.** Contiguous geographic hold-out
  split, because random patch splitting leaks spatially correlated tiles and
  inflates your numbers. Flattering metrics from a leaky split are just lies with
  decimal places.
- **Measured, not claimed.** +0.49 dB PSNR and +0.0062 SSIM over the bicubic
  baseline, reported alongside ΔNDVI and edge-F1 instead of buried under them.
- **Full stack.** PyTorch ensemble backend on FastAPI, React inspection UI,
  Streamlit fallback, and a split-curtain before/after viewer for when a
  screenshot needs to do the arguing.

`Python` `PyTorch` `FastAPI` `React` `Streamlit` `Remote Sensing`

### ⚡ [ATLA](https://github.com/storm201/ATLA) · 🌱 [Growth Garden](https://github.com/storm201/Growth-Garden)

Two builds where the point *is* the interface: a TypeScript world built around
Avatar: The Last Airbender, and a CSS-driven study in motion and interaction.
Design work with actual code underneath it, rather than a mockup and a promise.

`TypeScript` `CSS`

### 📊 [Country-Report](https://github.com/storm201/Country-Report) · [data-analysis](https://github.com/storm201/data-analysis)

Python projects where I learned to stop trusting a dataset on the first read.
Pulling country data through live APIs, then digging through real datasets with
Pandas and Matplotlib until the numbers made sense.

`Python` `Pandas` `Matplotlib` `REST APIs`

---

## 🛠️ Tech I Actually Reach For

| | |
|---|---|
| **Languages** | `Python` `JavaScript` `TypeScript` `C` `Java` `SQL` `HTML` `CSS` |
| **Data & ML** | `Pandas` `Matplotlib` `PyTorch` `NumPy` |
| **Web & Infra** | `Flask` `FastAPI` `React` `Supabase` `GitHub Actions` `Git` |

---

## 📊 By the Numbers

<p align="center">
  <img height="160" src="https://github-readme-stats.vercel.app/api?username=storm201&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" />
  <img height="160" src="https://github-readme-stats.vercel.app/api/top-langs/?username=storm201&layout=compact&theme=tokyonight&hide_border=true&langs_count=8" />
</p>

---

<div align="center">

**Currently:** hardening SourceShelf's nightly pipeline · reading up on how to
evaluate ML systems properly
**Open to:** interesting problems, weird ideas, and code reviews that sting a
little

[GitHub](https://github.com/storm201) · [Email](mailto:suhasbannikal@gmail.com)

<i>Still building. Still breaking things. Still fixing them before anyone notices.</i> ✌️

</div>

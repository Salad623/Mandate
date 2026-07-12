# MANDATE — Living President Simulator v0.2

A self-contained, mobile-friendly browser strategy game where the player governs a real country through economic pressure, cabinet conflict, coalition politics, voter blocs, delayed consequences, crises, elections, corruption, and international affairs.

No framework, build step, API key, or database is required for this version.

## Run locally

Open `index.html` in a modern browser.

For more reliable browser storage, run a local server:

```bash
python3 -m http.server 8080
```

Then open `http://localhost:8080`.

## Deploy on GitHub Pages

1. Create a public GitHub repository.
2. Upload `index.html` to the repository root.
3. Open **Settings → Pages**.
4. Select **Deploy from a branch**.
5. Choose `main` and `/root`, then save.

## Major systems in v0.2

- Eight playable countries with different political structures, baselines, constraints, and term rules
- Real-world daily presidential briefing tied to the browser calendar
- Three short daily decisions with uncertain advice and delayed consequences
- Daily streak, completed briefings, and unresolved consequence queue
- Eight cabinet ministers with competence, loyalty, ambition, integrity, ideology, resignation, leaks, misconduct, dismissal, and replacement
- Eight voter blocs with separate priorities and support levels
- Coalition and parliamentary factions that must be negotiated with
- Campaign promises, debates, opposition polling, elections, succession contests, and party congresses
- Monthly GDP, GDP per capita, inflation, unemployment, tax revenue, spending, debt, interest rates, exchange-rate confidence, foreign reserves, and growth
- Seven economic sectors: agriculture, manufacturing, services, technology, energy, tourism, and construction
- Country-specific economic and political pressures
- Permanent legislation with voter-group effects
- Multi-year infrastructure projects with delays, overruns, corruption leakage, and long-term benefits
- Bribery, patronage, abuse of agencies, scandal exposure, investigations, and removal from office
- Trade missions, foreign aid, sanctions, diplomatic relationships, influence, and global rankings
- Generated newspaper front pages and shareable headlines
- Persistent presidential profile, legacy score, promises, laws, projects, scandals, and timeline
- Local browser saving plus JSON export and import
- Responsive desktop and mobile interface

## Tested

- JavaScript syntax validation
- Desktop and mobile interface checks
- Navigation and interaction tests for every new section
- Twenty-four simulated months for all eight countries
- No `NaN`, undefined economic values, or runtime errors during the test run

## Current limitation

This release is fully playable but remains serverless. Real user accounts, cloud synchronization, multiplayer seasons, live diplomacy between human presidents, public leaderboards, and community scenario hosting require a backend and database. The current export/import system is the bridge toward that architecture.

## Data note

Starting values are simplified game baselines inspired by public macroeconomic indicators. They are not live forecasts and should not be presented as exact current statistics.

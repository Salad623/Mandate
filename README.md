# MANDATE v0.15 — Main Menu Restored

Open `index.html` in a modern browser. The game is a single-file browser simulation and stores the current career locally in the browser.

## Correct launch flow

1. The game always opens on the **Main Menu**.
2. **New Game** opens the role and country setup.
3. Choose one role, one country, and a leader or organization name.
4. Starting the new career replaces the previous local save after confirmation.
5. **Continue** appears only when a valid save exists.
6. The in-game **Menu** button saves the current career and returns to the Main Menu.

## Single-career rule

Each save contains one playable entity. The player cannot manually switch to another country, organization, or company during the run. A different starting entity requires returning to the Main Menu and beginning a new game. Political transformations caused by gameplay, such as losing office and becoming opposition, remain possible.

## Main systems retained

- 142-sector economic and supply-chain simulation
- Taxation, budgets, deficits, debt, and credit ratings
- Central-bank rates, currencies, exchange rates, stock markets, and international lenders
- Government, cabinet, workforce, intelligence, and crisis management
- Parliament, legislation, referendums, laws, and repeals
- Infrastructure, energy, industrial, and long-term projects
- National data, demographics, security, services, environment, culture, and science

## Deployment

Upload `index.html` to any static host such as GitHub Pages, Netlify, or Cloudflare Pages. No server is required for the local single-player build.

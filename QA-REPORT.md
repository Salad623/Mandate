# MANDATE 1.0C — Full QA Report

**Test date:** July 12, 2026  
**Build:** Version 1.0C Trade & Economic Diplomacy — QA Hotfix  
**Primary file:** `index.html`

## Result

**PASS with one regression found and repaired.**

The test run found that the real Main Menu had been lost during the Version 1.0C merge. The game could still start, but it opened directly into setup or a saved world. The build was patched so it now launches on the Main Menu, supports New Game and Continue, provides a Back button during setup, and returns safely to the menu from an active career.

## Automated and interaction tests passed

### Startup, menu, saves, and careers

- JavaScript syntax validation
- No duplicate static HTML IDs
- Main Menu is the first screen
- Continue is disabled when no save exists
- New Game opens the setup screen
- Setup Back button returns to the Main Menu
- Take Control starts the selected career
- In-game Menu button saves and returns to the Main Menu
- Continue restores the saved country, date, and career
- Single-entity career lock remains enforced
- All four starting roles launch:
  - National leader
  - Legal opposition leader
  - Underground movement leader
  - Multinational CEO
- All eight playable countries launch and advance through simulation time

### Navigation and responsive interface

All major navigation workspaces were opened and checked for rendered content for every playable role:

- Overview
- Operations
- Government
- Tax & Budget
- Money & Markets
- Trade & Diplomacy
- Sector Economy
- Bills
- Laws
- Projects
- Nation Data
- Opposition
- Rankings
- Timeline

Mobile navigation was tested at a 390 × 844 viewport with no page-wide horizontal overflow.

### Core simulation

- 24 consecutive monthly turns
- Random decision handling
- State remained numerically finite
- No `NaN`, `Infinity`, or undefined economic values detected
- No JavaScript page exceptions during the completed test paths

### Government management

- Minister appointment, replacement, dismissal, and vacancies
- Ministry budget changes
- Government spending-envelope changes
- National spending priorities
- Public-sector staffing and salary changes
- Head-of-state security funding
- Intelligence and counterintelligence funding
- Government-crisis generation and responses

### Taxation and public finance

- All 30 tax instruments increased and reduced
- All 12 spending allocations adjusted
- Overall spending target changed
- Bond issuance
- Debt repayment
- Fiscal-reserve action
- Deficit, debt, borrowing-cost, and rating calculations remained valid

### Monetary policy and financial markets

- Interest-rate cuts, holds, and increases
- Currency-regime controls
- Reserve intervention and currency-policy actions
- International lender negotiations
- Long-term national plans started and cancelled
- Credit, currency, and market state remained valid

### Trade and economic diplomacy

- Trade-agreement negotiations
- Embargo imposition and removal
- Import, export, energy, defense, and resource contracts
- Strategic-sector subsidies
- Cross-border infrastructure projects
- International institution influence
- Trade organizations
- Dynamic trade state remained valid

### Sector economy

- Exactly 142 sectors loaded
- Every sector detail modal opened and closed
- Subsidy, tariff, embargo, research, and procurement controls
- Supply-chain state remained numerically valid

### Parliament and laws

- At least 30 bill proposals loaded
- Every bill review modal opened
- Parliamentary-vote action executed
- 25-law catalog rendered
- Law detail actions opened correctly

### Projects and national data

- Transport, energy, industry, and public-service project categories
- Construction start and cancellation
- Every Nation Data section rendered
- National report generation
- Speech-control buttons invoked

## Important limits of this test

The build is a large procedural single-file game. Automated testing covered the main menus, buttons, controls, data mutations, save flow, and a 24-month simulation, but it cannot prove every rare random event or every possible multi-year branch. Browser speech controls were invoked, although audible sound cannot be verified in a headless test browser. The current build is serverless, so backend accounts, cloud saves, and real multiplayer were not tested because they are not part of Version 1.0C.

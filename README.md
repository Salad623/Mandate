# MANDATE — Global Power Simulator v0.14

A mobile-friendly, single-player browser strategy game about governing a country, leading an opposition party, directing an underground movement, or running a multinational company.

Each new career is locked to one playable entity. Changing the starting role or country requires beginning a new game.

## v0.14: 142-sector economic engine

The new **Sector Economy** page models 142 connected industries across 12 groups:

- Agriculture and natural production
- Mining and raw materials
- Food processing
- Basic manufacturing
- Advanced manufacturing
- Energy and utilities
- Construction and infrastructure
- Transport and logistics
- Consumer services
- Business and financial services
- Digital and frontier technology
- Health, education, and the social economy

The catalog includes hydrogen, fertilizer, integrated food processing, medical equipment, mobile phones, lithium, uranium, mechanical components, humanoid robots, and generative AI.

### Variables tracked for every sector

Every industry changes monthly and stores its own:

- Production and productive capacity
- Domestic consumption and demand
- Imports, exports, and inventory
- Raw-material stocks and upstream dependencies
- Shortages and surpluses
- Product and input-price indexes
- Employment, hiring growth, and wages
- Productivity and profit margins
- Corporate tax rate and estimated tax revenue
- Innovation and strategic R&D
- Product quality
- CO₂ emissions
- Domestic and international competition
- Import dependence and export orientation
- Supply-chain risk
- Subsidies, tariffs, embargoes, procurement preferences, and ownership status

### Supply chains

Industries consume outputs from other industries. Shortages in an upstream sector therefore affect downstream capacity, costs, prices, and trade.

Examples include:

- Natural gas and phosphates → fertilizer → crops → food processing
- Lithium and chemicals → batteries → electric vehicles and grid storage
- Uranium and mechanical components → nuclear generation
- Semiconductors → mobile phones, medical equipment, robots, data centers, and AI
- Steel, cement, and machinery → construction, railways, power grids, and factories

### Player controls

A national government can open an individual sector and manually change:

- Production subsidy
- Import tariff
- Trade embargo status
- Strategic R&D priority
- Domestic state-procurement preference

These policies have trade-offs. Assistance may improve investment, capacity, employment, innovation, and product quality, while also increasing government spending, inflation, corruption risk, shortages, or foreign retaliation.

### Economic integration

The 142-sector engine feeds into the existing national simulation:

- GDP growth and industrial output
- Inflation and consumer prices
- Employment and unemployment
- Government tax revenue and subsidy spending
- Trade balance and currency pressure
- Business confidence and investment
- Energy reliability and raw-material security
- CO₂ emissions and environmental outcomes

It also responds to taxation, government spending, central-bank rates, exchange rates, credit ratings, international lending, infrastructure projects, and legislation.

## Other major systems

- Eight playable countries
- More than 1,300 national variables per country before sector-level expansion
- Government, cabinet, ministries, staffing, salaries, security, and intelligence
- 30 manually adjustable taxes and 12 spending allocations
- Public debt, deficits, credit ratings, sovereign yields, and lender negotiations
- Interest rates, currencies, exchange-rate regimes, reserves, and stock markets
- Parliament, party ideology, 50 proposals, referendums, and law repeal
- Transport, energy, industrial, and public-service projects
- Elections, opposition, corruption, scandals, crises, and political removal
- Nation Data, reports, rankings, timeline, and browser speech
- Automatic local-browser saves and save migration

## Running the game

1. Extract the ZIP archive.
2. Open `index.html` in a modern browser.
3. Choose one role and country, then start a career.

No framework, build step, database, API key, or internet connection is required.

## Testing performed for v0.14

- Verified exactly 142 sectors in a new country model
- Verified more than 5,700 numeric values in the expanded Philippine country model
- Rendered all nine Sector Economy views
- Tested sector search, category pages, supply chains, and trade-policy controls
- Verified all ten requested newer sectors
- Ran a 24-month national simulation
- Checked every sector for `NaN`, infinite, or undefined numeric values
- Tested subsidy changes and policy persistence
- Tested desktop and mobile layouts
- Validated embedded JavaScript syntax

## Data note

All sector values are internally generated game baselines. They are designed to produce plausible strategic relationships, not to reproduce current official statistics or serve as economic forecasts.
